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
