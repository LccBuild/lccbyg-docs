---
title: "Dashboards til præsentationen"
type: guide
start: alternatives
requires: new-project
project: renoveringnybyggeri
description: Fra sammenligningsarket til alternativernes egne ark — og gem dem som billeder til præsentationen.
---

Et dashboard er ét færdigt ark med nøgletal, grafer og rangeringer, lavet til at
blive vist frem. Guiden går arkene igennem i den rækkefølge, du typisk bruger
dem i en præsentation: først sammenligningen, så hvert alternativ for sig.

## Velkommen
Vi bruger eksemplet "Renovering eller nybyggeri" med alternativerne
**Renovering** og **Nybyggeri**. Begge regner med Finansministeriets
skyggepriser, så arket kan også rangere efter skyggepris.

## Til dashboards {#hovedmenu}
field: Dashboards
action: click
wait: page=results/dashboards

Klik på **Dashboards** i sidemenuen.

## Tre dashboards {#dashboardkort}
field: Vedligeholdsprofil

Hvert kort er ét dashboard. **Vedligeholdsprofil** er nedtonet: det viser
vurderingen fra vedligeholdsplanen, og ingen af alternativerne bruger den.
Guiden **Vedligeholdsplanen** viser det ark.

## Sammenligninger {#dashboardkort}
field: Sammenligninger
action: click
wait: page=results/dashboards/compares

Klik på **Sammenligninger**.

## Ét ark til hele beslutningen {#dashboard-ark}
Boksen til venstre har nøgletallene for hvert alternativ: bruttoareal,
nutidsværdi, restværdi, årsomkostning og CO₂ pr. m² pr. år. Nybyggeriet koster
−119,6 mio. kr. i nutidsværdi, renoveringen −149,5 mio. kr. Graferne viser,
hvordan nutidsværdien og CO₂-udledningen summeres op over de 50 år.

## Rangeringerne {#dashboard-ark}
Rul ned: nederst rangeres alternativerne tre gange. Efter nutidsværdi vinder
**Nybyggeri**, og Renovering er 25,0 % dyrere. Efter CO₂ og skyggepris vinder
**Renovering**. Rangeringerne behøver ikke at være enige, og her er de det
ikke. Det er netop den afvejning, arket skal vise frem.

## Hvem er med {#dashboard-alternativvalg}
Knappen vælger, hvilke alternativer arket regner på. Det er samme valg som
**Medtag i grafer og rapporter** på alternativkortet. Arket har plads til fem;
er flere valgt, kommer de fem første med.

## Gem som billede {#dashboard-png}
Knappen gemmer arket som PNG i tredobbelt opløsning, så det står skarpt på et
lærred eller i et dokument. Filnavnet foreslås ud fra projektets navn.

## Alternativernes egne ark {#hovedmenu}
field: Alternativer:2
action: click
wait: page=results/dashboards/alternatives

Klik på **Alternativer** under Dashboards i sidemenuen.

## Ét ark pr. alternativ {#dashboard-ark}
Hvert alternativ får sit eget ark med de fem nøgletal øverst og hovedposterne
til venstre, hver med sin andel af nutidsværdien. Rul ned til Nybyggeri:
anskaffelsen er dyrere, 81 mio. kr. mod 60 mio. kr., men salget af den gamle
ejendom giver en engangsindtægt på 21,6 mio. kr., og forsyning og renhold er
billigere. Det er derfor, nybyggeriet ender billigst.

## Færdig
Gem arkene som billeder, og sæt dem ind i præsentationen: sammenligningen
først, så hvert alternativ. Under **Rapporter** kan dashboards også indgå i en
rapport, der gemmes som PDF.
