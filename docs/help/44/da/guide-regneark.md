---
title: "Regneark ud og ind"
type: guide
start: alternatives
requires: new-project
project: renoveringnybyggeri
description: Eksportér et alternativs grupper og rækker til Excel, ret et tal, og importér regnearket igen.
---

Et alternativ kan gemmes som regneark og læses ind igen. Så kan du rette mange
tal på én gang i Excel eller sende rækkerne til en rådgiver, der udfylder
priserne. Guiden tager dig hele vejen rundt: ud i Excel og ind igen.

## Velkommen
Vi bruger alternativet **Renovering** i eksemplet "Renovering eller nybyggeri".

## Til alternativet {#hovedmenu}
field: Renovering
action: click
wait: page=alternative

Klik på **Renovering** i sidemenuen.

## Eksportér {#eksport-regneark}
action: click
wait: click

Klik på knappen. Den gemmer alternativets grupper og rækker som en .xlsx-fil.

## Ret et tal i Excel
placement: center

Åbn filen i Excel. Hvert ark er en gruppe, og hver linje er en række. Find fx
en række, og skriv en ny mængde i kolonnen **Amount**. Gem filen, og kom
tilbage hertil.

## Importér {#import-regneark}
field: Vælg fil
action: click
wait: click

Klik på mappe-ikonet, og vælg den fil, du lige har rettet. Menuen husker også
de senest importerede filer, så næste gang kan du vælge den direkte i listen.

## Importen tilføjer
placement: center

Importen **tilføjer** regnearkets grupper til alternativet. Den retter ikke de
grupper, der var der i forvejen, så nu står grupperne der to gange: de
oprindelige og dem fra regnearket, der har fået et **1** efter navnet. Slet
dem, du ikke skal bruge, eller
importér i et nyt, tomt alternativ, så du kan sammenligne det gamle og det
rettede.

## Færdig
Regnearket er en nem vej til at rette mange tal på én gang. Har du en
tilbudsliste i Excel, kan du også kopiere rækkerne og sætte dem ind på siden
**Rækker** med knappen **Importér fra udklipsholder**.
