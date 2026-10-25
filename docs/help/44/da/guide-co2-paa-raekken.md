---
title: "CO2 på rækken — LCA-modulerne"
type: guide
start: alternatives
requires: new-project
project: tageeksempel
description: Hvor rækkens CO2 kommer fra: LCA-modulerne på hvert omkostningskort, og hvordan de bliver til rækkens og alternativets udledning.
---

Rækkens CO2 regnes ud fra LCA-moduler: livscyklusfaser som A1-3 (produktion),
B4 (udskiftning) og C3-C4 (affald og bortskaffelse). Guiden følger et sadeltag
i eksemplet "Tage" og viser, hvor modulerne står, og hvordan de lægges sammen.

## Velkommen
Taget ligger i alternativet **Sadeltag**. Bagefter sammenligner vi med det
CO2-reducerede sadeltag ved siden af.

## Til alternativet {#hovedmenu}
field: Sadeltag
action: click
wait: page=alternative

Klik på **Sadeltag** i sidemenuen.

## Til gruppen {#hovedmenu}
field: Sadeltag:2
action: click
wait: page=alternative-group-rows

Gruppen hedder også **Sadeltag**. Klik på den, den står lige under
alternativet.

## Åbn rækken {#raekkegrid}
field: Navn
action: click
wait: click

Klik på **Sadeltag** for at åbne rækkens detaljer.

## Generelt {#raekkekort}
field: Generelt

**Miljøpåvirkning** vælger, hvilken linje i alternativets miljøscenarie
rækkens CO2 fremskrives med over tid.
Knappen **Tilføj/nulstil CO₂-ækv moduler** erstatter rækkens moduler med tomme
moduler, så du kan skrive dine egne tal ind, fx fra en EPD. Tryk ikke på den
her, for så forsvinder eksemplets tal.

## Anskaffelse — A1-3 {#raekkekort}
field: Anskaffelse

Ved siden af priserne står kortets moduler. **A1-3** er produktionen af materialerne:
6,79 kg CO2 pr. m², **per gang**, dvs. én gang ved opførelsen. Med 450 m² giver
det 3.055 kg CO2.

## Vedligehold — B2 {#raekkekort}
field: Vedligehold

Vedligeholdet har modulet **B2**, men det er tomt i dette datasæt. Kortets pris
tæller med i økonomien, men ikke i CO2.

## Udskiftning — B4, C3 og C4 {#raekkekort}
field: Udskiftning

Udskiftning af dele (B4), affaldsbehandling (C3) og bortskaffelse (C4) står
**per år**: i alt 0,55 kg CO2 pr. m² hvert år. Tallene er allerede
fordelt over årene, så de tæller i alle periodens 50 år, selv om hele taget
først skiftes i år 80. Det giver 12.442 kg CO2.

## Genanvendelse — D {#raekkekort}
field: Genanvendelse

**D** er potentialet for genbrug og genanvendelse efter endt levetid. Det er
ikke udfyldt her.

## Rækkens CO2 {#raekke-noegletal}
placement: top

**CO₂-ækv i alt** er 15.498 kg, altså 3.055 kg ved opførelsen plus 12.442 kg
over årene. **Emissioner** er det samme pr. m² pr. år: 15.498 kg / 450 m² /
50 år = 0,69 kg CO2/m²/år.

## Luk rækken {#raekke-afslut}
field: Fortryd
action: click
wait: click

Tryk **Fortryd** for at lukke rækkens detaljer uden at gemme noget.

## Det CO2-reducerede tag {#hovedmenu}
field: Sadeltag - CO2 reduceret
action: click
wait: page=alternative

Klik på **Sadeltag - CO2 reduceret** i sidemenuen.

## Næsten halvt så meget CO2 {#resultat-ticker}
field: CO₂-ækv i alt

Her er tallet 8.509 kg mod 15.498 kg. Taget har genbrugte tegltagsten, som
ikke skal produceres igen, og papirisolering, der har optaget CO2, mens
træet voksede. Derfor er A1-3 **−46,37** kg pr. m². Til gengæld er C3 større,
1,22 kg pr. m² pr. år, fordi papiret brændes, når det bortskaffes.
Nutidsværdien er derimod lidt dårligere: −1,46 mio. kr. mod −1,21 mio. kr.

## Færdig
Rækker fra biblioteket har modulerne med. Vil du bruge dine egne tal, så nulstil
modulerne og skriv tallene ind. Guiden **Miljøpåvirkning og CO2-faktorer**
viser, hvordan faktorerne fremskrives over tid, og **Skyggepriser** viser,
hvordan CO2 kan regnes om til kroner.
