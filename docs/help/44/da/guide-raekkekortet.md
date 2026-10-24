---
title: "Én række gennem hele livet"
type: guide
start: alternatives
requires: new-project
project: lite_eksempel
description: Følg et tegltag fra anskaffelse over vedligehold til udskiftning og restværdi — kort for kort.
---

En række er mere end en pris: den har en levetid, vedligehold, udskiftning og
en værdi, når den tages ud af brug. Guiden følger et tegltag i eksemplet "Tag-
og vinduesudskiftning" gennem hele livet.

## Velkommen
Tegltaget ligger i alternativet **Forskudt renovering - trævinduer**, i
gruppen **Tagrenovering - om 10 år**.

## Til alternativet {#hovedmenu}
field: Forskudt renovering - trævinduer
action: click
wait: page=alternative

Klik på **Forskudt renovering - trævinduer** i sidemenuen.

## Til gruppen {#hovedmenu}
field: Tagrenovering - om 10 år
action: click
wait: page=alternative-group-rows

Klik på gruppen **Tagrenovering - om 10 år**.

## Åbn tegltaget {#raekkegrid}
field: Navn
action: click
wait: click

Klik på **Tegltag** for at åbne rækkens detaljer.

## Generelt {#raekkekort}
field: Generelt

Øverst står det, der gælder hele rækken: hvilken prisudvikling og
miljøpåvirkning den regnes med, og dens klassifikation, fx SfB-koden.

## Anskaffelse {#raekkekort}
field: Anskaffelse

Taget koster 933.750 kr. og holder i 60 år. **Start i år** er 10 — arvet fra
gruppen — så anskaffelsen falder i år 10, ikke i dag.

## Løbende vedligehold {#raekkekort}
field: Vedligehold

Hvert år fra år 11 bruges 0,10 % af genanskaffelsesprisen, 934 kr. Prisen kan
angives som procent eller som beløb pr. gang.

## Større vedligehold {#raekkekort}
field: Vedligehold 2

En række kan have flere vedligeholdskort. Her kommer hvert 10. år fra år 20 et
større eftersyn til 9 %, 84.038 kr. pr. gang.

## Udskiftning {#raekkekort}
field: Udskiftning

Efter levetiden på 60 år skal taget skiftes — i år 70, til 125 % af
genanskaffelsesprisen. Det ligger efter beregningsperiodens slut i år 50 og
kommer derfor ikke med. I stedet har taget en restværdi ved periodens slut,
fordi det stadig har levetid tilbage.

## Genanvendelse {#raekkekort}
field: Genanvendelse

Hvad taget er værd, når det tages ud af brug: en positiv værdi er en indtægt
ved genanvendelse, en negativ en udgift til bortskaffelse. Her er feltet ikke
udfyldt.

## Rækkens resultater {#raekke-noegletal}
placement: top

Bundlinjen viser rækkens bidrag til beregningen og følger med, hvis du retter
et tal. Prøv fx et andet interval på vedligeholdet — og tryk **Fortryd**
bagefter, hvis du ikke vil beholde det.

## Færdig
Anskaffelse, vedligehold, udskiftning og genanvendelse beskriver tilsammen
rækkens hele liv. Renhold, forsyning, forvaltning og indtægter bruger de samme
felter: pris, start, slut og interval.
