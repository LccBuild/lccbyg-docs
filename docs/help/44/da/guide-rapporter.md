---
title: "Lav en rapport"
type: guide
start: alternatives
requires: new-project
project: renoveringnybyggeri
description: En kort rapport til bestyrelsen — ny rapport, afsnit til og fra, din egen anbefaling, logo og PDF.
---

En rapport er ét dokument med de afsnit, du slår til. Guiden laver en kort
rapport til bestyrelsen i eksemplet "Renovering eller nybyggeri": projektets
beskrivelse, sammenligningsarket og din egen anbefaling, gemt som PDF.

## Velkommen
Bestyrelsen ønsker et hurtigt overblik over de to alternativer. Vi starter fra
en tom rapport og slår kun det til, der skal med.

## Til rapporterne {#hovedmenu}
field: Rapporter
action: click
wait: page=rapporter

Klik på **Rapporter** i sidemenuen.

## Rapportmenuen {#rapport-menu}
wait: click

Klik på de tre prikker. Menuen laver, omdøber og sletter rapporter.

## En ny, enkel rapport {#rapport-ny}
field: Ny rapport: Enkel rapport
action: click
wait: click

Klik på **Ny rapport: Enkel rapport**. Den har kun sidehoved og sidefod, så du
selv vælger indholdet. **Standard** og **Komplet** har flere figurer og tabeller
slået til fra start.

## Giv den et navn {#tekst-dialog}
Skriv fx **Til bestyrelsen**, tryk **OK**, og tryk så **Næste**. Projektet har
nu to rapporter, og vælgeren øverst til venstre skifter mellem dem.

## Projektet først {#rapport-indhold}
field: Projektoplysninger

Hvert afsnit har en kontakt til højre. **Projektoplysninger** er slået til og
viser projektets navn og beskrivelse fra siden Projektoplysninger. Retter du
dem dér, retter rapporten sig selv.

## Sammenligningen {#rapport-indhold}
field: Sammenligninger
action: click
wait: click

Slå **Sammenligninger** til under Dashboards. Arket er det samme som under
Dashboards, med nøgletal, grafer og rangeringer.

## Din anbefaling {#rapport-tilfoej}
field: Tilføj tekstfelt
action: click
wait: click

Tallene står ikke alene. Klik på **Tilføj tekstfelt** under "Brugerdefinerede
tekst og billeder".

## Skriv teksten {#rapport-indhold}
field: Overskrift

Skriv en overskrift, fx **Anbefaling**, og i brødteksten hvad bestyrelsen skal
tage stilling til: nybyggeriet er billigst i nutidsværdi, renoveringen udleder
mindst CO2. Skraldespanden ved afsnittets navn fjerner det igen.

## Billeder {#rapport-tilfoej}
field: Tilføj illustration

**Tilføj illustration** indsætter et billede med billedtekst, fx et
situationsfoto eller en skitse. Du vælger, om det fylder 50, 75 eller 100 % af
sidens bredde.

## Logoet {#rapport-logo}
Billedet øverst står i sidehovedet på hver side. Billed-ikonet til højre
skifter det til jeres eget logo.

## Hvem er med {#rapport-alternativvalg}
Knappen vælger, hvilke alternativer rapportens dashboards, figurer og tabeller
tager med, som **Medtag i grafer og rapporter** på alternativkortet.

## Gem som PDF {#rapport-pdf}
Knappen gemmer rapporten som PDF. Kun det, der er slået til, kommer med, i
samme rækkefølge som på siden, og hver side får sidehoved og en sidefod med
sidetal, dato og projektnavn.

## Færdig
Rapporten gemmes i projektet, så den er der næste gang med de samme valg, og
tallene følger beregningen. Længere tekster som baggrund og forudsætninger kan
også skrives under **Projektoplysninger**; de udfyldte felter kommer med under
Generelt. Omdøb eller slet rapporten i menuen med de tre prikker.
