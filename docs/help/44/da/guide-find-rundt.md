---
title: "Find rundt i LCCbyg"
type: guide
start: alternatives
requires: new-project
description: Sidemenuen, alternativerne og grupperne i menuen, brødkrummen og pilene.
---

LCCbyg er bygget op i samme rækkefølge, som du arbejder: fra projektets
oplysninger over forudsætningerne til alternativerne og resultaterne. Guiden
viser, hvordan du finder rundt — og hvordan du springer direkte mellem
alternativer og grupper. Den åbner et nyt, tomt standardprojekt, så dit eget
arbejde ikke røres.

## Velkommen
Du står på Alternativer i et nyt standardprojekt. Guiden peger på ét element ad
gangen — klik selv, eller lad **Vis mig** gøre det.

## Sidemenuen {#hovedmenu}
placement: right

Menuen står i arbejdsrækkefølge: **Projektoplysninger** og **Målsætninger**
først, så **Forudsætninger**, derefter **Alternativer**, hvor beregningen
bygges, og til sidst resultaterne i **Visninger**, **Dashboards** og
**Rapporter**.

## Forudsætningerne {#hovedmenu}
field: Forudsætninger

Forudsætningerne gælder hele projektet: biblioteket, prisudviklinger,
miljøpåvirkning, skyggepriser og vedligehold. Står du dér, folder punktet sig
ud med de fem sider.

## Alternativerne står i menuen {#hovedmenu}
field: Nyt alternativ
action: click
wait: page=alternative

Under **Alternativer** står projektets alternativer — her kun ét, "Nyt
alternativ". Klik på det for at åbne det direkte.

## Og grupperne under dem {#hovedmenu}
field: Unavngiven gruppe
action: click
wait: page=alternative-group-rows

Når du står i et alternativ, folder menuen dets grupper ud. Klik på gruppen
for at gå direkte til dens rækker — har alternativet flere grupper, springer
du på samme måde fra den ene til den anden.

## Hvor er du? {#broedkrumme}
Toplinjen viser, hvor du står: alternativets navn og gruppens navn.
Alternativets navn er et link op til alternativet.

## Op, tilbage og frem {#navigation-pile}
Op-pilen fører ét niveau op — fra gruppen til alternativet, fra alternativet
til oversigten. Tilbage og frem virker som i en browser.

## Færdig
Det var kortet over programmet. Guiden **Værktøjskassen** viser de knapper, der
følger dig rundt: resultaterne, quickview, fortryd og hjælpen.
