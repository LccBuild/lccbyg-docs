---
layout: lccbyghelp40
title: "Versionshistorik LCCbyg 4"
date: "2024-03-04"
search: false
---

# LCCbyg 4 - Versionshistorik

## [4.4.10]

#### Added
- [Guider] 22 guider i hjælpepanelet viser trin for trin rundt i LCCbyg, fra den første beregning over alternativer, biblioteket, vedligeholdsplanen og visninger til dashboards og rapporter. En guide åbner selv det projekt, den bruger, og peger på de knapper og felter, du skal bruge.
- [Vedligeholdsplan] Felterne i rosen og chipsene under den er links ned til den gruppe af spørgsmål, de handler om. Rosen står nu øverst.

#### Changed
- [Biblioteker] Renhold og Forsyning er låste biblioteker fra LCCbyg ligesom de øvrige standardbiblioteker. Projekter fra ældre versioner, der ikke selv angiver deres biblioteker, får de samme seks biblioteker som et nyt standardprojekt: Bygningstyper, Bygningsdele, Forsyning, Renhold, Andre nøgletal og Tomme rækker.
- [Eksempler] Eksempelprojekternes rækker følger bibliotekernes aktuelle navne og priser, så de igen vises med grønt ikon. Bl.a. er renholdsrækkerne skiftet til bibliotekets nuværende rækker, og forsyningspriserne følger Forsyning.
- [DGNB-skabeloner] DGNB kontor og DGNB hospital er tomme skabeloner opbygget som standardskabelonen, med DGNB-logo. Eksemplerne bruger faldende realrente.
- [Tekster] Stave- og grammatikrettelser i programmets tekster, bibliotekernes beskrivelser og vedligeholdsplanens spørgsmål og svar. CO₂, m² og m³ skrives med sænket og hævet skrift.

#### Removed
- [Lite] Lite-eksemplet vises midlertidigt ikke på forsiden.

#### Fixed
- [Projektets logo] Et projekt med eget logo kunne få LCCbyg-logoet i stedet, når det blev åbnet.
- [Skabeloner] Skabelonerne henviste til kontoplanen Vedligehold, som ikke findes længere.
- [Guider] En guide kunne fejle, når den åbnede sit projekt.

## [4.4.9]

#### Changed
- [Spørgeskema til vedligeholdsplan] Ja står altid til højre og Nej til venstre, og skalaer læses lav, middel, høj. Svarkortene er neutrale, kun det valgte er markeret, og en måler med fem cirkler viser hvert svars score.
- [Vedligeholdsplan] Spørgsmålet om lofttype vurderer fast loft dårligst, nedhængt loft i midten og åbent bedst.
- [Projektoplysninger] Titlerne står over felterne og bliver stående, også når feltet er tomt.
- [Figurer] Enheden står på værdiaksen (kr. eller kg CO₂e) og År på tidsaksen. Dashboardets figurer har en overskrift med enhed.
- [Biblioteket] Kontoplaner og grupper med en beskrivelse har et info-ikon foran navnet.
- [Søgning i biblioteket] Søgningen er klar fra start. Tekstsøgningen filtrerer fra første tegn, den semantiske søgning fra tredje, og der vises højst 50 rækker under søgning.
- [Indsæt og erstat rækker] Påmindelsen om at tilrette mængde og enhedspris står i dialogen i stedet for i en meddelelse, der forsvandt for hurtigt.
- [Målsætninger] En redigering kan fortrydes samlet med Fortryd eller Escape. Vitruvius' principper står uden numre.
- [Startsiden] Versionsnummeret står i bundlinjen.

#### Fixed
- [Eksport af figur] Figurer kunne ikke gemmes som PNG.
- [Dashboards og rapporter] Figurer kunne være tomme.
- [Sammenligningsdashboard] "Mindste skyggepris" viste den største.
- [Gruppeomkostninger] Vedligeholdsplanens række havde ikke det rigtige navn, og Sum stod ikke altid nederst.
- [Rækkegrid] Et rettet navn vises sort. Navne fra biblioteket forbliver grønne.
- [Vedligeholdsplan] To spørgsmål om tilgængelighed uden lift havde vendt værdierne om.
- [Klassisk tema] Sprogvælgeren og Menu-knappen forsvandt på den hvide topbjælke.
- [Moderne tema] Første linje i felter med flere linjer blev skåret af.
- [Målsætninger] Overskrifterne på vigtighedskortene kunne ikke læses i mørkt tema.
- [Rapporter] Siden hoppede til toppen ved tilvalg. Et udskiftet logo kan fjernes igen, så LCCbyg-logoet kommer tilbage. Billeder centreres i PDF'en.
- [Regnearksimport] En gruppe beholder sin egen label, beskrivelse og sine koder.

## [4.4.8]

#### Added
- [Sammenligning af alternativer] En figur viser forskellene med én graf pr. nøgletal. Differencetabellerne har en kolonne med forskellen i procent.
- [Rapporter] Tre rapportskabeloner i menuen: Enkel rapport, Standard rapport og Komplet rapport. Rapporter kan omdøbes.
- [Egne biblioteker] Importerer du et bibliotek, du allerede har, kan du vælge at tilføje, erstatte eller opdatere det.

#### Changed
- [Egne biblioteker] Rækker i egne biblioteker er skrivebeskyttede indtil videre.
- [Indsæt og erstat rækker] Knappen siger, hvad der sker: "Indsæt denne række", "Erstat med disse 3 rækker" osv.
- [Visninger] Kopiering til udklipsholderen giver en ren tabel uden titellinje.
- [Vedligeholdsprofil] Plads til de længere tekster og rosens yderste etiketter.
- [Opstart] Desktopprogrammet starter hurtigere igen.

#### Fixed
- [Faner] Den valgte fane havde mørk tekst på mørk bund i Klassisk mørkt tema.
- [Rækkedetaljer i biblioteket] Vedligeholds- og udskiftningsprocent vises igen.

## [4.4.7]

#### Added
- [Egne biblioteker] Egne biblioteker kan importeres fra regneark, eksporteres, omdøbes og slettes igen.
- [Rapporter] Ny rapport fra en skabelon. Rapporter kan omdøbes og slettes.
- [Visninger] Nøgletal pr. alternativ side om side.

#### Changed
- [Visninger] GWP-udtræk viser alternativernes navne, fasernes navne og enheder, også når de kopieres til udklipsholderen eller eksporteres til regneark.
- [Figurer] Farver pr. omkostningsfamilie.
- [Faner] Den valgte fane er tydeligere markeret.
- [Biblioteket] Tydeligere navigation i målsætninger og en tydelig erstat-handling.
- [Vedligeholdsprofil] Dashboardet har fået nye titler.
- [Rapport] Billeder vises i den valgte bredde.

#### Removed
- [Skabeloner] Skabelonen "Almene boliger med SfB".
- [Alternativer, listevisning] Den unødige markeringsboks i bunden.

## [4.4.6]

#### Added
- [Eksempel] Nyt eksempel: kvalitativt vurderet vedligehold.
- [Tabeller] Markeringskolonne med vælg alle.

#### Changed
- [Skyggepriser] Finansministeriets og Klimarådets sæt er opdateret til juni 2026.
- [Installation] Installationen fylder ca. 200 MB mod tidligere ca. 470 MB.
- [Søgning i biblioteket] Søgeindekset bygges ved start, og der vises fremdrift, mens det bygges.

## [4.4.5]

#### Changed
- [Installation] Unødvendige filer er fjernet fra installationen.

## [4.4.4]

Første udgave af LCCbyg 4.4.

#### Added
- [Vedligeholdsplan] Vedligehold kan vurderes ud fra et spørgeskema i stedet for at prissætte hver række. Det slås til pr. alternativ. Et nyt dashboard viser vurderingen som en rose.
- [Visninger] Resultaterne er samlet som visninger, der kan ses som tabel eller som graf med de samme tal.
- [Hjælp] Ny hjælp i et panel ved siden af programmet. Hjælpen følger den side og fane, du står på, "Vis mig hvor" springer til funktionen, og du kan søge med almindeligt sprog.
- [Søgning i biblioteket] Søgningen i biblioteket og i projektets rækker forstår betydning, ikke kun stavning. Søgeresultaterne viser kontoplanen.
- [Rapporter] Ny rapportmotor. Rapporten bygges som én side, kan indeholde dashboards og gemmes som PDF.
- [Alternativer] Faner for Grupper, Vedligeholdsplan og Bedømmelse, en vælger til at skifte alternativ og adgang til alternativer og grupper fra venstremenuen. Grupper kan vises som liste, hvor flere kan markeres og kopieres, klippes, indsættes eller slettes på én gang.
- [Udklipsholder] Indsætning fra udklipsholderen genkender selv format og kolonner.
- [Forside] Skabelonerne vises som kort eller liste, og de senest brugte filer ligger i menuen.

#### Changed
- [Beregning] Beregningen kører parallelt og opdateres løbende, mens du indtaster.
- [Levetider] Levetidstabel 2025.
- [Figurer] Ny grafmotor.
- [Installation] LCCbyg 4.4 installeres ved siden af version 4.0, for din egen brugerprofil og uden administratorrettigheder. Installationsfilen er signeret.

#### Removed
- [Biblioteket] Kontoplanerne Opgaver og DGNB byrum.

#### Fixed
- [Faldende realrente] Når kalkulationsrenten skifter undervejs i beregningsperioden (fx 3,5 % i år 1-35, 2,5 % i år 36-70 og 1,5 % derefter), diskonteres hvert år nu med de renter, der har gældt frem til det år, som i Finansministeriets vejledning i samfundsøkonomiske konsekvensvurderinger (juni 2023). Tidligere versioner brugte det enkelte års rente på hele perioden, så nutidsværdier og annuiteter blev for store for alle år efter det første renteskift. Projekter med en beregningsperiode over 35 år viser derfor lavere nutidsværdier end i 4.0.52; fx falder standardprojekteksemplet med ca. 2,4 mio. kr. Samme rettelse gælder prisudviklinger med flere satser.
- [Vedligeholdsplan] Vedligeholdsplanen var fælles for alle alternativer, og en kopi af et alternativ mistede valget af vedligeholdsplan.
- [Rapport] Ændringer i projektoplysningerne kom ikke med i rapporten som PDF.
- [Regnearksimport] En gruppe med samme navn som alternativet forsvandt ved import.
- [Dashboard-eksport] Illustration og skrifttype kom ikke med, når et dashboard blev gemt som PNG.
- [Mørkt tema] Tekster forsvandt.
- [Erstat] Erstat virkede først ved andet klik.
- [Bygningstyper] Navne og levetider manglede for nogle bygningstyper.
- [Dashboard] Enheden manglede på GWP i sammenligningen af alternativer.
