# Forfattermetoden for LCCbyg-hjælpen

Dette dokument er kontrakten for AL forfatning af hjælpen — uanset om teksten
skrives af Claude Code, en anden AI eller et menneske. Konsistens er hele
pointen: hver side i appen har ét dokument, hvert vigtigt element har ét anker
og én sektion.

## Strukturen (helptree.json)

- `helptree.json` er den ene kilde til sandhed for træet: grupper og sider i
  samme rækkefølge som appens sidemenu. Panelets indholdsfortegnelse, ruterne
  bag "Vis mig hvor" og kurateringen i `buildhelp index` udledes af den.
- Ét dokument pr. side: `{context}.md`, hvor context er appens kanoniske
  rutenavn (`ProjectRoutes.HelpTopic` — fx `alternative-group-rows`).
- `shared.md` = elementer der findes overalt (toplinje, menu, fortryd/gendan).
  `faq.md` = ofte stillede spørgsmål (vokser via spørg-AI + `buildhelp fold`).
- Nye sider: tilføj til `helptree.json`, kør `buildhelp tree --content .` — så
  oprettes skelettet.
- `search: false` i front matter holder en side UDE af søgning og spørg-AI —
  den bliver i træet og kan læses som før, men hverken dens emner eller dens
  titel kan rammes af en søgning, og den koster ingen plads i vektorindekset.
  Til sider hvis ord ellers drukner rigtige emner: `about`, `versionhistory`,
  `licences`. `buildhelp index` skriver hvilke sider der er markeret.

## Strukturen pr. dokument

```markdown
---
title: "Sidens navn (som i menuen)"
---

Indledning uden overskrift: 2-4 sætninger. Hvad bruger du siden til, og
hvornår kommer du her? Ingen "velkommen til"-fyld.

### Elementnavn {#anker}
Hvad elementet gør, og hvornår du bruger det. 1-4 sætninger.

### Næste element {#andet-anker}
…
```

- Sektioner i **visuel rækkefølge**: top→bund, venstre→højre.
- Ankernavne: lowercase ascii-slug (æ→ae, ø→oe, å→aa), og navnet **skal**
  matche `HelpBubble`/`HelpAnchor` `Id` i koden. Ét anker pr. element eller
  naturlig elementgruppe.
- Dækker én sektion flere elementer: `<!-- anchors: id-et, id-to -->` i sektionen.

## Sproget

- Dansk, du-form, nutid. Kort og konkret: "Knappen opretter et nyt alternativ"
  — aldrig "man kan …" eller "denne funktionalitet muliggør …".
- Brug appens egne ord (samme betegnelser som i UI'et/AppResources).
- Ingen tabeller, billeder eller rå HTML. Links til andre emner er velkomne:
  `[Alternativer](alternatives.md#anker)`.
- Skriv hvad tingene GØR — aldrig hvad du gætter på, de gør.

## Arbejdsgangen

1. **Læs sidens .razor-kode** (og de vigtigste børnekomponenter), før du
   skriver ét ord. Beskrivelsen skal matche virkeligheden.
2. Wrap de væsentlige elementer i koden: `<HelpBubble Id="anker">…</HelpBubble>`
   (eller selvlukkende `<HelpBubble Id="anker" />` lige FØR elementet, hvis
   wrapping er akavet — blink-målingen tager så det næste element).
3. Skriv/opdater dokumentets sektioner, så alle ankre er dækket.
4. Genbrug eksisterende viden: visningernes beskrivelser står i
   `LcViews\Presets.cs`; de gamle hjælpetekster (popup.md m.fl.) er
   referencemateriale — aldrig skabelon.
5. Kør `buildhelp validate --content . --source <LccUi>` og derefter
   `buildhelp index --content . --version 40` (inkrementel — kun ændrede
   sektioner embeddes).

## Forfatterværktøjet i appen (kun debug)

Blyanten i hjælpevinduets titellinje (debug-builds) viser sidens status:
dokument/træ-medlemskab, ankre med/uden emne, og en scanner der finder
interaktive elementer uden anker. **"Kopiér forfatter-prompt"** lægger en
færdig opgavebeskrivelse i udklipsholderen — sæt den ind i Claude Code, og
ret teksten i samtalen.

## Guides (interaktive rundvisninger)

En guide er en trin-for-trin-rundvisning i appen: hvert trin fremhæver ét
element (maske med hul + ring), viser en kort tekst i en flydende boks og kan
bede brugeren om at klikke eller skrive — eller gøre det selv med **Vis mig**.
Guider ligger i hjælpetræet under gruppen **Guides** og er almindelige
markdown-filer, så de kan skrives af mennesker og AI på lige fod.

> **Kun i debug indtil videre.** Guider er stadig en udviklerfunktion: LCCbyg
> sætter `help.Guides = true` inde i `#if DEBUG`, så en release-build hverken
> viser Guides-gruppen i hjælpetræet, finder guider i søgningen eller genoptager
> en guide, der lå gemt i browseren. Guide-filerne bliver liggende i docs-repoet
> og i det indekserede katalog — der er kun tale om visningen. Når funktionen
> skal ud til brugerne, flyttes den ene linje ud af `#if DEBUG`.

### Filen

- Navn: `guide-<slug>.md` (præfikset er obligatorisk), i samme mappe som de
  øvrige dokumenter, og listet i `helptree.json` under gruppen "Guides"
  (uden `route`).
- Front matter: `title`, `type: guide`, valgfrit `start` (den rute guiden
  begynder på — `""` er forsiden), `requires`, evt. `project` og `description`.
- Indledning uden overskrift: 1-3 sætninger om hvad guiden fører til. Vises i
  panelet sammen med trinlisten og knappen **Start guide**.
- Hvert trin er en `## Trintitel {#anker}`-sektion. De første linjer efter
  overskriften er koder på formen `nøgle: værdi`; efter en blank linje følger
  brødteksten (1-3 sætninger: én handling pr. trin, skriv hvad brugeren skal
  gøre).
- En overskrift **uden** `{#anker}` er et rent tekst-trin (centreret boks,
  ingen maske) — til velkomst og afslutning.

```markdown
---
title: "Opret din første beregning"
type: guide
start: project
requires: new-project
description: Fra tomt projekt til de første rækker.
---

Guiden fører dig gennem de første skridt i en beregning.

## Giv projektet et navn {#stamoplysninger}
action: type
field: Projekttitel
value: Min første beregning
wait: value

Skriv projektets titel. Den vises i vinduets titel og i rapporterne.

## Gå til alternativerne {#nav-alternativer}
action: click
wait: page=alternatives

Klik på **Alternativer** i sidemenuen.

## Færdig
Du er igennem.
```

### Front matter

| Nøgle | Værdier | Betydning |
|---|---|---|
| `requires` | `new-project`, `project`, `none` (default) | `new-project`: appen spørger om lov til at lukke det åbne projekt og åbner den tomme standardskabelon, så guiden aldrig ændrer i brugerens eget projekt. `project`: guiden kan kun startes med et åbent projekt. |
| `project` | skabelonens filnavn uden endelse (fx `renoveringnybyggeri`) eller dens label | Kun med `requires: new-project`: åbner dette eksempelprojekt i stedet for den tomme skabelon, så guiden har rigtige tal at vise. Ukendt navn = fejlbesked og ingen start. |
| `start` | rute, fx `project` eller `""` | Siden guiden navigerer til ved start. Første trin arver den som sin side. |
| `description` | tekst | Én linje under titlen i panelet. |

### Koder pr. trin (alle valgfrie)

| Nøgle | Værdier | Default | Betydning |
|---|---|---|---|
| `page` | kontekst eller rute (`alternatives`, `results/dashboards/compares`) | arves fra forrige trin; første trin = `start` | Siden trinnet hører til. Er brugeren et andet sted, viser boksen "Trinnet hører til en anden side", og **Vis mig** navigerer derhen (hvis træet kender ruten). |
| `placement` | `auto`, `top-left`, `top`, `top-right`, `left`, `center`, `right`, `bottom-left`, `bottom`, `bottom-right` | `auto` | `auto` lægger boksen ved siden af elementet (højre → venstre → under → over); de andre låser den til en fast plads på skærmen. Brugeren kan altid trække boksen. |
| `action` | `click`, `type`, `select`, `none` | `none` | Hvad **Vis mig** gør: klikker på målet, skriver `value` i feltet, eller vælger `value` i en liste. |
| `field` | tekst, `name`, `data-help-field`, nummer eller kolonnetitel | – | Et delmål inde i ankeret, når ankeret dækker flere felter: feltets label/hjælpetekst, knappens tekst, et menupunkts tekst (også i en åben menu), eller det n'te inputfelt. I en tabel (fx rækkegridet): kolonnens titel rammer cellen i første datarække — `field: Mængde`; `field: Mængde:3` rammer tredje række. "Vis mig" klikker rækken i redigering, hvis cellen først får sit felt ved klik. |
| `value` | tekst | – | Det, `type`/`select` skriver eller vælger. |
| `mask` | `dim`, `none` | `dim` | `none` dropper den mørke maske og beholder kun ringen — til trin, hvor brugeren skal se resten af siden ændre sig (fx en søgeliste). |
| `wait` | `click`, `value`, `page=<kontekst>`, `none` | `none` | Auto-fremdrift: trinnet går selv videre, når målet klikkes, når feltets værdi ændres, eller når appen lander på siden. Uden `wait` skal brugeren trykke **Næste**. |

Danske stavemåder virker som aliaser (`side`, `placering`, `handling`, `felt`,
`vaerdi`, `vent`, `maske`, `kraever`, `beskrivelse`; værdier `klik`, `skriv`,
`vaelg`, `ingen`, `nyt-projekt`, `projekt`, `intet`), men skriv de engelske — de
er kontrakten.

### Regler

- Ankeret i overskriften **skal** findes som `HelpBubble`/`HelpAnchor` `Id` i
  appen. `buildhelp validate --source <LccUi>` afslører ankre, der ikke
  findes, sider (`page`, `wait: page=`) der ikke er i træet, og koder med
  ugyldige værdier.
- Peg på ét element ad gangen. Dækker ankeret et helt kort med flere felter,
  brug `field`.
- Sideskift: lad det trin, der fører til den nye side, vente med
  `wait: page=<kontekst>` — så hægter næste trin sig på, når siden er tegnet.
  Dybe sider (uden `route` i træet) kan **Vis mig** ikke navigere til; der skal
  klikket komme fra brugeren eller fra `action: click` på forrige trin.
- Åbner en handling en dialog eller menu, ligger den oven på masken og kan
  bruges; næste trin viser "Elementet vises, når siden er klar", indtil målet
  findes. Peger et trin med `field` på et punkt i en lukket menu (fx
  `{#fil-menu}` + `field: Gem`), åbner guiden selv menuen. Esc lukker en åben
  menu eller dialog først og afbryder guiden næste gang.
- Guiden overlever en fuld sideindlæsning (fx "Åbn fil", som genindlæser
  LCCbyg): den huskes i browserens sessionStorage og genoptages på samme trin.
- Guidens trin indekseres ikke til søgning — kun titlen. Skriv altså det
  vigtigste i titlen og indledningen.

### Opskrift: fra idé til kørende guide

Arbejdsgangen, der virker — gennemprøvet på guiderne i Guides-gruppen. Rækkefølgen
er ikke tilfældig: trin 2 er det, der oftest vælter en guide skrevet i blinde.

1. **Find sidens ankre først.** `grep` efter `HelpBubble Id=` i sidens `.razor` og
   dens børnekomponenter. Guiden kan KUN pege på ankre, der findes i koden —
   `buildhelp validate` er dommeren.
2. **Tjek at hvert trin har et mål, der kan rammes.** Dækker ét anker hele siden,
   skal trinnet bruge `field:` til at snævre ind. `field` finder (i den rækkefølge)
   `data-help-field`, `name`/`id`, en tabelcelle (`Kolonne` eller `Kolonne:3` —
   KUN i ankerets FØRSTE `<table>`), synlig tekst på label/knap/menupunkt, eller
   det n'te inputfelt. Ikoner uden tekst, gruppe-rækker i et MudDataGrid og alt i
   den anden tabel kan altså ikke rammes — der skal et anker til.
3. **Mangler der ankre, så sæt dem — også i genbrugte komponenter.** En komponent,
   der vises på flere sider (fx `ScenarioCollectionComponent` på Prisudviklinger,
   Miljøpåvirkning og Skyggepriser), må ikke eje et anker-id: id'et skal være unikt
   i DOM'en, og hjælpeteksten er forskellig fra side til side. Lad komponenten tage
   id'et som parameter — navngiv parameteren `…AnchorId`, så `buildhelp validate`
   kan se den — og lad SIDEN give det videre:

   ```razor
   @* Siden: *@
   <ScenarioCollectionComponent … GroupedAnchorId="kalkulationsrente" />

   @* Komponenten: kun paa det foerste kort, saa id'et er unikt *@
   <HelpBubble Id="@(firstCard ? GroupedAnchorId : "")" Title="@GroupedAnchorTitle">
   ```

   Er komponenten gentaget i en løkke, så sæt kun ankeret på det første element.
4. **Skriv guiden** som `guide-<slug>.md` efter formatet ovenfor, og føj den til
   Guides-gruppen i `helptree.json` (uden `route`).
5. **Dæk nye ankre med et emne** i sidens `{context}.md`, ellers melder validate
   dem UDÆKKET — og hjælpepanelet har intet at vise, når brugeren klikker badgen.
6. **Kør `buildhelp validate --content <…$\da> --source <…\LccUi>`.** Stien skal
   pege på SPROGMAPPEN (`44\da`), ikke på `44` — ellers meldes hvert eneste anker
   udækket. Validate tjekker guidens koder, ankre og sider.
7. **Kør `buildhelp index --content <…$\da>`.** Uden det står guiden ikke i
   panelets Guides-gruppe: listen kommer fra `catalog.json`, ikke fra træet.
8. **Byg appen igen.** `LccUi.csproj` indlejrer `.md`/`.json`/`.bin` som
   EmbeddedResource — en ændret guide slår først igennem efter en ny build, ikke
   ved en sidegenindlæsning.
9. **Kør guiden igennem i browseren** (LCCbygWeb i Development på :60265). Start
   den fra hjælpepanelet, klik **Næste** trin for trin og se, at ringen sidder om
   det rigtige element. Tjek ringens mål programmatisk, når skærmbilledet er i
   tvivl:

   ```js
   const b = document.querySelector('[class*=guide-ring]').getBoundingClientRect();
   document.elementFromPoint(b.x + b.width/2, b.y + b.height/2).closest('tr').textContent;
   ```

10. **Ret teksten efter det, ringen faktisk peger på.** Det er her guiden bliver
    god: peg på den række, der beviser pointen (fx spildevandets 2,10 %, ikke den
    generelle 0,00 %), og skriv de konkrete tal ind i trinnet.

Gode vaner: ét mål pr. trin; `wait: click` hvor brugeren selv skal gøre noget
(den lytter på HELE ankeret, så ethvert klik deri fører videre); ingen
`action: click` på knapper, der ændrer brugerens projekt, medmindre guiden har
`requires: new-project`; og husk, at kun titel og indledning kan søges frem.

### Forfatterværktøjet (kun debug)

Blyanten i hjælpevinduet har **Ny guide** / **Rediger guide**: en editor med
trinliste, koder og tekst pr. trin. **Optag** lytter på siden og opretter et
trin-skelet for hvert ankret element, du klikker på eller skriver i (anker,
felt, værdi, `wait`). **Afspil trin** / **Afspil guide** kører guiden på den
åbne side uden at bygge appen, **Gem** skriver `guide-<slug>.md` i docs-klonen
og føjer guiden til træets Guides-gruppe, og **Kopiér markdown** /
**Kopiér forfatter-prompt** lægger filen eller en færdig opgave til Claude Code
i udklipsholderen. Kør altid `buildhelp validate` og `buildhelp index` til
sidst.
