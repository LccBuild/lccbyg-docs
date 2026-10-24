---
title: "Grupper — del beregningen op på din måde"
type: guide
start: alternatives
requires: new-project
project: lite_eksempel
description: Fag, etaper, bygningsdele eller budget-ejer — grupperne kan dele et alternativ op på mange måder.
---

Grupperne bestemmer, hvordan et alternativ er delt op — og der er ikke én
rigtig måde. Guiden åbner eksemplet "Tag- og vinduesudskiftning" og viser fire
måder at bruge grupperne på.

## Grupper er struktur
Grupperne styrer både, hvordan du inddaterer, og hvordan resultaterne kan
fordeles bagefter. Vælg den opdeling, der passer til det spørgsmål, du skal
svare på.

## Åbn et alternativ {#hovedmenu}
field: Forskudt renovering - trævinduer
action: click
wait: page=alternative

Klik på **Forskudt renovering - trævinduer** i sidemenuen.

## Kort i stedet for liste {#gruppe-listevisning}
action: type
value: false

Grupperne kan vises som liste eller som kort. Slå **Listevisning** fra — så
viser hvert kort gruppens egenskaber, også start- og slutår.

## 1. Efter fag eller entreprise {#grupper}
field: Vinduesudskiftning - nu

Eksemplet deler arbejdet op i byggeplads, vinduer og tag — det, der typisk
udbydes og udføres hver for sig. Så kan du se, hvad hver del koster over hele
levetiden.

## 2. Efter etape {#grupper}
field: Tagrenovering - om 10 år

Tagrenoveringen er udskudt: gruppen har **Start i år** 10, og alle dens rækker
arver startåret — tegltaget anskaffes i år 10, ikke i dag. Feltet **Udgår i
år** gør det modsatte: en gruppe kan stoppe, fx en midlertidig pavillon, der
fjernes i år 5, samme år som en tilbygning med Start i år 5 tager over.

## 3. Efter bygningsdel
placement: center

Standardskabelonen deler op efter SfB: ydervægge, tag, vinduer og så videre.
Men rækkerne bærer selv deres klassifikation, så visningen **Omkostninger
efter klassifikation** kan altid vise fordelingen på bygningsdele — uanset
hvordan grupperne er lavet. Grupperne er derfor frie til at fortælle noget
andet.

## 4. Efter hvem der betaler
placement: center

Grupper kan også følge pengene: bygherre, lejer og driftsorganisation hver for
sig, eller anlæg og drift. Så viser resultaterne, hvem der bærer hvilke
omkostninger over tid.

## Farve og ikon {#grupper}
field: Byggeplads - nu

Ikonet viser gruppens indhold og åbner gruppens egenskaber, og den lille
firkant nederst vælger farven. Skal en gruppe flyttes til et andet
alternativ, så brug listevisningen, hvor grupper kan klippes, kopieres og
indsættes.

## Grupperne i resultaterne {#hovedmenu}
field: Visninger

Under **Visninger** viser **Gruppeomkostninger** alternativets omkostninger
fordelt på netop de grupper, du har lavet.

## Færdig
Fag, etape, bygningsdel eller budget-ejer: vælg den opdeling, der svarer på
dit spørgsmål. Og husk, at start- og slutår på gruppen er den nemme vej til
etaper i tid.
