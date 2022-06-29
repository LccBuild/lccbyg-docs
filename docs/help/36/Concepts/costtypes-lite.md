---
title: "Rækketyper og posteringer - Den enkle skabelon"
date: "2022-01-12"
---

LCCbyg benytter rækketyper til posteringer. Der findes i alt 6 forskellige rækketyper i den enkle skabelon, imens det øvrige LCCbyg benytter 8 rækketyper. Hver af disse indeholder forskellige posteringstyper, som påvirker de totaløkonomiske beregninger.

### Rækketyper

Tabellen nedenfor indeholder beskrivelser af de 6 forskellige rækketyper, der indgår i den enkle skabelon i LCCbyg. Yderligere viser kolonnen 'Typeikon' de respektive symboler for de forskellige rækketyper. Disse fremkommer både blandt nøgletal og i inddateringen, således at du let kan se hvilken rækketyper og derved posteringstype, der er tale om. I det efterfølgende beskrives de typiske rækkedetaljer og posteringstyper for de forskellige rækketyper.

| Typeikon | Rækketype | Beskrivelse |
| --- | --- | --- |
| ![](images/Pasted-9.png) | Engangsudgift | Benyttes til postering af engangsudgifter. Dette kan fx. være honorarer til arkitekter og ingenører eller udgifter til byggeplads. |
| ![](images/Pasted-11.png) | Løbende udgift | Benyttes til postering af løbende udgifter. Dette kan eksempelvis være løbende administrationsudgifter, ejendomskat, dækningsafgifter eller forsikringer. |
| ![](images/Pasted-10.png) | Bygningsdel | Benyttes til anskaffelse af bygningsdele og bygningstyper. Det vil sige, at denne rækketype benyttes til byggematerialer. |
| ![](images/Pasted-12.png) | Forsyningsudgift | Forsyningsudgifter dækker over de løbende udgifter til forsyning af dit byggeprojekt, herunder varme, el og vandforbrug. |
| ![](images/Pasted-13.png) | Renholdsudgift | Renholdsudgifter dækker over de løbende udgifter til renhold af dit byggeri. Det kan fx. være vinduespudsning, gulvvask eller snerydning. |
| ![](images/Pasted-14.png) | Løbende indtægt | Løbende indtægter dækker over de løbende indtægter dit byggeri har. Det kan fx. være solcellestrøm, vindmøllestrøm eller solvarmeanlæg. |

Bemærk, at der er yderligere to rækketyper, der benyttes i de øvrige skabeloner af LCCbyg, henholdsvis ![](images/Pasted-8.png)Anskaffelse og ![](images/Pasted-15.png)Engangsindtægt. For nærmere information om disse, se ['Rækketyper og posteringer'](https://lccbyg.dk/help/34/docs/interface/costtypes/) under 'Nøgletal og kilder'.

### Posteringstyper

Der findes 9 forskellige posteringstyper I LCCbyg. Den enkle skabelon er opbygget efter et princip, hvor du skal indtaste et minimum af informationer, imens LCCbyg indeholder resten. Fælles for alle posteringstyper er, at der skal angives mængder, imens nogle også skal have inddateret enhedspriser. I det følgende gennemgås de forskellige posteringstyper og hvordan disse påvirkes af inddateringen.

#### Anskaffelse

Posten 'Anskaffelse' indeholder anskaffelsesomkostningerne i dit projekt. Typisk vil det være omkostninger til fx. facaderenovering inkl. arbejdskraft. Anskaffelsen bliver påvirket af rækker fra følgene opgavegrupper (se yderligere information om opgaver under [nøgletal](https://lccbyg.dk/help/34/docs/interface/groupeddataentry-lite/keydata/)):

- Afløb og kloak
- Altaner
- Elevator
- Elinstallationer
- Etageadskillelser
- Facader og sokler
- Gasinstallationer
- Gulve
- Indervægge og skillevægge
- Kælder og fundamenter
- Lofter
- Porte og gennemgange
- Tag
- Trapper
- Udearealer
- Vandinstallationer
- Varmeinstallationer
- Ventilation
- Vinduer og udvendige døre

#### Engangsudgift

Engangsudgifter konteres i det år, der er angivet i ‘startår’. Typisk vil engangsudgifter dække over omkostninger til byggeplads, honorarer til arkitekt, ingeniør og lignende, eller bygherreomkostninger.

#### Vedligehold

Posten for vedligeholdelse er delt i et årligt vedligehold og periodisk vedligehold. Posten for årlig vedligeholdelse dækker primært over inspektion, rensning og småreparationer. Når intervallet er lig én, medregnes vedligehold i alle år, også i det år bygningsdelen udskiftes. Et interval på én bruges derfor til at angive et teoretisk gennemsnit eller til at supplere et periodisk vedligehold med opgaver, der også udføres samme år, som en del udskiftes.

Posten for den periodiske vedligeholdelse dækker over alt andet vedligehold, der gentages i en periode over et år. Ved værdier der er større end ét, startes intervallet forfra, når en del udskiftes. Ved udskiftning bortfalder det periodiske vedligehold det pågældende år. Når intervallet er større end udskiftningsintervallet, vedligeholdes der ikke.

De inddaterede nøgletal kommer med en prædefineret vedligeholdelsesprocent, som ikke kan ændres. Denne angiver hvor mange procent af anskaffelsesværdien, der årligt skal bruges på løbende vedligehold af bygningsdelen/typen. Hvis du ønsker at afsætte et større beløb per vedligeholdsgang, kan du tilpasse dette ved at skifte til 'Almindelig grænseflade' (se  under [Hovedmenulinjen - Vis)](https://lccbyg.dk/help/31/docs/interface/help/) og afsætte et større beløb under ‘Kr./gang’.

#### Udskiftning

LCCbyg hensætter 125 % af anskaffelsesomkostning til udskiftning af bygningsdelen/typen ved endt levetid.

Udskiftningsprocenten kan ikke ændres, men hvis du ønsker at afsætte et større eller lavere beløb til udskiftning af bygningsdelen, kan du tilpasse dette ved at skifte til 'Almindelig grænseflade' (se  under [Hovedmenulinjen - Vis)](https://lccbyg.dk/help/31/docs/interface/help/) og afsætte et større beløb under ‘Kr./gang’. LCCbyg beregner udskiftning med udgangspunkt i ‘Levetid (år)’ og ‘Startår’ året for beregningsperioden. Hvis ‘Startår’ for udskiftningen er større end udløb af beregningsperioden, vil programmet ikke medtage udskiftningen.

#### Forvaltning

Forvaltning omfatter omkostninger til skatter, forsikring osv. Under denne omkostningskosttype skal mængden, enhedsprisen samt start- og slutår inddateres. Forvaltningsomkostningerne falder som en løbende udgift, der medregnes årligt fra startår til slutår.

#### Renhold

Renhold omfatter omkostninger til forskellige typer af renhold i beregningen baseret på standardværdier for frekvens (per år) og enhedspriser. Enhedsprisen dækker alle omkostninger i forbindelse med renhold inkl. rengøringspersonale og overheadomkostninger. Enhedspriserne opgøres i kr./m2 eller kr./stk.

Under ‘Inddatering’ skal du alene indtaste mængder. Du kan dog om nødvendig overskrive standardværdierne under ‘Inddatering’ ved at skifte til 'Almindelig grænseflade' (se  under [Hovedmenulinjen - Vis)](https://lccbyg.dk/help/31/docs/interface/help/). Udgifter til renhold er en løbende udgift, der medregnes årligt fra startår til slutår.

#### Løbende indtægt

Forsyningsindtægter posteres som løbende indtægter i LCCbyg. Forsyningsindtægter omfatter indtægter fra lokal produktion af elektricitet på ejendommen typisk i form af elektricitet fremstillet ved hjælp af solceller på tag og facade eller ved hjælp af en lille husstandsvindmølle på taget.

Under ‘Mine opgaver’ skal du alene indtaste mængder. Du kan dog om nødvendig overskrive enhedsprisen. Bemærk, at forsyningsindtægter skal medregnes positivt i beregningen, hvorfor enhedsprisen har positivt fortegn. Ændres enhedsprisen til negativ vil forsyningsindtægten i stedet blive en løbende udgift posteret i løbende indtægt. Forsyningsindtægt er en løbende udgift, der medregnes årligt fra startår til slutår.

#### Engangsindtægt

Engangsindtægter kan eksempelvis forekomme, hvis du får et tilskud eller sælger en bygningsdel til genbrug fx dine vinduer i år 10. Engangsindtægter kan også bruges til scrapværdier. Denne postering vil normalvis ikke påvirkes af beregninger i den enkle skabelon, da rækketyper med denne posteringstype ikke direkte kan inddateres fra nøgletallene/'Opgaver'.
