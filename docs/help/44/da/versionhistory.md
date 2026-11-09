---
layout: lccbyghelp40
title: "Versionshistorik LCCbyg 4"
date: "2024-03-04"
search: false
---

# LCCbyg 4 - Versionshistorik

## [4.4.10]

#### Fixed
- [Faldende realrente] Når kalkulationsrenten skifter undervejs i beregningsperioden (fx 3,5 % i år 1-35, 2,5 % i år 36-70 og 1,5 % derefter), diskonteres hvert år nu med de renter, der har gældt frem til det år, som i Finansministeriets vejledning i samfundsøkonomiske konsekvensvurderinger (juni 2023). Tidligere versioner brugte det enkelte års rente på hele perioden, så nutidsværdier og annuiteter blev for store for alle år efter det første renteskift. Projekter med en beregningsperiode over 35 år viser derfor lavere nutidsværdier end i 4.0.52; fx falder standardprojekteksemplet med ca. 2,4 mio. kr. Samme rettelse gælder prisudviklinger med flere satser.

## [4.0.43]

#### Changed
- [Miljøudvikling] Rettet værdier så de stemmer overens med BR18 tabel 8

#### Fixed
- [Bedømmelse af målsætning] LCCbyg kunne gå ned når man bedømte en målsætning

## [4.0.42]

#### Added
- [Versionshistorik] Dette dokument
- [Sprogskifter] Der kan nu skiftes sprog. Dette skifter også tusindtalsseparator og decimalseparator. Rækkenavne mv. følger stadig projektfilens sprog.
- [Søgefunktion i projektets rækker] Funktionaliteten findes nu i et søgefelt der filtrerer rækkevisningen.

#### Changed
- [Oversættelser] Oversættelser af tabelnavne hentes på en ny måde, så de virker mere konsistent.


#### Removed
- [Fortryd-knap på quickview-dialog] Knappen er fjernet, fordi funktionen ikke ligger der, men i fortryd- og gendan-knapperne.

#### Fixed
- [Opdatering af resultattabeller] Tabellerne blev ikke altid genereret når de blev valgt, og nogle gange blev den forkerte type vist, når man valgte ny
- [Opdatering af resultat] Når quickview blev brugt til at ændre fx prisudvikling, blev resultatvisningen ikke opdateret (bl.a. på siden med grupper og rækker.
- [Opdatering af oversættelser] Flere manglende oversættelser tilføjet, stavefejl rettet.
- [Opdatering af beregning ved regnearksimport] Resultater blev ikke automatisk opdateret, når der blev importeret fra regneark.
 
 
 
