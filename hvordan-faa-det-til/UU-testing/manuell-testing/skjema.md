# Skjema

## Hvorfor det er viktig
Tilgjengelige skjema gir økt brukervennlighet for alle, men er spesielt viktig for brukere som benytter skjermlesere eller tastaturnavigasjon, og brukere med motoriske eller kognitive funksjonsnedsettelser (kilde: [uu.difi.no](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/skjema)).

## Teststeg

Automatiserte testverktøy kan teste nokså mye når det kommer til skjema, se også [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md). Det er fortsatt endel ting du må alltid teste manuelt:

1. Beskriver label (ledeteksten) formålet med skjemafeltet? 
2. Er labelelementet koblet korrekt med skjemafelet?
3. Hvis en inndatafeil blir oppdaget automatisk: Får brukeren en tekstlig beskrivelse av feilen og hvor feilen oppstår
4. Hvis et skjemafelt krever spesielt format: Er formatet spesifisert?
5. Hvis bruker fyller ut skjemaet feil: Får brukeren en feilmeldingmed konkrete forslag til løsning?
6. Får brukerne mulighet til å bekrefte, kontrollere og/eller endre sine data i skjema med viktig formål? 


Vær obs når det skjer kontekstendringer

7. Når et skjemaelement får fokus: Skjer det  kontekstendring? (forventet resultat: nei)
8. Ved utfyllelse av skjema: Skjer det automatisk kontekstendring (Unntak: Ok, dersom brukeren blir varslet om det før bruk av komponenten)(forventet resultat: nei)

## Verktøy du kan bruke


## Andre ressurser
* Kontekstendringer - suksesskriterie [3.2.1 Fokus](https://uu.difi.no/krav-og-regelverk/wcag-20-standarden/321-fokus-niva) og 
[3.2.2 Inndata](https://uu.difi.no/krav-og-regelverk/wcag-20-standarden/322-inndata-niva)
* [Lær mer om hvordan teste skjema på Tilsynets veiledningssider.](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#skjema)

