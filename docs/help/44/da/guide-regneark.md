---
title: "Regneark ud og ind"
type: guide
start: alternatives
requires: new-project
project: renoveringnybyggeri
description: Eksportér et alternativs grupper og rækker til Excel, ret tallene, og importér dem igen — og gem en visning som regneark.
---

Et alternativ kan gemmes som regneark og læses ind igen. Så kan du rette mange
tal på én gang i Excel eller sende rækkerne til en rådgiver, der udfylder
priserne. Guiden viser, hvad regnearket indeholder, og hvad importen gør med
det.

## Velkommen
Vi bruger alternativet **Renovering** i eksemplet "Renovering eller nybyggeri".

## Til alternativet {#hovedmenu}
field: Renovering
action: click
wait: page=alternative

Klik på **Renovering** i sidemenuen.

## Eksportér {#eksport-regneark}
Knappen gemmer alternativets grupper og rækker som en .xlsx-fil, du kan åbne i
Excel.

## Ét ark pr. gruppe
placement: center

Regnearket har et ark for hver gruppe med én linje pr. række. Gruppens egen
linje står øverst på arket. Arket **Information** henviser til en beskrivelse
af formatet på lccbyg.dk.

## Kolonnerne
placement: center

Kolonnerne har LCCbygs feltnavne: **Amount** er mængden, **Unitprice**
enhedsprisen og **Lifetime** levetiden. Der er også kolonner for vedligehold,
udskiftning og CO2-modulerne. Kolonner, der begynder med **Base**, er
bibliotekets værdier. Vil du ændre en værdi, så skriv den i kolonnen uden
Base.

## Nye rækker
placement: center

En ny linje på et ark bliver til en ny række i gruppen. Det nemmeste er at
kopiere en eksisterende linje, slette dens **UUID** og rette navn, mængde og
pris.

## Importér {#import-regneark}
Knappen henter regnearket ind igen. Menuen viser de senest importerede filer,
og mappe-ikonet øverst vælger en ny fil. Kun .xlsx kan importeres her.

## Importen tilføjer
placement: center

Importen **tilføjer** regnearkets grupper til alternativet. Den retter ikke i
de grupper, der allerede er der. Importér derfor i et nyt, tomt alternativ
(**Tilføj et alternativ** under Alternativer). Så har du både det oprindelige og
det rettede og kan sammenligne dem. Regnearket rummer kun grupper og rækker,
så sæt bruttoareal og forudsætninger på det nye alternativ, som på det gamle.

## Til visningerne {#hovedmenu}
field: Visninger
action: click
wait: page=visninger

Visningerne kan også gemmes som regneark. Klik på **Visninger** i sidemenuen.

## Opsummeret nutidsværdi {#visningskort}
field: Opsummeret nutidsværdi
action: click
wait: page=visning

Klik på visningen **Opsummeret nutidsværdi**.

## Gem visningen som regneark {#visning-eksport}
Knappen gemmer visningens tal som .xlsx, også når visningen er en graf. Viser
visningen et panel pr. alternativ, får hvert alternativ sit eget ark.

## Færdig
Regnearket er en nem vej til at rette mange tal på én gang. Har du en
tilbudsliste i Excel, kan du også kopiere rækkerne og sætte dem ind på siden
**Rækker** med knappen **Importér fra udklipsholder**.
