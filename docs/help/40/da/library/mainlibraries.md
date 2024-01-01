---
layout: lccbyghelp40
title: "Bibliotek"
date: "2024-01-01"
---

I LCCBygs bibliotek findes kontoplaner, der kan anvendes til at opbygge din beregning. Kontoplanerne indeholder forskellige rækker, der hver er af en bestemt rækketype med tilhørende nøgletal. I biblioteket kan man kun læse værdierne, det er ikke muligt at redigere dem.

<br />

### Kontoplaner
Som udgangspunkt vises alle rækker i biblioteket, men du kan også vælge kun at få vist rækkerne i en af kontoplanerne. Det gør du ved at vælge en af følgende kontoplaner i fanebladsmenuen:

<ul>
<li>Bygningsdele</li>
Alle standardskabeloner har kontoplanen 'Bygningsdele'. Bygningsdelene er baseret på <a href="https://lccbyg.dk/levetidstabel2021/" target="_blank">BUILD's levetidstabel</a>, der er bygget over SfB-klassifikationssystemet. I kontoplanen kan man både vælge rækker på et overordnet niveau ( kode 1, 2, 3 etc.) på mellem niveau ( kode 1.x, 2,x , 3. x etc) og på konstruktionsniveau ( kode 1.3.23 etc.)
  
<li>Andre nøgletal</li> 
Denne kontoplan indeholder nøgletal for henholdsvis 'Grund, rådgivning og bygherre', 'Forvaltning', 'Forsyning' og 'Renhold'.

<li>Bygningstyper</li> 
Denne kontoplan indeholder nøgletal for forskellige bygningstyper. Nøgletalene er defineret på baggrund af <a href="https://lccbyg.dk/levetidstabel2021/" target="_blank">BUILD's levetidstabel</a>. Bygningstyperne er opbygget efter seneste udgave af BBR-koderne fra maj 2020.

<li>Opgaver</li> 
Denne kontoplan er udformet med udgangspunkt i 20-punkts listen for typiske drifts- og vedligeholdsplaner for ejerboligforeninger og andelsboligforeninger. Du kan læse mere om de forskellige aspekter og bygningskomponenter under <a href="https://lccbyg.dk/videnskilder/" target="_blank">her</a>.

<li>Tomme rækker</li> 
Denne kontoplan er speciel derved, at den inholder en tom række uden nøgletal for hver rækketype. Dem kan du anvende, hvis du ikke kan finde en prædefineret række, der passer til dit behov.
</ul>


Yderst til højre i fanebladsmenuen vises et symbol med blå baggrund og et hvidt '+'-tegn. Har du et større datasæt med nøgletal, som du ønsker at basere dine beregninger på, kan du tilføje dem til biblioteket.  Klik på '+'-tegnet for at importerer en skabelon med egne rækker og nøgletal i biblioteket fra en fil. Når filen er indlæst, bliver der tilføjet et nyt faneblad i fanebladsmenuen.

<br />

### Navigering i kontoplanerne
I nogle af kontoplanerne bliver der ud over tabellen med rækker også vist en menustruktur til venstre i fanebladet. Her kan du navigere endnu længere ned i den valgte kontoplan og finde netop den eller de rækker, som svarer til dit behov.

Du kan åbne en række ved at klikke på '>'-symbolet og dermed få vist de nøgletal, som rækken indeholder.  Klik igen på '>'-symbolet for at lukke rækken. 

I hver række vises desuden et ikon, så du kan se, hvilken rækketype den enkelte række repræsenterer.

Nogle rækker har flere varianter. Det er angivet med 'Pil ned'-symbolet i feltet 'Variant'. Klik i feltet og vælg den variant, som som svarer til dit behov.

<br />

### Sorteringsfunktionen
Det er muligt at angive, hvilket felt rækkerne skal sorteres efter. Flyt markøren ind i det ønskede felt i tabellens titellinje. Nu fremokmmer et 'Pil'-symbol i feltet. Klik i feltet for at vælge stigende sortering ('Pil op'-symbol vises). Klik igen i feltet, hvis du ønsker faldende sortering ('Pil ned'-symbol vises).Det fremkomne 1-tal til højre for 'pil'-symboletsymbolet indikerer, at feltet nu er bestemmende for sorteringsrækkeføljen.

Det desuden muligt at tilføje flere felter som rækkerne skal sorteres efter i prioriteret rækkefølje. Flyt markøren ind i et nyt felt i titellinjen. Når 'Pil'-symbolet vises skal du holde Ctrl-tasen nede og klikke i feltet. Nu fremkommer et 2-tal til højre for 'pil'-symboletsymbolet. Rækkerne bliver nu først sorteret efter kolonnen markeret med et 1-tal og derefter sorteret efter kolonnen markeret med et 2-tal. Fremgangsmåden kan gentages indtil alle kolonner er markeret med et fortløbende tal.

Sorteringen for et felt kan fravælges ved at flytte markøren ind i feltet, klikke på kebab-symbolet med de 3 lodrette prikker og vælge 'Usortér'.

<br />

### Søgefunktionen
I søgefeltet lige over fanebladsmenuen er det muligt at søge efter bestemte rækker i hele biblioteket. 

Hvis du ønsker at begrænse din søgning til rækker af en bestemt type så klik på 'Rækketype' og vælg den ønskede rækketype. 

I søgefeltet kan du både søge på tekst og på koder.

Husk at slette teksten i søgefeltet og fravælge den valgte rækketype, når du ikke længere ønsker at begrænse din søgning.

> TIPS
<ul>
<li>Rækker med CO<sub>2</sub>/GWP findes under 'Bygningstyper' og under 'Andre nøgletal' > 'Forsyning'</li>

<li>Rækker med priser findes under 'Opgaver' og under 'Andre nøgletal' > 'Renhold'</li>

<li>Det er ikke alle rækker der indeholder priser, men alle rækker har vedligeholds- og genopretningsprocenter</li>
</ul>

<br />

### Rækketyper
I LCCbyg er der 8 forskellige rækketyper:
<ul>
<li>Anskaffelse</li>
  Benyttes til anskaffelse af materiel til byggeprojektet, som ikke er bygningsdele. Fx. posteres grundkøb som en anskaffelse.
<li>Engangsudgift</li>
  Benyttes til postering af engangsudgifter. Dette kan fx. være honorarer til arkitekter og ingenører eller udgifter til byggeplads.
<li>Bygningsdel</li>
  Benyttes til anskaffelse af bygningsdele og bygningstyper. Det vil sige, at denne rækketype benyttes til byggematerialer.
<li>Forvaltning</li>
  Benyttes til postering af løbende udgifter. Dette kan eksempelvis være løbende administrationsudgifter, ejendomskat, dækningsafgifter eller forsikringer.
<li>Forsyning</li>
  Benyttes til at postere de løbende udgifter til forsyning af dit byggeprojekt, herunder varme, el og vandforbrug.
<li>Renhold</li>
  Benyttes til postering af de løbende udgifter, der er til renhold af dit byggeri. Det kan fx. være vinduespudsning, gulvvask eller snerydning.
<li>Løbende indtægt</li>
  Benyttes til postering af de løbende indtægter dit byggeri har. Det kan fx. være solcellestrøm, vindmøllestrøm eller solvarmeanlæg.
<li>Engangsindtægt</li>
  Benyttes til postering af de individuelle indtægter, der falder i løbet af beregningsperioden. Dette kan fx. være scrap-værdi for salg af bygningsdele, der ikke længere benyttes.
</ul>
Rækketypen afgør, hvordan der regnes og hvor resultaterne bliver posteret.

<br />
<br />

### Posteringstyper
Der findes 10 forskellige posteringstyper:
<ul>
<li>Anskaffelse</li>
<li>Genanvendelse</li>
<li>Engangsudgift</li>
<li>Vedligehold</li>
<li>Udskiftning</li>
<li>Forvaltning</li>
<li>Forsyning</li>
<li>Renhold</li>
<li>Løbende indtægt</li>
<li>Engangsindtægt</li>
</ul>
