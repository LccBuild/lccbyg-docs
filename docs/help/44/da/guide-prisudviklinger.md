---
title: "Rente, prisudvikling og egne sæt"
type: guide
start: developmentsets
requires: project
description: Rentetrappen og prisudviklingen i ét sæt, hvordan du laver dit eget — og at det samme gælder alle forudsætningerne.
---

Forudsætningerne er beregningens fælles grundlag: hvad fremtidige kroner er
værd i dag, hvor hurtigt priserne stiger, hvor meget CO2 der udledes, og hvad
den koster. Guiden går et prisudviklingssæt igennem og viser, hvordan du laver
dine egne sæt. Det fungerer på samme måde for alle forudsætningerne.

## Velkommen til forudsætningerne
Kalkulationsrente og prisudvikling gælder ikke kun ét alternativ. De ligger
under **Forudsætninger** sammen med biblioteket, miljøpåvirkning, skyggepriser
og vedligehold.

## De fire sæt {#prisudviklingssaet}
placement: center

LCCbyg leverer fire færdige sæt. **Faldende realrente** er standarden for
offentlige bygherrer og for DGNB efter 2025-manualen; **Fast nominel rente**
regner med løbende priser. Hvert kort er ét sæt.

## Kalkulationsrenten {#kalkulationsrente}
wait: click

Renten tilbagediskonterer fremtidige omkostninger til nutidsværdi. Klik på
**Kalkulationsrente** for at folde rentetrappen ud.

## Rentetrappen {#kalkulationsrente}
field: Procent

Faldende realrente følger Finansministeriets rentetrappe: 3,5 % fra år 1,
2,5 % fra år 36 og 1,5 % fra år 71. Kolonnen **År** er det år, hvor værdien
tager over fra den foregående.

## Prisudviklingen {#prisudvikling}
Nedenunder står prisudviklingen for hver omkostningsgruppe: byggeri, forsyning
og drift. Øverst står **Prisudvikling generelt** — den er 0,00 % i dette sæt,
altså faste priser: 100 kr. i dag er også 100 kr. om ti år.

## Kun forskellen {#prisudvikling}
field: Procent:4

Tallene er udviklingen **ud over** den generelle prisudvikling. Spildevand står
til 2,10 %, fordi udgiften forventes at stige så meget mere end priserne
generelt. Stiger en omkostning 6 %, mens den generelle udvikling er 2 %,
skriver du altså 4 %.

## Lav dit eget sæt {#prisudvikling-handlinger}
De fire sæt er låste, så de betyder det samme fra projekt til projekt. Vil du
regne med egne værdier, så kopiér et sæt med kopi-knappen og ret kopien. Den
kan også slettes igen.

## Miljøpåvirkning {#miljoe-handlinger}
page: impactscenarios

Det samme gælder miljøpåvirkningens scenarier, dvs. fremskrivningen af
CO2-faktorerne. Kopiér et scenarie for at regne med dine egne faktorer.

## Skyggepriser {#skyggepris-handlinger}
page: shadowpricescenarios

Og skyggepriserne: kopiér fx **Fast skyggepris**, og sæt din egen pris pr. ton
CO2 i kopien.

## Vedligehold {#vedligehold-handlinger}
page: maintenanceprerequisites

Vedligeholdsplanens ejendomstyper har prisspænd pr. m². Også her laver
kopi-knappen et sæt, du selv kan prissætte.

## Sættet vælges pr. alternativ {#beregningsforudsaetninger}
page: alternatives
field: Rente og prisudvikling

På alternativkortet vælger du, hvilket sæt alternativet regner med: rente og
prisudvikling, miljøpåvirkning og skyggepris — og ejendomstypen under
vedligeholdsberegningen. Dine egne sæt står i listerne sammen med
standardsættene.

## Færdig
Ændrer du sæt eller værdier, regnes alle resultater om med det samme. To
alternativer kan altså regnes med hver sin forudsætning. Det er en af de
måder, alternativerne kan bruges på. Vil du vide mere om CO2-faktorerne, så
tag guiden **Miljøpåvirkning og CO2-faktorer**.
