---
title: "Vedligeholdsegnethed"
---

Vedligeholdsdashboardet er ét ark pr. alternativ: rosen med vurderingen af
vedligeholdsegnetheden og de vedligeholdstal, vurderingen fører til. Du
bruger det til at vise, hvorfor vedligeholdsprisen ligger, hvor den gør.
Svarene giver du på alternativets
[vedligeholdsvurdering](alternatives.md#vedligeholdsvalg).

### Vælg alternativer {#dashboard-alternativvalg}
Knappen bestemmer, hvilke alternativer der får et ark — samme valg som
"Medtag i grafer og rapporter" på
[alternativkortet](alternatives.md#alternativ-handlinger). Kun valgte
alternativer med "Brug vedligeholdsplan" slået til får et ark; er der ingen
af dem, siger siden det, og menupunktet er slået fra, indtil planen er slået
til et sted.

### Gem som billede {#dashboard-png}
Knappen gemmer arket som PNG i tredobbelt opløsning, så det holder til at
blive sat ind i et dokument. Filnavnet foreslås ud fra projektets og
alternativets navn.

### Arket {#dashboard-ark}
Øverst står projektets og alternativets navn samt året. Til venstre står
den bygningstype, alternativets vedligeholdsberegning peger på, og de tre
tal den giver: estimeret vedligeholdspris pr. m², årlig vedligeholdskost og
vedligeholdets nutidsværdi. Prisen findes ved at glide mellem bygningstypens
lave, midterste og høje pris fra
[vedligeholdsforudsætningerne](maintenanceprerequisites.md) efter
vurderingens samlede niveau.

### Rosen {#dashboard-rose}
Hvert felt er én spørgsmålsgruppe. Feltets bredde er gruppens vægt, og dets
længde og farve er gruppens niveau — fra "Meget lav" (grøn) inderst til
"Meget høj" (rød) yderst. Højt niveau trækker vedligeholdsprisen op.
Grupper med ubesvarede spørgsmål tegnes gennemsigtige og tæller som "Meget
høj", indtil de er besvaret. Midten viser det samlede niveau, og grupper,
du har taget ud af vurderingen, er ikke med i rosen.
