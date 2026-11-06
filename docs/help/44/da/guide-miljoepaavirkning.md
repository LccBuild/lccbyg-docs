---
title: "Miljøpåvirkning og CO₂-faktorer"
type: guide
start: impactscenarios
requires: project
description: Scenarierne bag CO₂-beregningen, og hvordan emissionerne udvikler sig over tid.
---

Ved siden af kronerne regner LCCbyg på CO₂. Miljøpåvirkningsscenariet bestemmer,
hvordan udledningen udvikler sig i beregningsperioden. Guiden går de to
leverede scenarier igennem.

## Velkommen til miljøpåvirkningerne
Et scenarie siger ikke, hvor meget en bygningsdel udleder — det tal kommer fra
bibliotekets rækker. Scenariet siger, hvordan udledningen ændrer sig, år for år.

## De to scenarier {#miljoescenarier}
placement: center

**Ingen udvikling** bruges ved DGNB-certificering: udledningen antages at være
den samme i hele perioden. **Fremskrivning 2025** følger de politiske mål om
mere vedvarende energi i den danske forsyning.

## Faktorerne {#miljoe-faktorer}
Kortet **Ingen udvikling** har én linje pr. type: generelt, energi,
elproduktion og fjernvarme. Kolonnen **Enhed** siger *Faktor* — tallet ganges
på rækkens egen udledning.

## Faktor 1 betyder uændret {#miljoe-faktorer}
field: GWP

Alle fire står til 1,0000. Udledningen i år 50 regnes altså med præcis samme
tal som i år 1 — det er dét, DGNB forudsætter.

## Fremskrivningen {#miljoe-fremskrivning}
field: Miljøpåvirkning fra elproduktion
action: click
wait: click

Kortet **Fremskrivning 2025** har i stedet en linje pr. år for el, fjernvarme
og ledningsgas. Klik på pilen ved **Miljøpåvirkning fra elproduktion** for at folde
årene ud.

## Udledning pr. kWh {#miljoe-fremskrivning}
field: GWP

Her er tallet ikke en faktor, men den faktiske udledning: el falder fra
0,0801 kg CO₂-ækv pr. kWh i 2025 til 0,0248 i 2050, efterhånden som strømmen
bliver grønnere. Kolonnen **År** er det år, værdien gælder fra.

## Lav dit eget scenarie {#miljoe-handlinger}
De to scenarier er låste. Vil du regne med dine egne emissionsfaktorer, så
kopiér et scenarie og ret kopien — men vær opmærksom på, at DGNB endnu ikke
regner med en udvikling i miljøpåvirkningerne.

## Scenariet vælges pr. alternativ {#nav-alternativer}
Hvert alternativ peger på ét scenarie, som du vælger i feltet
**Miljøpåvirkningsscenarie** på alternativkortet — ved siden af rente og
prisudvikling.

## Færdig
CO₂-resultaterne finder du i visningerne og på dashboardet sammen med
omkostningerne. Selve nøgletallene (GWP pr. modul) står på rækkerne i
biblioteket.
