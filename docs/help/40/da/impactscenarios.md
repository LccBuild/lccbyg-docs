---
layout: lccbyghelp40
title: "Miljøpåvirkning"
date: "2024-01-01"
---

DGNB Byområder beregner foruden levetidsomkostninger også på CO2\-udledninger forbundet med et byområde. Miljøpåvirkningerne (i form af CO2\-udledninger) beregnes via [Miljøpåvirkningsscenarie](#miljø) og [nøgletal](#byrum) udviklet til certificering af byområder fra DGNB2020-manualen.

### Miljøpåvirkningsscenarier(#miljø)

I denne skabelon er det muligt at vælge miljøpåvirkningsscenarier på samme vis som for rente- og prisudvikling. I skabelonen er det muligt at vælge mellem to miljøpåvirkningsscenarier:

- Ingen udvikling (det scenarie der anvendes i DGNB).
- Fremskrivning 2020 (denne fremskrivning er baseret på politiske mål om at øge andelen af vedvarende energi i dansk energiforsyning i perioden 2020-2050). Fremskrivningen gælder for el og fjernvarme. Kilde: Trafik-, Bygge, og Boligstyrelsen: Nye emissionsfaktorer for el og fjernvarme 2020.

På samme vis som det er muligt at opbygge sit eget sæt af rente- og prisudvikling i LCCbyg, er det her også muligt at opbygge sit eget miljøpåvirkningsscenarie. Dette gøres ved at oprette en kopi af et af de to scenarier og ændre i værdierne herfor til det ønskede scenarie. Der skal dog gøres opmærksom på, at i DGNB-regi opereres der endnu ikke med en udvikling for miljøpåvirkningsscenarier.

### Miljøpåvirkninger(#byrum)

Skabelonen 'DGNB-byrum' indeholder nøgletal for arealer, forsyning og renhold. Nøgletallene er opbygget med udgangspunkt i strukturen i DGNB Byområde Manualen 2020. Kontoplanen kommer med levetider, priser på forsyning og renhold samt CO2\-miljøpåvirkning (GWP) referenceværdier.

Beregninger med værktøjet giver et overslag over de forventede omkostninger og CO2\-miljøpåvirkning (GWP) til gennemførelse af en byudviklingsopgave og den efterfølgende drift heraf over en 50-årig periode samt eventuelle udskiftninger undervejs. Beregningerne bygger på generiske nøgletal, som ikke nødvendigvis er retvisende for den konkrete opgave. Priser er baseret på vejledende overslag fra Molio Prisdata. Forventede levetider er bearbejdet fra [levetidstabellen](https://lccbyg.dk/levetidstabel2021/) i rapporten BUILD2021:32.

Miljøpåvirkningerne stammer fra BMVBS 2012, her er A1-3 Produktfasen opgivet. Denne værdi er på baggrund af en erfaringsbaseret fordelingsnøgle (ses herunder) anvendt til at fastlægge de resterende moduler under areal-rækkerne, nemlig B2 Vedligehold og B4 Udskiftning, som anvendes i denne skabelon. Den erfaringsbaserede fordelingsnøgle er bestemt ud fra SBi 2020:04.

- A1-3 Produkt: Svarende til 50 % af den samlede udledning.
- B2 Vedligeholdelse: Svarende til 10 % af A1-3 Produktfasen.
- B4 Udskiftning: Svarende til A1-3 adderet med C3/C4.
- B6 Forsyning: Svarende til 25 % af A1-3 Produktfasen – dette indtaster man dog separat på samme måde som Renhold.
- C3/C4 Bortskaffelse: Svarende til 15 % af A1-3 Produktfasen (Modulerne vedrørende bortskaffelse er ikke en del af DGNB Byområde).

Usikkerheden på resultaterne afhænger af de anvendte beregningsforudsætninger og data til beregningerne. Ændringer af disse kan have stor betydning for resultaterne. Ved mere komplekse byggeopgaver eller behov for mere retvisende beregninger bør en rådgiver konsulteres og følsomhedsanalyser gennemføres.
