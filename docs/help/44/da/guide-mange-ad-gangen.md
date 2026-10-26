---
title: "Mange ad gangen — markér, kopiér og indsæt"
type: guide
start: alternatives
requires: new-project
project: renoveringnybyggeri
description: Markér flere grupper i listevisningen og kopiér dem til et andet alternativ i én arbejdsgang.
---

I listevisningen kan du markere flere grupper og kopiere, klippe eller slette
dem på én gang. Guiden bygger en variant af renoveringen, hvor medarbejderne
bliver i bygningen: et nyt alternativ med tre af Renoverings fire grupper,
altså uden genhusningen.

## Velkommen
Vi bruger eksemplet "Renovering eller nybyggeri". Først laver vi et tomt
alternativ, så henter vi grupperne til det.

## Et nyt alternativ {#tilfoej-alternativ}
action: click
wait: click

Klik på **Tilføj et alternativ**. Det nye alternativ hedder **Nyt alternativ**
og er tomt.

## Til Renovering {#hovedmenu}
field: Renovering
action: click
wait: page=alternative

Klik på **Renovering** i sidemenuen.

## Listevisningen {#gruppe-listevisning}
action: type
value: true

Markering af flere grupper kræver listevisning; i kortvisningen arbejder du
med én gruppe ad gangen. Står **Listevisning** fra, så slå den til, eller tryk
**Vis mig**.

## Markér tre grupper {#gruppe-liste}
Sæt flueben ved **Byggearbejder**, **Forsyning** og **Renhold**, men ikke ved
genhusningen. Fluebenet står yderst til venstre i hver linje.

## Åbn menuen {#gruppe-redigeringsmenu}
action: click
wait: click

Klik på de tre prikker øverst i listen. Menuen virker på alle de markerede
grupper.

## Kopiér {#gruppe-kopier}
action: click
wait: click

Klik på **Kopiér**. De tre grupper ligger nu på LCCbygs udklipsholder med
alle deres rækker.

## Til det nye alternativ {#hovedmenu}
field: Nyt alternativ
action: click
wait: page=alternative

Klik på **Nyt alternativ** i sidemenuen. Udklipsholderen følger med.

## Åbn menuen igen {#gruppe-redigeringsmenu}
action: click
wait: click

Klik på de tre prikker igen.

## Indsæt {#gruppe-indsaet}
action: click
wait: click

Klik på **Indsæt**. Grupperne sættes ind som kopier, så Renovering er
uændret.

## Tre grupper på én gang {#gruppe-liste}
Det nye alternativ har nu de tre grupper med alle rækker. Alternativets egne
felter følger ikke med grupperne: giv det et navn, og sæt bruttoareal og
forudsætninger på alternativkortet som på Renovering, før du sammenligner.

## Færdig
**Klip** flytter grupperne i stedet for at kopiere dem, og **Slet** fjerner
dem. Højreklik på en gruppe for at arbejde med netop den eller sætte ind over
eller under den. Rækkerne i en gruppe markeres og kopieres på samme måde.
Fortryd (Ctrl+Z) tager en hel indsættelse eller sletning tilbage på én gang.
Skal hele alternativet med, er **Kopiér** på alternativkortet hurtigere.
