---
title: "Biblioteket"
type: guide
start: library/mainlibraries
requires: none
description: Kontoplanerne, den semantiske søgning og rækkernes egenskaber.
---

Biblioteket er LCCbygs datasamling. Guiden viser dig kontoplanerne, en søgning
der forstår betydning, og hvor du ser en rækkes egenskaber.

## Velkommen til biblioteket
Alt, du bygger en beregning af, ligger her: bygningsdele, bygningstyper,
forsyning og renhold. Guiden går kontoplanerne igennem og viser søgningen.

## Kontoplaner {#bibliotek-kontoplaner}
Knapperne øverst er bibliotekets kontoplaner — hver sin måde at inddele data
på. Klik på dem én ad gangen for at se, hvad de indeholder.

## Bygningsdele {#bibliotek-kontoplaner}
action: click
field: Bygningsdele
wait: click

**Bygningsdele** er bygningen delt op efter SfB: fundamenter, ydervægge, tage,
installationer … Hver række har levetid og priser for anskaffelse, drift og
vedligehold.

## Bygningstyper {#bibliotek-kontoplaner}
action: click
field: Bygningstyper
wait: click

**Bygningstyper** er nøgletal for hele bygninger — boliger, skoler,
daginstitutioner, kontorer — til hurtige overslag, før bygningsdelene kendes.

## Forsyning {#bibliotek-kontoplaner}
action: click
field: Forsyning
wait: click

**Forsyning** dækker el, vand og varme: forbrug og priser, som indgår i
driftsomkostningerne.

## Renhold {#bibliotek-kontoplaner}
action: click
field: Renhold
wait: click

**Renhold** er rengøring pr. gulvtype og rum — en driftsudgift, der ofte
overses i de tidlige overslag.

## Andre nøgletal og tomme rækker {#bibliotek-kontoplaner}
action: click
field: Andre nøgletal
wait: click

**Andre nøgletal** samler øvrige erfaringstal, og **Tomme rækker** er
skabeloner, du selv udfylder, når biblioteket ikke har det, du skal bruge.

## Mine biblioteker {#bibliotek-mine}
Til højre for systemets kontoplaner står dine egne biblioteker — nøgletal, du
har importeret fra et regneark. De gemmes i projektfilen og følger projektet.
Menuen på hvert bibliotek kan **eksportere** det som regneark, **omdøbe** og
**slette** det. Systemets kontoplaner er låste og kan ikke ændres.

## Tilføj bibliotek {#bibliotek-tilfoej}
**Tilføj bibliotek** læser et regneark i LCCbygs format ind som et nyt
bibliotek. Eksportér et af dine biblioteker, ret det i Excel og importér det
igen: rækkerne genkendes, og du får at vide, hvilke der blev opdateret, tilføjet
og fjernet. Rækker, der allerede findes i en af systemets kontoplaner, kan ikke
importeres.

## Søg på betydning {#bibliotek-soegning}
placement: right
mask: none
action: type
value: Børn
wait: value

Søgningen forstår betydning, ikke kun bogstaver. Skriv **Børn** — og se, at
daginstitutionerne kommer øverst, både som bygningstype og som renhold, selv om
ordet ikke står i navnet.

## Prøv Ungdom {#bibliotek-soegning}
placement: right
mask: none
action: type
value: Ungdom
wait: value

Skriv **Ungdom**: biblioteket har ingen række med det ord, så søgningen
finder det nærmeste i betydning — igen daginstitutionerne. Der søges på tværs
af alle kontoplaner.

## Prøv Åbning {#bibliotek-soegning}
placement: right
mask: none
action: type
value: Åbning
wait: value

Skriv **Åbning**: døre og vinduer rangeres øverst, selv om "åbning" ikke står
i nogen rækkes navn. Det er betydningen, der matcher.

## Sortér resultaterne {#bibliotek-sortering}
placement: right
mask: none

Under en søgning kan du lægge en almindelig sortering oven på relevansen —
navn, kode, kontoplan eller variant. **Relevans** vender tilbage til
søgningens egen orden.

## Vælg en række {#bibliotek-raekker}
Klik på en række i tabellen for at se, hvad den indeholder.

## Rækkens egenskaber {#bibliotek-egenskaber}
Panelet til højre viser rækkens mængder, priser, levetid og moduler — det
samme, som rækkekortet viser, når rækken er hentet ind i en gruppe.

## Færdig
Nu kender du biblioteket. Rækkerne henter du ind i dine grupper med
**Tilføj rækker** på rækkesiden — søgningen virker på samme måde dér.
