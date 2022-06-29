---
title: "Rækketyper og posteringer"
date: "2020-06-16"
coverImage: "34_indtaegt.jpg"
---

Der findes otte forskellige typer af rækker, der kan inddateres i LCCbyg. Disse er nærmere beskrevet i nedenstående afsnit. Den inddaterede rækketype har direkte indflydelse på hvordan det inddaterede medtages i den totaløkonomiske beregning, fordi rækketyperne afspejler posteringstypen for de respektive rækker.

### Rækketyper

LCCbyg benytter rækketyper til posteringer. Der findes i alt 8 forskellige rækketyper. Hver af disse indeholder forskellige posteringstyper, som påvirker de totaløkonomiske beregninger.  Tabellen nedenfor indeholder beskrivelser af de 8 forskellige rækketyper, der indgår i LCCbyg. Yderligere viser kolonnen 'Typeikon' de respektive symboler for de forskellige rækketyper. Disse fremkommer både blandt nøgletal og i inddateringen, således du let kan se hvilken rækketyper og derved posteringstype der er tale om. I det efterfølgende beskrives de typiske [rækkedetaljer](#rowdetails) og posteringstyper for de forskellige rækketyper.

| Typeikon | Rækketype | Beskrivelse |
| --- | --- | --- |
| ![](images/Pasted-8.png) | Anskaffelse | Benyttes til anskaffelse af materiel til byggeprojektet, som ikke er bygningsdele. Fx. posteres grundkøb som en anskaffelse. |
| ![](images/Pasted-9.png) | Engangsudgift | Benyttes til postering af engangsudgifter. Dette kan fx. være honorarer til arkitekter og ingenører eller udgifter til byggeplads. |
| ![](images/Pasted-11.png) | Løbende udgift | Benyttes til postering af løbende udgifter. Dette kan eksempelvis være løbende administrationsudgifter, ejendomskat, dækningsafgifter eller forsikringer. |
| ![](images/Pasted-10.png) | Bygningsdel | Benyttes til anskaffelse af bygningsdele og bygningstyper. Det vil sige, at denne rækketype benyttes til byggematerialer. |
| ![](images/Pasted-12.png) | Forsyningsudgift | Forsyningsudgifter dækker over de løbende udgifter til forsyning af dit byggeprojekt, herunder varme, el og vandforbrug. |
| ![](images/Pasted-13.png) | Renholdsudgift | Renholdsudgifter dækker over de løbende udgifter til renhold af dit byggeri. Det kan fx. være vinduespudsning, gulvvask eller snerydning. |
| ![](images/Pasted-14.png) | Løbende indtægt | Løbende indtægter dækker over de løbende indtægter dit byggeri har. Det kan fx. være solcellestrøm, vindmøllestrøm eller solvarmeanlæg. |
| ![](images/Pasted-15.png) | Engangsindtægt | Engangsindtægter dækker over individuelle indtægter der falder i løbet af beregningsperioden. Dette kan fx. være scrap-værdi for salg af bygningsdele der ikke længere benyttes. |

Alt efter hvilken rækketype, der er inddateret, fremkommer forskellige rækkedetaljer og posteringstyper. Figur 1 viser rækkedetaljer for samtlige rækketyper. Der findes 9 forskellige posteringstyper; Anskaffelse, Engangsudgift, Vedligehold, Udskiftning, Forvaltning, Forsyning, Renhold, Løbende indtægt og Engangsindtægt.

[![](../images/34_postering_04-scaled.jpg)](http://lccbyg.dk/help/36/wp-content/uploads/sites/12/2022/01/34_postering_04-scaled.jpg)Figur 1: Eksempel på rækkedetaljer og nogle af de typiske kosttyper.

### Posteringer

Alternativets posteringer opsummeres i bunden af LCCbyg. Her ses nutidsværdien for de forskellige posteringstyper sammen med restværdien og den samlede nutidsværdi. Under ['Rapport'](https://lccbyg.dk/help/34/docs/interface/reports/) kan hovedposter og nutidsværdier sammenlignes på tværs af alternativer.

[![](../images/34_posteringer_resultat-scaled.jpg)](http://lccbyg.dk/help/36/wp-content/uploads/sites/12/2022/01/34_posteringer_resultat-scaled.jpg)Figur 2: Alternativets samlede posteringer og nutidsværdi kan ses i bunden af LCCbyg.

Fælles for alle posteringstyper er at der skal angives mængder, enheder og enhedspriser. Nogle posteringstyper, som fx. renhold, kommer med en prædefineret enhedspris.

#### Anskaffelse

Både 'Anskaffelse/grundkøb', bygningsdele og bygningstyper posteres under anskaffelse i LCCbyg. Det vil sige, at anskaffelsesomkostningerne i inddateringen summeres på tværs af rækketyper og posteres under 'Anskaffelse'.

Under 'Inddatering' indtastes anskaffelsesomkostningerne for hver af de omkostningstyper, der er valgt. Bemærk, at anskaffelsesomkostningerne falder i det år, som gruppen medregnes fra. Dette er som regel år 0, medmindre du har tilpasset denne værdi. Du kan også se, hvornår omkostningen forfalder i feltet 'startår'. Du kan inddatere eller tilpasse levetiden for din anskaffelse, hvis du ønsker.

#### Engangsudgifter

Engangsudgifter konteres i det år, der er angivet i 'startår'. Typisk vil engangsudgifter dække over omkostninger til byggeplads, honorarer til arkitekt, ingeniør o. lign. eller bygherreomkostninger.

#### Vedligehold

De inddaterede nøgletal kommer med en prædefineret vedligeholdelsesprocent, som ikke kan ændres. Denne angiver hvor mange procent af anskaffelsesværdien, der årligt skal bruges på løbende vedligehold af bygningsdelen/typen. Hvis du ønsker at afsætte et større beløb per vedligeholdsgang, kan du tilpasse denne under 'Kr./gang' ved at overskrive værdien, der står i feltet.

'Interval (år)' angiver, hvornår vedligeholdet begynder. Dette afspejles også i 'startår', imens 'slutår' angiver, hvornår udgiften frafalder. Slutåret vil som hovedregel svare til beregningsperioden.

#### Udskiftning

LCCbyg hensætter 125 % af anskaffelsesomkostning til udskiftning af bygningsdelen/typen ved endt levetid. Udskiftningsprocenten kan ikke ændres, men hvis du ønsker at afsætte et større eller lavere beløb til udskiftning af bygningsdelen, kan dette gøres under ’Kr./gang’, hvorved udskiftningsprocenten overskrives.

LCCbyg beregner udskiftning med udgangspunkt i 'Levetid (år)' og 'Startår' året for beregningsperioden. Hvis 'Startår' af udskiftning er større end udløb af beregningsperioden, vil programmet ikke medtage udskiftningen.

#### Forvaltning

Forvaltning omfatter omkostninger til skatter, forsikring osv. Under denne kosttype skal mængden, enhedsprisen samt start- og slutår inddateres.

Forvaltningsomkostningerne falder som en løbende udgift, der medregnes årligt fra startår til slutår.

#### Forsyning

Forsyning omfatter omkostninger til vand, varme, elektricitet og anden forsyning i beregningen baseret på forslag til enhedspriser i applikationen. Enhedspriserne kan overskrives med egne værdier fx fra det lokale forsyningsselskab. Forslagene til standardværdierne kan om nødvendig overskrives under inddatering.

Under 'Inddatering' skal du alene indtaste de samlede mængder fx energibehov opgjort i kWh per år. Disse mængder vil normalt fremgå af de obligatoriske energirammeberegninger eller energimærker. Forsyningsudgifterne er en løbende udgift, der medregnes årligt fra startår til slutår.

#### Renhold

Renhold omfatter omkostninger til forskellige typer af renhold i beregningen baseret på standardværdier for frekvens (per år) og enhedspriser.

Enhedsprisen dækker alle omkostninger i forbindelse med renhold inkl. rengøringspersonale og overheadomkostninger. Enhedspriserne opgøres i kr./m2 eller kr./stk.

Frekvens svarer til hvor mange gange årligt rengøringen skal udføres udføres (opgjort i antal/år).  Tabellen viser, hvordan de typiske frekvenser anvendt i LCCbyg forstås. 

| Frekvens | Beskrivelse |
| --- | --- |
| 1 | Én gang årligt |
| 2 | To gange årligt |
| 26 | Én gang hver anden uge |
| 100 | To gange om ugen, ekskl. helligdage |
| 256 | 5 gange om ugen, ekskl. helligdage. Dvs. renhold i hverdagene. |

Under 'Inddatering' skal du alene indtaste mængder. Du kan dog om nødvendig overskrive standardværdierne under 'Inddatering'. Udgifter til renhold er en løbende udgift, der medregnes årligt fra startår til slutår.

#### Løbende indtægt

Forsyningsindtægter posteres som løbende indtægter i LCCbyg. Forsyningsindtægter omfatter indtægter fra lokal produktion af elektricitet på ejendommen typisk i form af elektricitet fremstillet ved hjælp af solceller på tag og facade eller ved hjælp af en lille husstandsvindmølle på taget.

Under 'Inddatering' skal du alene indtaste mængder. Du kan dog om nødvendig overskrive standardværdierne under 'Inddatering'. Forsyningsindtægt er en løbende indtægt, der medregnes årligt fra startår til slutår.

Bemærk, at forsyningsindtægter skal medregnes positivt i beregningen, hvorfor enhedsprisen har positivt fortegn. Ændres enhedsprisen til negativ vil forsyningsindtægten i stedet blive en løbende udgift posteret i løbende indtægt.

#### Engangsindtægt

Engangsindtægter kan eksempelvis forekomme, hvis du modtager et éngangsbeløb fx i form af en støttebevilling fra en fond. Engangsindtægter kan også omfatte salg af bygningsdele, fx salg af vinduer i år 50 som led i en cirkulær tankegang. Engangsindtægter kan med andre ord bruges til at inddatere scrapværdier. Foruden mængde og enhedspris skal du ændre 'startår' til det år hvor indtægten falder.
