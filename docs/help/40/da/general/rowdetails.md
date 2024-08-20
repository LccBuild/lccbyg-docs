---

layout: lccbyghelp40  
title: "Posteringstyper"  
date: "2024-01-14"  

---

LCCbyg samler beregningsresultaterne i forskellige posteringer. En række vil, alt efter type, placere sine resultater i en eller flere af disse.

#### Anskaffelse

Posten 'Anskaffelse' indeholder anskaffelsesomkostningerne i dit projekt. Her skal du indtaste **levetid** og **anskaffelsespris** for den pågældende bygningsdel eller komponent. Levetiden angiver, hvor længe bygningsdelen forventes at holde, mens anskaffelsesprisen er den initiale omkostning. Derudover kan du angive **startår** og **slutår** for beregningsperioden, hvilket bestemmer, hvornår anskaffelsesomkostningen medregnes i beregningen. Du kan også tilføje eventuelle relevante bemærkninger i feltet "Bemærkninger".

#### Engangsudgift

Engangsudgifter konteres i det år, der er angivet i **startår**. Typisk vil engangsudgifter dække over omkostninger til byggeplads, honorarer til arkitekt, ingeniør og lignende, eller bygherreomkostninger. Startåret definerer det år, hvor udgiften påløber, og slutåret kan angives, hvis udgiften strækker sig over flere år.

#### Vedligehold

Posten for vedligeholdelse er delt i **årligt vedligehold** og **periodisk vedligehold**. Ved indtastning af årligt vedligehold angiver du et **interval**, som bestemmer, hvor ofte vedligeholdelsen skal udføres. Et interval på 1 betyder, at vedligeholdelsen sker hvert år. Du skal også angive en procentdel af anskaffelsesprisen, der årligt skal bruges på vedligehold. Hvis du ønsker at afsætte et specifikt beløb pr. gang, kan du indtaste dette i feltet for **kr./gang**. 

Ved periodisk vedligehold skal du ligeledes angive intervallet, som bestemmer, hvor ofte vedligeholdelsen skal gentages over årene. Her gælder det, at hvis intervallet er større end udskiftningsintervallet, udføres der ikke vedligehold, når udskiftning sker. 

#### Udskiftning

LCCbyg beregner omkostninger til udskiftning baseret på en angivet **udskiftningsprocent** af anskaffelsesomkostningen, typisk sat til 125 %. Denne procentdel kan justeres. Du skal også angive **levetid** og **startår** for beregningsperioden. Udskiftningen vil ske ved udløb af levetiden, og hvis startåret for udskiftningen overstiger beregningsperiodens slutår, vil udskiftningen ikke blive medtaget i beregningen. Eventuelle bemærkninger kan også tilføjes i dette afsnit.

#### Forvaltning

Forvaltning omfatter omkostninger som skatter og forsikringer. Her skal du indtaste **mængde**, **enhedspris**, samt **startår** og **slutår** for perioden, hvor disse omkostninger påløber. Forvaltningsomkostninger vil blive medregnet som en årlig udgift inden for den angivne periode.

#### Renhold

Renhold dækker over omkostninger til rengøring og anden vedligeholdelse, der udføres med en bestemt frekvens. Du skal indtaste **mængde**, og programmet bruger standardværdier for frekvens og enhedspriser. Hvis du ønsker at overskrive standardværdierne, kan du indtaste dem manuelt i den avancerede grænseflade. Udgifterne til renhold bliver medregnet årligt fra startår til slutår.

#### Løbende indtægt

Løbende indtægter kan stamme fra forsyningskilder som solceller eller vindmøller på ejendommen. Her kan du indtaste **mængde**, og programmet vil beregne den årlige indtægt baseret på den angivne enhedspris. Husk, at enhedsprisen skal have et positivt fortegn, da en negativ pris vil blive opfattet som en udgift. Indtægterne vil blive medregnet årligt fra startår til slutår.

#### Engangsindtægt

Engangsindtægter kan for eksempel opstå ved salg af bygningsdele til genbrug eller ved modtagelse af tilskud. Denne posteringstype registrerer indtægter, der kun sker én gang inden for den angivne periode. Du kan angive **startår**, og hvis indtægten skal gentages, kan du angive et interval.

 
