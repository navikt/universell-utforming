# Skjema

## Hvorfor det er viktig
Tilgjengelige skjema gir økt brukervennlighet for alle, men er spesielt viktig for brukere som benytter skjermlesere eller tastaturnavigasjon, og brukere med motoriske eller kognitive funksjonsnedsettelser (kilde: [uutilsynet.no](https://www.uutilsynet.no/wcag-standarden/skjema/38)).

## Teststeg
Automatiserte testverktøy kan teste nokså mye når det kommer til skjema, se også [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md). Det er fortsatt endel ting du må alltid teste manuelt:

1. Beskriver label (ledeteksten) formålet med skjemafeltet? Teksten skal være treffende, enkel og forståelig.
2. Er labelelementet koblet korrekt med skjemafelet?
3. Hvis bruker fyller ut skjemaet feil: Får brukeren en tekstlig beskrivelse av feilen og hvor feilen oppstår? Og konkrete forslag til løsning? Se gjerne [mønster for skjemavalidering i NAV](https://design.nav.no/patterns/form-validation)
4. Hvis et skjemafelt krever spesielt format: Er formatet spesifisert? Dette gjelder for eksempel dato, personnummer, telefon eller liknende.
5. Får brukerne mulighet til å bekrefte, kontrollere og/eller endre sine data i skjema med viktig formål? Dette kan for eksempel løses gjennom en oppsummeringsside som viser alt som er fylt ut, og der man kan gå tilbake og rette eventuelle feil.
6. Blir obligatoriske felt tydelig merket, og er markeringen forklart? Eller er alterntivt valgfrie felt markert? Se våre [retningslinjer på design.nav.no](https://design.nav.no/components/input/accessibility) 
7. Sjekk at farge ikke brukes som eneste virkemiddel for å formidle informasjon; for eksempel at feil ikke bare markeres med farge.
8. Sjekk at lengden på input-felt speiler forventet input. For eksempel 11-siffer lang inputfelt for fødselsnummer. Se veiledning på [siden om input-felt](https://design.nav.no/components/input#lengde)


Vær obs når det skjer kontekstendringer

9. Når et skjemaelement får fokus: Skjer det  kontekstendring? (forventet resultat: nei)
10. Ved utfyllelse av skjema: Skjer det automatisk kontekstendring (Unntak: Ok, dersom brukeren blir varslet om det før bruk av komponenten)(forventet resultat: nei)

## Verktøy du kan bruke
Kjør gjerne automatiserte test først. Utover det kan for eksempel ARC toolkit identifisere skjemaelement og hvordan de er kodet:

![skjemavisning i ARC toolkit](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/skjema.png)

## Andre ressurser
* Kontekstendringer - suksesskriterium [3.2.1 Fokus](https://www.uutilsynet.no/wcag-standarden/321-fokus-niva/112) og 
[3.2.2 Inndata](https://www.uutilsynet.no/wcag-standarden/322-inndata-niva/114)
* [Lær mer om hvordan teste skjema på Tilsynets veiledningssider.](https://www.uutilsynet.no/regelverk/sjekk-nettstedet-ditt-selv/708#7_skjema)
* [Retningslinjer for disabled-attributet på design.nav.no](https://design.nav.no/accessibility/disabled)
* [Retningslinjer for placeholder på design.nav.no](https://design.nav.no/accessibility/placeholders)
