---
title: "Nu eller senere? Tiden i beregningen"
type: guide
start: alternatives
requires: new-project
project: lite_eksempel
description: Hvorfor en udgift om ti år vejer mindre end en i dag — nutidsværdi, kalkulationsrente og restværdi i et konkret eksempel.
---

Det samme arbejde koster ikke det samme i en totaløkonomisk beregning, hvis
det udføres på forskellige tidspunkter. Guiden sammenligner en renovering, der
udføres nu, med en, hvor taget venter ti år — og viser hvorfor.

## Velkommen
Eksemplet "Tag- og vinduesudskiftning" har to løsninger: alt på én gang nu,
eller vinduerne nu og taget om ti år.

## Alt nu {#alternativkort}
field: Fuld renovering nu - trævinduer

**Fuld renovering nu - trævinduer** skifter vinduer og renoverer taget i år
0.

## Nutidsværdien {#resultat-ticker}
Nutidsværdien er alle fremtidige udgifter og indtægter regnet om til kroner i
dag. For "alt nu" er den omkring −3,96 mio. kr.

## Taget om ti år {#alternativkort}
field: Forskudt renovering - trævinduer

**Forskudt renovering - trævinduer** gør det samme arbejde, men udskyder
tagrenoveringen til år 10. Nutidsværdien lander på omkring −3,80 mio. kr.:
ca. 160.000 kr. billigere for det samme arbejde.

## Kalkulationsrenten
placement: center

Eksemplet regner med **Fast realrente**: 3 % om året. En udgift om ti år
tilbagediskonteres derfor — 100 kr. i år 10 svarer til ca. 74 kr. i dag. Til
gengæld stiger byggeomkostningerne 0,6 % om året ud over den generelle
prisudvikling, så taget bliver lidt dyrere af at vente.

## Til visningerne {#hovedmenu}
field: Visninger
action: click
wait: page=visninger

Klik på **Visninger** i sidemenuen.

## Opsummeret nutidsværdi {#visningskort}
field: Opsummeret nutidsværdi
action: click
wait: page=visning

Klik på visningen **Opsummeret nutidsværdi**.

## Se det år for år {#visning-indhold}
Visningen **Opsummeret nutidsværdi** lægger nutidsværdien sammen år for år,
med én kurve pr. alternativ. Kurverne for "alt nu" falder brat i år 0; de
forskudte deler springet i to — år 0 og år 10.

## Restværdien {#visning-indhold}
Restværdien kommer først med i sidste år: værdien af den levetid,
bygningsdelene har tilbage, når perioden slutter. Et tag lagt i år 10 er ti år
yngre ved periodens slut og har derfor mere værdi tilbage.

## Vælg hvad der sammenlignes {#visning-alternativvalg}
Knappen vælger, hvilke alternativer visningen tegner. Vælg kun de to med
trævinduer, hvis du vil se forskydningen alene.

## Færdig
Tidspunktet tæller: en udgift senere vejer mindre i dag, og en nyere
bygningsdel har mere restværdi tilbage ved periodens slut. Start- og slutår på
grupperne og levetiden på rækkerne er de greb, der flytter udgifterne i tid.
