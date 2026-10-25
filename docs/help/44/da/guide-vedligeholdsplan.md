---
title: "Vedligeholdsplanen"
type: guide
start: alternatives
requires: new-project
project: maintenanceplanprojekt
description: En anden beregningsmetode for vedligehold — spørgsmål om ejendommen i stedet for priser på rækkerne.
---

Vedligeholdsplanen er en anden beregningsmetode for vedligehold: i stedet for
at summere vedligeholdet på hver række besvarer du spørgsmål om ejendommen, og
LCCbyg finder prisen inden for et typisk spænd for ejendomstypen. Guiden åbner
eksemplet "Kvalitativt vurderet vedligehold", hvor planen er udfyldt.

## Velkommen
Eksemplet har ét alternativ, **Vurdering af vedligehold**, med en udfyldt
vedligeholdsplan for en beboelsesejendom. Du kan roligt svare anderledes —
det er en kopi.

## Kontakten skifter beregningsmetode {#vedligeholdsvalg}
**Brug vedligeholdsplan** skifter alternativets vedligehold fra rækkerne til
planen: rækkernes vedligeholdskort regnes ikke med — de står nedtonede — og
planens pris pr. m² gange bruttoarealet træder i stedet. Slår du kontakten fra
igen, er rækkernes vedligehold tilbage præcis som før. Ejendomstypen — her
Beboelse — bestemmer prisspændet.

## Til alternativet {#hovedmenu}
field: Vurdering af vedligehold
action: click
wait: page=alternative

Klik på **Vurdering af vedligehold** i sidemenuen.

## Fanen Vedligeholdsplan {#alternativ-faner}
field: Vedligeholdsplan
action: click
wait: click

Planen har sin egen fane. Klik på **Vedligeholdsplan**.

## Spørgsmålsgrupperne {#vedligehold-grupper}
Hver chip er en gruppe spørgsmål — afløb, tag, facader, installationer og så
videre. Farven er gruppens niveau, fra grøn (lille behov for vedligehold) til
rød (stort), og stregen under viser, hvor meget der er besvaret.

## Svar på et spørgsmål {#vedligehold-grupper}
field: Tag
action: click
mask: none

Klik på **Tag**. Listen viser gruppens spørgsmål med en prik i svarets farve —
vælg et, og giv et andet svar i dialogen. Chippens farve, rosen og
nøgletallene følger med med det samme.

## Rosen {#vedligehold-rose}
Rosen samler vurderingen: hvert felt er en gruppe, bredden er gruppens vægt,
og længden og farven er niveauet. Midten viser det samlede niveau. Et klik på
et felt fører til gruppens spørgsmål.

## Nøgletallene {#vedligehold-noegletal}
placement: top

Bundlinjen viser ejendomstypens prisspænd pr. m² — minimum, middel og høj — og
den pris, vurderingen lander på, samt det årlige vedligehold og dets
nutidsværdi. Jo lavere niveau, jo tættere ligger prisen på minimum.

## Prisspændet {#vedligehold-enhedspriser}
page: maintenanceprerequisites

Spændet pr. ejendomstype ligger under **Forudsætninger → Vedligehold**.
Standardtyperne er låste; kopiér en type, hvis du vil regne med dine egne
priser.

## Dashboardet {#dashboard-ark}
page: results/dashboards/maintenance

Dashboardet **Vedligeholdsprofil** viser den samme rose og de samme tal på ét
ark pr. alternativ — klar til at blive gemt som billede og sat ind i en
rapport.

## Færdig
Planen er ikke et groft overslag, men en anden måde at regne på. Den kræver
ingen rækker og kan derfor bruges tidligt — men den kan lige så vel bruges på
et alternativ, der er udfyldt i detaljer, når du hellere vil vurdere
vedligeholdet ud fra ejendommens tilstand end summere det række for række.
