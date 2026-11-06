---
title: "Opret din første beregning"
type: guide
start: project
requires: new-project
description: Fra tomt projekt til de første rækker — navn, alternativ, gruppe og rækker.
---

Guiden fører dig gennem de første skridt i en beregning: projektets navn, et
alternativ, en gruppe og gruppens rækker. Den åbner et nyt, tomt
standardprojekt, så dit eget arbejde ikke røres.

## Velkommen
Du står nu i et nyt, tomt standardprojekt. Guiden peger på ét element ad
gangen — gør selv det, der står, eller lad **Vis mig** gøre det for dig.

## Giv projektet et navn {#stamoplysninger}
action: type
field: Projekttitel
value: Min første beregning
wait: value

Skriv projektets titel. Den vises i vinduets titel og øverst i rapporterne.

## Rapportafsnit {#rapportfelter}
De øvrige felter er fritekst, der følger med ind i rapporten. Dem kan du
udfylde senere.

## Gå til alternativerne {#nav-alternativer}
action: click
wait: page=alternatives

Beregningen bygges op af alternativer. Klik på **Alternativer** i sidemenuen.

## Tilføj et alternativ {#tilfoej-alternativ}
action: click
wait: click

Et alternativ er ét samlet bud på en løsning — fx "renovering" eller
"nybyggeri". Klik på **Tilføj et alternativ**.

## Åbn alternativets grupper {#grupper-knap}
action: click
wait: page=alternative

Det nye alternativ har fået et kort. Klik på **Grupper**-knappen for at bygge
det op.

## Tilføj en gruppe {#tilfoej-gruppe}
action: click
wait: click

En gruppe samler de rækker, der hører sammen — fx en bygningsdel. Klik på
**Tilføj gruppe**, giv gruppen et navn og tryk OK.

## Åbn gruppens rækker {#raekker-knap}
action: click
wait: page=alternative-group-rows

Klik på **Rækker**-knappen på gruppekortet.

## Tilføj rækker {#tilfoej-raekker}
action: click
wait: click

Rækkerne er selve beregningen: bygningsdele og ydelser med mængder og priser.
Klik på **Tilføj rækker**, vælg en eller flere rækker i biblioteket, og luk
dialogen igen.

## Angiv en mængde {#raekkegrid}
field: Mængde
action: type
value: 10
wait: value

Klik i kolonnen **Mængde** på den første række, og skriv hvor meget der skal
bruges — fx 10. Enheden står i kolonnen ved siden af.

## Angiv en enhedspris {#raekkegrid}
field: Enhedspris
action: type
value: 1500
wait: value

Skriv prisen pr. enhed i **Enhedspris**. Rækkens sum og resultaterne nederst
opdateres med det samme.

## Færdig
Du har nu et projekt med et alternativ, en gruppe og rækker med mængde og
pris. Resultaterne opdateres løbende, mens du arbejder — og du gemmer
projektet via menuen, når du vil beholde det.
