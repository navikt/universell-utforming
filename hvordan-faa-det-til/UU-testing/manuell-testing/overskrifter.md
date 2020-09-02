# Overskrifter

## Hvorfor det er viktig
Overskrifter gjør det lettere å orientere seg på siden. Mange brukere "skanner" siden etter overskrifter og lenker, for å se om de er på riktig side og finner svar på det de lurer på. Riktig koding på overskriftene er spesielt viktig for brukere av opplesningsverktøy, både for orientering og navigering på siden.

![Overskriftsliste fra VoiceOver på nav-side](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/overskriftsliste.png)

## Teststeg
Dette må du alltid teste manuelt:

1. Er innholdet på siden organisert ved hjelp av overskrifter, og der passende med underoverskrifter? 
2. Er all tekst som ser ut som overskrifter også kodet med overskriftstag (<h*>) 
3. Dersom en overskrift er del av et visuelt overskriftshierarki, må du sjekke om den er kodet med samme nivå som den visuelle overskriften. Det vil si er overskrift som visuelt på nivå to også kodet som nivå 2? Det bør ikke hoppes over overskriftsnivåer.
4. Beskriver overskriftene innholdet på siden? Sjekk både overskrifter og ledetekster i skjema og tabeller.  

## Verktøy du kan bruke
Det er en del testregler på overskrifter som dekkes av automatiserte verktøy, se også [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md) der vi viser hva SortSite, ARC Toolkit og W3C tester.

For å se Overskriftshirarki og -rekkefølge kan du bruke forskjellige verktøy, som for eksempel [Web Developer Toolbar for Chrome (lenke til download)](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=no):

![WebDeveloperToolbar](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/webdevelopertoolbar.png)

Document Outline Web Developer Toobar genererer:

![Document Outline fra WebDeveloperToolbar](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/docoutline.png)

Hvis du bare ønsker å se hva som er en overkrift på siden og med hvilket nivå, kan du også bruke ARC toolkit. Husk at du på denne måten ikke kan sjekke om overskriftene er på riktig nivå, siden du ikke ser rekkefølgen og hirarkiet.

![ARC overskrifter](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/headings-arc.png)

## Andre ressurser
* [Lær mer om hvordan teste overskrifter på Tilsynets veiledningssider.](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#overskrifter)

