# Bilder, illustrasjoner og ikoner

## Hvorfor det er viktig
Å kommunisere et budskap i form av noe annet enn kun tekst kan gi en god brukeropplevelse for de fleste, være det kan være spesielt nyttig for dyslektikere og for personer som har norsk som andrespråk. Gjennom bilder kan man få en bekreftelse på at man har forstått budskapet i teksten. 
Det er likevel viktig å huske at ikke alle kan se bildene, enten på grunn av dårlig syn eller dårlig nettverk. Noen kan også ha utfordringer med å forstå (komplekse) bilder og illustrasjoner. Bilder med bevegelser og animasjoner kan distrahere, og blinkende bilder kan utløse epileptiske anfall.

## Teststeg
Automatiserte testverktøy kan sjekke at det finnes et tekstalternativ for bildet, en såkalt alt-tag ( alt=»illustrasjosbilde av...»), men kun du kan sjekke kvaliteten på beskrivelsen.  

Dette må du alltid teste manuelt:

### 1. Identifiser: 
* Finnes det bilder på siden du tester?
* Er bildene på siden kun dekorasjon, eller blir de brukt til å kommunisere innhold eller funksjonalitet?  

**Med bilder menes:** Foto, ikoner, illustrasjoner, grafer, dekorativ grafikk og tegninger.

**Dekorasjon:**  Innhold som kun har et estetisk formål, som ikke inneholder informasjon eller funksjonalitet. 

### 2. Finnes det en alternativ tekst for meningsbærende bilder?
1. Alt-teksten skal være et reelt alternativ for personer som ikke ser. 

  * alt="Kim Daniel Skogstad i en XXL-butikk, kledd i XXL-genser" (teksten under bildet ligger på siden som tekst) ![meningsbærende bilde](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/alt-xxl.png) 
  * OBS! Hvis bildet formidler samme informasjon som (HTML-)tekst i nærheten, skal alt-teksten være tom, for å unngå at samme informasjon gis to ganger. Her viser bildet en dame på telefon foran en laptop, som skal vise at man kan ringe eller chatte. Samme informasjon står som ren tekst rett ved siden av bildet ("Ring eller chat med oss om økonomi"). Å gjenta dette kan oppfattes som støy, og gir ikke noen nyttig ekstra-informasjon. Bildet skal derfor ha et tomt alt-attributt.

![meningsbærende bilde med tekst ved siden av](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/alt-ringchat.png). 

2.  Bilder av text skal ha en alt-tekst som inkluderer teksten i bildet, hvis ikke samme tekst står i HTML-teksten rett ved siden av bildet. Bilder av tekst bør unngås, men vi bruker det for eksempel i logoen.
3. Har bilder som kommuniserer innhold eller funksjonalitet en alternativ tekstbeskrivelse? For eksempel innlogging i ID-porten eller forstørrelsesglass for søk.
4. Er alt-teksten på samme språk som hovedinnholdet på siden? 

### 3. Er dekorativ grafikk er kodet korrekt og på den måten skjult for skjermleserne? 
For eksempel et bakgrunnsbilde med CSS, eller er de kodet med alt="", role="presentation" eller lignende.
  
### 4.Bilder med kompleks informasjon  
For eksempel grafer, tabeller og bilder med tekst. 

Bruk alt-tekst som beskriver motivet i bildet OG en tekst med detaljert informasjon om innholdet i motivet. Teksten skal enten ligge på samme side, eller man kan legge inn en lenke som tar deg til en side hvor man kan nå tekstbeskrivelsen. I noen tilfeller er det best å tilby visning som tabell. 

- alt="Tar du for eksempel 2 uker ferie i foreldrepengerperioden, forskyves sluttdatoen med 2 uker. Skjematisk illustrasjon" 

![Illustrasjon om foreldrepengeplanlegging](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/alt-foreldrepengerplanlegging.png)
- Eksempel på en graf som alternativ bør kunne vises som tabell. alt="Oversikt over arbeidsledige og ledige stillinger de siste 13 måneder." 

![Graf over ledighet](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/alt-ledighet.png)

### 5. Bilder med lenker: 
* Har bilder med lenker en tydelig markering ved tastaturnavigasjon og når du fører muspekeren over bildet? 
* Er alt-teksten beskrivende for siden du kommer til? 
* Åpner lenken en ny fane, vindu eller et program? I såfall må du sjekke om du har fått informasjon om dette før du trykker på lenken. 

## Verktøy du kan bruke
* ARC toolkit kan vise hvilke bilder som er kodet med &lt;img&gt;

## Andre ressurser
* [Lær mer om hvordan teste bilder på Tilsynets veiledningssider.](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#bilder)
* [Informasjonsside om alternative tekster på Designsystem-sidene](https://design.nav.no/accessibility/alt-text)


