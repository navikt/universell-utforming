# Fargekontrast

## Hvorfor det er viktig
God kontrast mellom tekst og bakgrunn er særlig viktig for brukere med nedsatt syn, lesevansker og nedsatt kognisjon, og for alle brukere under krevende lysforhold. I tillegg er det viktig at farge ikke er den eneste måten å formidle informasjon på med tanke på nedsatt fargesyn. (kilde: [uu.difi.no](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#farger-og-kontrast))

## Teststeg

1. Har du brukt [designsystemet og NAV frontend(https://design.nav.no/resources/colors)]?
2. Er det tilstrekkelig kontrast mellom tekst og bakgrunn? 
3. Er klikkbare elementer markert med mer enn bare farge?
4. Er brukeren avhengig av å kunne se farge (eller form) for å forstå innholdet? Refereres det for eksempel til "den blåe knappen" eller "bildet til høyre"?

### Vær obs på følgende: 
NAV har som mål å levere tjenester som har kontrastnivå på AAA-nivå. Designsystemet er stadig i forbedringer. Til nå er kontrasten godkjent når den møter kontrastforhold 4,5:1 (AA-nivå i WCAG). Bruk gjerne høyere kontrast. Du finner kontrastforhold mot forskjellige farger i detaljevisningen av fargene på https://design.nav.no/resources/colors.

Inaktive funksjoner bør unngås da de ofte har svært lav kontrast og ikke sees av alle. Er det noe vi ønsker å kommunisere må disse komponentene være tilgjengelig for alle. Se også https://design.nav.no/accessibility/disabled


## Automatisert testing
De fleste automatiserte verktøyene tester for fargekontrast. 

Noen rene kontrastsjekkere:
* [Color Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/)
* [Snook.ca](https://snook.ca/technical/colour_contrast/colour.html#fg=FFFFFF,bg=000000)

## Andre ressurser
* [Lær mer om hvordan teste farger og kontraster på Tilsynets veiledningssider](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#farger-og-kontrast)
* [Tilsynets veiledningsside om kontrast](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/kontrast)
