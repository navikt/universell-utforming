# Forstørring og responsive design

## Hvorfor det er viktig
For brukere med moderat nedsatt syn, er nettleserforstørring en enkel metode for å få større tekst på nettsiden. Er nettsiden responsivt, kan man lett både forstørre innholdet eller bruke sidene på mindre vindustørrelser, som på mobiltelefoner eller nettbrett.

## Teststeg
Automatiserte testverktøy kan simulere forskjellige skjermstørrelser og forstørret innhold på sider. Det kreves likevel alltid en manuell sjekk for å se om alt innhold er synlig og kan betjenes med tastatur:

### Vanlig nettleserzoom
1. Sett nettleseren til 1280px bredde, deretter bruk nettleserens zoomfunksjon (Ctrl og +/- eller Cmd og +/-) stegvis til 400 prosent. 
2. Sjekk at alt innhold og funksjonalitet er tilgjengelig og forståelig, i alle media-queries mellom 100 og 400 %. Det skal også være tilgjengelig når du bruker kun tastatur. Horisontalt skrolling bør unngås.
3. Sett forstørringen til 100 prosent, og endre vindusbredden på din nettleser gradvis fra fullskjerm og ned til det smaleste du får til. Se om rekkefølge, gruppering og generell layout fungerer godt i hele spekteret.

### Endring av skriftstørrelse på pc/mac
1. Forstørr fonten til 200 % (for eksempel i firefox med text-only zoom: view --> zoom --> text-only zoom)
2. Sjekk at alt innhold og funksjonalitet er tilgjengelig og forståelig. Det skal også være tilgjengelig når du bruker kun tastatur. Horisontalt skrolling bør unngås.

## Zoom på mobil
1. Forstørr fonten til 200 % (du kan [endre det i innstilingene på iPhone](https://support.apple.com/en-us/HT202828) eller direkte i safari)
2. Sjekk at alt innhold og funksjonalitet er tilgjengelig og forståelig.

<img src="/hvordan-faa-det-til/UU-testing/manuell-testing/zoom.jpeg" alt="zoom i safari i oppe venstre hjørne" style="max-width:50% />

## Text-spacing
1. Slå på text-spacing, for eksempel i ARC-toolkig (se under) eller med en [bookmarklet](http://www.html5accessibility.com/tests/tsbookmarklet.html).
2. Sjekk at alt innhold og funksjonalitet er tilgjengelig og forståelig, i alle media-queries mellom 100 og 400 %. Det skal også være tilgjengelig når du bruker kun tastatur. Horisontalt skrolling bør unngås.

## Verktøy du kan bruke
Bruk gjerne nettsiden [My viewport size (ekstern lenke, engelsk)](https://viewportsizes.com/mine/) for å sette vindusstørrelsen til spesifikke størrelser eller sjekke vindusstørrelsen når du oppdager problemer.

ARC toolkit tilbyr også en zoomfunksjon til 400%:, og det kan simulere text-spacing.

![zoom med ARC på nav.no](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/zoom-arc.png)

## Andre ressurser
- [Tilsynets veilednignssider om forstørring og zoom](https://www.uutilsynet.no/wcag-standarden/utforming-og-presentasjon/227#forstorring)
- [W3C - Unerstanding success criterion Reflow](https://www.w3.org/WAI/WCAG21/Understanding/reflow.html)
