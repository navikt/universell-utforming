# Skjema

## Hvorfor det er viktig
Tilgjengelige skjema gir økt brukervennlighet for alle, men er spesielt viktig for brukere som benytter skjermlesere eller tastaturnavigasjon, og brukere med motoriske eller kognitive funksjonsnedsettelser (kilde: [uu.difi.no](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/skjema)).

## Teststeg
Automatiserte testverktøy kan teste nokså mye når det kommer til skjema, se også [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md). Det er fortsatt endel ting du må alltid teste manuelt:

1. Beskriver label (ledeteksten) formålet med skjemafeltet? Teksten skal være treffende, enkel og forståelig.
2. Er labelelementet koblet korrekt med skjemafelet?
3. Hvis bruker fyller ut skjemaet feil: Får brukeren en tekstlig beskrivelse av feilen og hvor feilen oppstår? Og konkrete forslag til løsning? Se gjerne [mønster for skjemavalidering i NAV](https://design.nav.no/patterns/form-validation)
4. Hvis et skjemafelt krever spesielt format: Er formatet spesifisert? Dette gjelder for eksempel dato, personnummer, telefon eller liknende.
5. Får brukerne mulighet til å bekrefte, kontrollere og/eller endre sine data i skjema med viktig formål? Dette kan for eksempel løses gjennom en oppsummeringsside som viser alt som er fylt ut, og der man kan gå tilbake og rette eventuelle feil.
6. Blir obligatoriske felt tydelig merket, og er markeringen forklart? Et * kan gjerne brukes, men forklar i begynnelsen av søknaden at dette er markeringen for obligatoriske felt.
7. Sjekk at farge ikke brukes som eneste virkemiddel for å formidle informasjon; for eksempel atn feil ikke bare markeres med farge.


Vær obs når det skjer kontekstendringer

8. Når et skjemaelement får fokus: Skjer det  kontekstendring? (forventet resultat: nei)
9. Ved utfyllelse av skjema: Skjer det automatisk kontekstendring (Unntak: Ok, dersom brukeren blir varslet om det før bruk av komponenten)(forventet resultat: nei)

## Verktøy du kan bruke
Kjør gjerne automatiserte test først. Utover det kan for eksempel ARC toolkit identifisere skjemaelement og hvordan de er kodet:

![skjemavisning i ARC toolkit](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/skjema.png)

## Andre ressurser
* Kontekstendringer - suksesskriterie [3.2.1 Fokus](https://uu.difi.no/krav-og-regelverk/wcag-20-standarden/321-fokus-niva) og 
[3.2.2 Inndata](https://uu.difi.no/krav-og-regelverk/wcag-20-standarden/322-inndata-niva)
* [Lær mer om hvordan teste skjema på Tilsynets veiledningssider.](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#skjema)

