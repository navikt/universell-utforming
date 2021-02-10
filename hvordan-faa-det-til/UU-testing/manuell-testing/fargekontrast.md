# Farge og kontrast

## Hvorfor det er viktig
God kontrast mellom tekst og bakgrunn er særlig viktig for brukere med nedsatt syn, lesevansker og nedsatt kognisjon, og for alle brukere under krevende lysforhold. I tillegg er det viktig at farge ikke er den eneste måten å formidle informasjon på med tanke på nedsatt fargesyn. (kilde: [uutilsynet.no](https://www.uutilsynet.no/regelverk/sjekk-nettstedet-ditt-selv/708#3_farger_og_kontrast)

## Teststeg
De fleste automatiserte verktøyene tester for fargekontrast. Se gjerne [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md) der vi viser hva SortSite, ARC Toolkit og W3C kodejsekker tester.

En del må likevel testes manuelt:

1. Har du brukt [designsystemet og NAV frontend](https://design.nav.no/resources/colors)?
2. Er det tilstrekkelig kontrast mellom tekst og bakgrunn? (kan stort sett testes automatisert, se nedenfor under "automatisert testing")
3. Er klikkbare elementer markert med mer enn bare farge?
4. Er brukeren avhengig av å kunne se farge (eller form) for å forstå innholdet? Refereres det for eksempel til "den blåe knappen" eller "bildet til høyre"? Gjelder også diagrammer som baserer seg på farge. Se [Tilsynets veileder for farge](https://www.uutilsynet.no/regelverk/bruk-av-farger/206).

### Vær obs på følgende: 
NAV har som mål å levere tjenester som har kontrastnivå på AAA-nivå. Designsystemet er stadig i forbedringer. Til nå er kontrasten godkjent når den møter kontrastforhold 4,5:1 (AA-nivå i WCAG). Bruk gjerne høyere kontrast. Du finner kontrastforhold mot forskjellige farger i detaljevisningen av fargene på https://design.nav.no/resources/colors.

![Fargekontrastene på designsystemfarger](/hvordan-faa-det-til/UU-testing/manuell-testing/kontrast.png)

Inaktive funksjoner bør unngås da de ofte har svært lav kontrast og ikke sees av alle. Er det noe vi ønsker å kommunisere må disse komponentene være tilgjengelig for alle. Se også https://design.nav.no/accessibility/disabled

## Verktøy du kan bruke
Noen rene kontrastsjekkere:
* [Color Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/)
* [Snook.ca](https://snook.ca/technical/colour_contrast/colour.html#fg=FFFFFF,bg=000000)

## Andre ressurser
* [Lær mer om hvordan teste farger og kontraster på Tilsynets veiledningssider](https://www.uutilsynet.no/regelverk/sjekk-nettstedet-ditt-selv/708#3_farger_og_kontrast)
* [Tilsynets veiledningsside om kontrast](https://www.uutilsynet.no/wcag-standarden/kontrast/48)
* [Tilsynets veiledningsside om farge](https://www.uutilsynet.no/regelverk/bruk-av-farger/206)
