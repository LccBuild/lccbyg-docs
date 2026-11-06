---
title: "Rækkekortet"
---

Rækkekortet viser én række med alle detaljer: omkostningerne fordelt på
anskaffelse, drift, vedligehold og bortskaffelse — og rækkens CO₂-moduler.
Her retter du tallene, så rækken passer til dit projekt, og ser rækkens
nøgletal opdatere sig i bunden.

### Rækkedetaljer {#raekkekort}
Klikker du på en række i rækkelisten, åbner den i dialogen Rækkedetaljer med
de samme kort: Generelt øverst og et kort pr. omkostning nedenunder. OK
gemmer ændringerne, Fortryd ruller dem tilbage.

### Fortryd og OK {#raekke-afslut}
Knapperne øverst i dialogen lukker den. **OK** beholder det, du har rettet, som
ét fortryd-trin; **Fortryd** ruller alle rettelser i dialogen tilbage. Enter i
et felt svarer til OK, Escape til Fortryd.

### Skift række {#raekke-vaelger}
Vælgeren øverst hopper direkte til en anden række i gruppen, uden at du skal
tilbage til rækkelisten.

### Rækkens indstillinger {#raekke-indstillinger}
<!-- anchors: rowsettings -->
Kortet "Generelt" holder det, der gælder hele rækken, og ikke én enkelt
omkostning: rækkens stamfelter og de to valg for prisudvikling og
miljøpåvirkning. Prisudviklingen bestemmer, hvordan rækkens priser
fremskrives hen over beregningsperioden, og miljøpåvirkningen gør det samme
for rækkens CO₂. Vælgerne viser de sæt, projektet har liggende under
Forudsætninger — vælger du et andet, slår det igennem på alle kortene
nedenfor.

### Nulstil CO₂-moduler {#nulstil-moduler}
Knappen opretter et nyt sæt tomme CO₂-moduler (LCA-faser), som du selv kan
udfylde. Brug den, når du vil inddatere egne klimadata i stedet for
bibliotekets.

### Indsæt CO₂-moduler {#indsaet-moduler}
Knappen åbner CO₂-biblioteket, hvor du finder moduler, der passer til rækkens
enhed. Modulerne erstatter dem, rækken allerede har.

### Omkostningskortene {#omkostningskort}
Hvert kort dækker én omkostningstype — fx anskaffelse, renhold, vedligehold,
genopretning og bortskaffelse. På kortet skriver du mængde, enhedspris og
interval/levetid; kortets sum indgår direkte i beregningen. Afsnittene
herunder forklarer det enkelte kort; hjælpeknappen på kortet fører direkte
hertil.

### Anskaffelse {#omkostning-acquire}
<!-- anchors: acquire -->
Engangsudgiften ved at anskaffe rækken. Enhedsprisen ganges med rækkens
mængde og giver anskaffelsesprisen. Levetiden siger, hvor mange år rækken
holder, og bruges af Udskiftning nedenfor — sæt den, også når anskaffelsen
er nul, hvis rækken skal skiftes undervejs i beregningsperioden.

### Renhold {#omkostning-cleaning}
<!-- anchors: cleaning -->
Den løbende rengøring. Enhedsprisen er prisen for én gang, og frekvensen
siger, hvor mange gange om året det sker; sammen giver de årets udgift.
Første gang og Stop efter afgrænser, i hvilke år udgiften tæller med.

### Vedligehold {#omkostning-maintain}
<!-- anchors: maintain -->
Det tilbagevendende vedligehold. Prisen per gang kan enten skrives som beløb
eller som procent af genanskaffelsesprisen, og intervallet siger, hvor mange
år der går mellem gangene. Start i år og Udgår i år afgrænser perioden. Har
alternativet vedligeholdsplanen slået til, beregnes vedligeholdet efter planen
i stedet: kortet står nedtonet, og rækkens beløb indgår ikke i totalerne, før
planen slås fra igen.

### Udskiftning {#omkostning-restore}
<!-- anchors: restore -->
Genopretning eller udskiftning med et fast interval, typisk når rækkens
levetid er opbrugt. Prisen per gang kan som ved vedligehold angives enten som
beløb eller som procent af genanskaffelsesprisen. Første gang og Stop efter
afgrænser perioden.

### Genanvendelse {#omkostning-endoflife}
<!-- anchors: endoflife -->
Hvad rækken er værd, når den tages ud af brug: en engangsindtægt ved
genanvendelse — eller en udgift til bortskaffelse, hvis du skriver et
negativt beløb. Året afgør, hvornår posten falder.

### Forsyning {#omkostning-supply}
<!-- anchors: supply -->
Løbende forbrug: energi, vand og lignende. Enhedsprisen ganget med rækkens
mængde giver årets udgift, og Første gang og Stop efter afgrænser, hvilke år
den tæller med.

### Forvaltning {#omkostning-manage}
<!-- anchors: manage -->
Løbende udgifter til administration, forsikring, afgifter og anden
forvaltning. Regnes som de øvrige løbende poster: enhedspris gange mængde,
afgrænset af Første gang og Stop efter.

### Løbende indtægt {#omkostning-income}
<!-- anchors: income -->
En tilbagevendende indtægt, fx leje. Den regnes som de øvrige løbende poster,
blot med modsat fortegn, og trækker derfor ned i rækkens nutidsværdi.

### Engangsudgift {#omkostning-nonrecurringcost}
<!-- anchors: nonrecurringcost -->
En udgift, der falder i ét bestemt år og ikke gentager sig. Året skrives i
Start i år. Brug kortet til poster, der hverken hører til anskaffelsen eller
til det løbende.

### Engangsindtægt {#omkostning-nonrecurringincome}
<!-- anchors: nonrecurringincome -->
Modstykket til engangsudgiften: en indtægt i ét bestemt år, som ikke gentager
sig.

### Låste CO₂-moduler {#laaste-co2-moduler}
<!-- anchors: co2modulesarelockedbecausetheyarepartofaset -->
Når CO₂-værdierne kommer fra et samlet LCA-fasesæt, er modulerne låst, så der
regnes konsistent. Vil du arbejde med egne værdier, så brug Nulstil
CO₂-moduler og udfyld selv.

### Rækkens resultater {#raekke-noegletal}
<!-- anchors: resultat-ticker -->
Bundlinjen viser rækkens aktuelle bidrag til beregningen og opdateres, mens
du retter tallene.
