---
title: "Visninger — find og læs resultaterne"
type: guide
start: alternatives
requires: new-project
project: standardprojektexample
description: Find en visning i kataloget, læs den som tabel og figur, vælg opdeling og alternativer, og tag tallene med videre.
---

Visningerne er dine resultater: økonomi, CO2, målsætninger og forudsætninger.
Hver visning kan ses som tabel eller figur med de samme tal. Guiden finder en
visning i kataloget og går dens knapper igennem.

## Velkommen
Vi bruger "Eksempel på standardprojekt" med alternativerne **Teglvæg og
træbeklædning** og **Beton og solceller**.

## Til visningerne {#hovedmenu}
field: Visninger
action: click
wait: page=visninger

Klik på **Visninger** i sidemenuen.

## Kataloget {#visningskort}
field: Målsætninger

Hvert kort er én visning med navn, beskrivelse og et ikon for, om den åbner
som tabel eller figur. Et nedtonet kort mangler data: **Målsætninger** viser
bedømmelser, og alternativerne er ikke bedømt endnu.

## Søg {#visnings-soegning}
action: type
value: klassifikation

Feltet filtrerer kortene, mens du skriver, både på navn og beskrivelse. Skriv
fx **klassifikation**, eller tryk **Vis mig**.

## Åbn en visning {#visningskort}
field: Omkostninger efter klassifikation
action: click
wait: page=visning

Klik på **Omkostninger efter klassifikation**.

## Tabellen {#visning-indhold}
field: Kode:3

Én linje pr. kode og én kolonne pr. alternativ. Ydervæggene (SfB 21.3) koster
mest i teglvæg-alternativet, mens taget (27.1) koster mest i
beton-alternativet med solceller.

## Opdeling {#visning-parameter}
**Klassifikation** vælger, hvad omkostningerne opdeles efter: SfB, BOSSINF,
forvaltningsklassifikation, BIM-typekode eller vedligehold. Listen viser kun
de klassifikationer, projektets rækker er mærket med.

## Tabel eller figur {#visning-tabel-graf}
field: Figur
action: click
wait: click

Klik på **Figur**. Tallene er de samme; kun formen skifter.

## Vælg alternativer {#visning-alternativvalg}
Knappen vælger, hvilke alternativer visningen tager med. Det er samme valg
som **Medtag i grafer og rapporter** på alternativkortet.

## Kopiér og gem som billede {#visning-indhold}
Over figuren kopierer den ene knap tabellen som tekst, med navne og enheder,
så den kan sættes ind i et dokument. Den anden gemmer figuren som billede.
Visninger, der viser ét panel pr. alternativ, har knapperne på hvert panel.

## Regneark {#visning-eksport}
Knappen gemmer visningens tal som regneark.

## Færdig
Visningerne ligger også direkte i sidemenuen under **Visninger**, og pilen op i
toplinjen fører fra en visning tilbage til kataloget.
