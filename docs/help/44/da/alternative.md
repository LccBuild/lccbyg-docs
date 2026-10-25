---
title: "Alternativet"
---

Siden samler alt om ét alternativ i tre faner: **Grupper**, **Vedligeholdsplan**
og **Målsætninger** — grupperne er rygraden i beregningen. Hver gruppe samler de
rækker, der hører sammen (fx en bygningsdel), og gruppens Rækker-knap åbner
[rækkerne](alternative-group-rows.md), hvor du inddaterer. Vil du til et andet
alternativ, så klik på det i [sidemenuen](shared.md#hovedmenu), hvor projektets
alternativer står under **Alternativer**.

### Fanerne {#alternativ-faner}
Fanebladet øverst skifter mellem sidens tre dele — hver har sit eget afsnit
her i hjælpen: [Grupper](#grupper), [Vedligeholdsplan](#vedligeholdsplan) og
[Målsætninger](#bedoemmelse). Hjælpen følger med, når du skifter fane.
### Gruppekortene {#grupper}
Hvert kort er én gruppe: ikonet viser gruppens indhold og antal rækker, navnet
kan rettes direkte i feltet, og farven vælges med ikon-knappen. Nederst kan
gruppen slettes. Grupperne opdeler alternativet, så strukturen matcher dit
projekt — fx efter SfB eller efter opgavetype.

### Rækker-knappen {#raekker-knap}
Knappen viser gruppens antal rækker og åbner
[rækkelisten](alternative-group-rows.md), hvor du henter bygningsdele fra
biblioteket og skriver mængder og priser.

### Listevisning {#gruppe-listevisning}
Kontakten skifter mellem gruppekort og en liste. I listevisningen kan du
markere flere grupper og klippe, kopiere, indsætte eller slette dem i én
arbejdsgang via menuen i kolonnehovedet.

### Gruppelisten {#gruppe-liste}
I listevisningen står grupperne som rækker i en tabel. Fluebenet yderst til
venstre markerer en gruppe; markér flere for at kopiere, klippe eller slette dem
på én gang. Navnet fører ind i gruppen, og et højreklik på en gruppe åbner
menuen for netop den gruppe.

### Menuen for de markerede grupper {#gruppe-redigeringsmenu}
De tre prikker øverst i listen åbner menuen, der virker på alle markerede
grupper: Klip, Kopiér, Indsæt og Slet.

### Kopiér grupper {#gruppe-kopier}
Lægger de markerede grupper på LCCbygs udklipsholder med alle deres rækker.
Udklipsholderen bliver liggende, når du skifter alternativ, så grupperne kan
sættes ind i et andet alternativ.

### Indsæt grupper {#gruppe-indsaet}
Sætter grupperne fra udklipsholderen ind sidst i alternativet som kopier. Højreklik
på en gruppe for at sætte dem ind over eller under netop den. Fortryd (Ctrl+Z)
tager en hel indsættelse tilbage på én gang.

### Tilføj en gruppe {#tilfoej-gruppe}
Knappen opretter en ny, tom gruppe. Giv den et sigende navn — grupperne
strukturerer både inddateringen og resultaterne.

### Importér fra regneark {#import-regneark}
Knappen henter grupper og rækker ind fra en .xlsx-fil, typisk en, der er
eksporteret fra LCCbyg og rettet. Menuen viser de senest brugte importfiler, og
mappe-ikonet vælger en ny. Importen tilføjer regnearkets grupper; den retter
ikke i dem, alternativet har i forvejen.

### Eksportér til regneark {#eksport-regneark}
Knappen gemmer alternativets grupper og rækker som regneark med ét ark pr.
gruppe, så du kan arbejde med tallene udenfor og importere dem igen.

### Vedligeholdsplan {#vedligeholdsplan}
Vedligeholdsplanen er et alternativt system til at angive vedligeholdsudgifter:
i stedet for at prissætte hver række besvarer du en række spørgsmål om centrale
forhold ved ejendommen, og udgifterne beregnes ud fra et typisk prisspænd for
den valgte ejendomstype. Planen skifter beregningsmetode: mens den er slået
til, regnes rækkernes vedligeholdskort ikke med, og slås den fra, er de tilbage
som før. Tænd systemet med kontakten **Brug vedligeholdsplan**,
vælg ejendomstype, og besvar spørgsmålene — diagrammet viser, hvor langt du er.

### Spørgsmålsgrupperne {#vedligehold-grupper}
Hver chip er én gruppe spørgsmål om ejendommen — fx tag, facader eller
installationer. Farven er gruppens niveau fra grøn (lavt behov for
vedligehold) til rød (højt), og stregen under viser, hvor mange spørgsmål der
er besvaret; ubesvarede grupper tæller som højt niveau. Klik på en chip for at
se dens spørgsmål og svare, og sortér chips med knapperne over dem.

### Rosen {#vedligehold-rose}
Rosen samler vurderingen: hvert felt er en spørgsmålsgruppe, feltets bredde er
gruppens vægt, og længden og farven er dens niveau. Midten viser det samlede
niveau. Klik på et felt for at gå til gruppens spørgsmål.

### Nøgletallene {#vedligehold-noegletal}
Bundlinjen viser ejendomstypens prisspænd pr. m² — minimum, middel og høj —
og den pris, vurderingen lander på, samt det årlige vedligehold og
vedligeholdets nutidsværdi. Jo lavere niveau, jo tættere på minimum.
### Bedømmelse af målsætninger {#bedoemmelse}
Her bedømmer du, hvor godt alternativet opfylder de målsætninger, der er
valgt under [Målsætninger](criteria.md): giv stjerner for hver målsætning —
skalaen står under stjernerne — og skriv begrundelsen i feltet ved siden af.
Bedømmelserne sammenlignes på tværs af alternativer i visningen Målsætninger.

### Rediger projektets målsætninger {#rediger-maalsaetninger}
Knappen glider [Målsætninger](criteria.md) op nedefra, så du kan tilføje
eller vægte målsætninger uden at forlade bedømmelsen.

### Rediger alternativet {#alternativ-detaljer}
<!-- anchors: alternativedetails -->
Hus-knappen i værktøjslinjen åbner alternativkortet i et vindue, så du kan
rette navn, beskrivelse og beregningsforudsætninger uden at forlade den side,
du står på. Det er nøjagtig det samme kort, som ligger på
[Alternativer](alternatives.md) — retter du her, er det rettet der.

### Rediger gruppen {#gruppe-detaljer}
<!-- anchors: groupdetails -->
Gruppe-knappen i værktøjslinjen åbner den åbne gruppes felter i et vindue:
navn og farve øverst, og derunder gruppens egenskaber, statistik og
beregningsfiltre foldet sammen hver for sig. Ændringerne slår igennem med det
samme i gruppelisten og i beregningen.
