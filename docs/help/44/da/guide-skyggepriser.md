---
title: "Skyggepriser — CO2 i kroner"
type: guide
start: shadowpricescenarios
requires: project
description: De fem skyggeprisscenarier, hvad de antager, og hvordan du laver dine egne priser.
---

En skyggepris sætter kroner på udledningen af CO2, så klimapåvirkningen kan
vejes mod økonomien i samme regnestykke. Guiden gennemgår de fem scenarier,
LCCbyg leverer, og viser, hvor du laver dine egne priser og vælger dem.

## Hvad er en skyggepris?
Hvert scenarie giver en pris pr. ton CO2-ækvivalent hen over
beregningsperioden. Prisen ganges med alternativets udledning, og resultatet
indgår i totaløkonomien som posten **Skyggepris**. Kolonnen **År** er det år,
hvor en pris tager over fra den foregående.

## Ingen skyggepris {#skyggeprisscenarier}
field: Ingen skyggepris

CO2 koster 0 kr. Brug den som reference — eller når opgaven slet ikke skal
have klimaet med i kroner. Det er standardvalget i et nyt projekt.

## Fast skyggepris {#skyggeprisscenarier}
field: Fast skyggepris

Samme pris i hele perioden: 1.500 kr. pr. ton. Enkel at forklare og god, når
bygherren har en fast intern CO2-pris — så kopierer du sættet og retter
prisen.

## Finansministeriets skyggepriser {#skyggeprisscenarier}
field: Finansministeriets skyggepriser juni 2026

Følger Finansministeriets vejledning: 728 kr. pr. ton i år 0, stigende år for
år til omkring 38.000 kr. i år 75. Vejledningens faktorpriser er ganget med
nettoafgiftsfaktoren 1,28, og alle priser er i 2026-kroner.

## Klimarådets skyggepriser {#skyggeprisscenarier}
field: Klimarådets skyggepriser juni 2026

Samme startpris, men en stejlere stigning: knap 2.000 kr. allerede i år 4 og
omkring 85.000 kr. i år 75. Finansministeriet anbefaler Klimarådets priser til
følsomhedsanalyser — regn et alternativ med begge, og se hvor meget det
betyder.

## Trinvise skyggepriser {#skyggeprisscenarier}
field: Trinvise skyggepriser

Prisen indfases i spring: 1.000 kr. fra start, så 1.500, 2.500, 3.500 og
4.500 kr., og 5.500 kr. fra år 10 — som en CO2-politik, der strammes gradvist.

## Dine egne priser {#skyggepris-handlinger}
De fem scenarier er låste. Kopiér det, der ligger tættest på det, du vil
regne med, og ret priserne i kopien — den kan også omdøbes og slettes igen.

## Scenariet vælges pr. alternativ {#beregningsforudsaetninger}
page: alternatives
field: Skyggeprisscenarie

På alternativkortet vælger du, hvilket scenarie alternativet regner med. To
alternativer med de samme rækker, men hver sit scenarie, viser, hvor følsomt
resultatet er for prisen på CO2.

## Færdig
Skyggeprisen går igen i resultat-tickeren, i visningerne og i
Sammenligninger-dashboardet, hvor alternativerne rangeres efter mindste
skyggepris.
