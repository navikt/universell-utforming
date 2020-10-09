# Hvilket verktøy er best?

Her skal vi legge ut en sammenlikning mellom hva som testes med SortSite, ARC toolkit og W3Cs kodesjekker.

<alertstripe type="advarsel">Denne siden er ikke ferdig enda. Inntil videre finner du den fullstendige oversikten på <a href="https://confluence.adeo.no/display/MEBO/Automatisert+testing">NAV-intern Confluence-side</a>.</alertstripe>



## Bilder

### Det verktøyene tester på bilde
<table>
  <caption>Automatisert test av bilder</caption>
  <tr>
    <th scope="col">Test</th>
    <th scope="col">SortSite</th>
    <th scope="col">ARCToolkit</th>
    <th scope="col">W3Cs kodesjekker</th>
    <th scope="col">Siteimprove (ikke testet enda)</th>
    <th scope="col">TECH</th>
    <th scope="col">WCAG</th>
  </tr>
  <tr>
    <th scope="row">Alt-teksten skal ikke være et filnavn, eller inneholder ord som <lang="en">picture, spacer, graphic, icon, iage, thumnail, spacer</lang></th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F30.html">F30</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">AREA-elementer må ha et ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">IMG-elementer uten ALT-Attribute skal ikke ha Title eller ARIA-Label-Attributes</th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2010/WD-WCAG20-TECHS-20100708/F39">F39</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
   <tr>
    <th scope="row">IMG-elementer må ha en ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
     <tr>
    <th scope="row">Input TYPE = IMAGE må ha et beskrivende ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">ALT-tekst skal ikke bruke ASCII ART (inkluderer Smileys)</th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">BUTTON-elementer som bare inneholder en IMG skal ha et ALT-attribute for bildet</th>
    <td>✅</td>
    <td>❌</td>
    <td>✅</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">Alt-teksten er lik lenketeksten. Dette fører til at skjermlesen leser opp samme teksten to ganger. Dette ønsker vi å unngå. Bruk Alt="" evt. annen teknikk.</th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/H2.html">H2</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a>, <a href="https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html">2.4.4</a>, <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-link.html">2.4.9</a></td>
  </tr>
  <tr>
    <th scope="row">Dekorasjonsbilder (og Spacer images) skal ikke alt-tekst. Dokumentasjonen sier at SortSite tester dette....</th>
    <td>ℹ️</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2010/WD-WCAG20-TECHS-20100708/F39">F39</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1</a></td>
  </tr>
</table>

### Det verktøyene ikke tester på bilder

Se gjerne <a href="/hvordan-faa-det-til/UU-testing/manuell-testing/bilder.md">vår veileder for manuell test på bilder</a>.

#### Om bildene inneholder kompleks informasjon

For eksempel:

- graf
- tabeller
- plakat med tekst

Denne typen bilder skal ha et mer utfyllende alternativtekst.

Teksten skal enten ligge på samme side eller man kan legge inn en lenke som tar deg til en side hvor man kan nå tekstbeskrivelsen.

####  Om bilder med lenker:
- får tydelig fokusmarkering ved tastaturnavigasjon eller ved å føre muspekeren over bildet.
- har en alt-tekst som beskriver siden du kommer til.
- åpnes i en ny fane, vindu, program e.
- Får du info om dette før du klikker på lenken?

#### Om bildene er dekorasjon eller meningsbærende
Vi får kun et hint om at et bilde kan være dekorasjon dersom vi tilfeldigvis har brukt følgende engelske ord i alt-tekste: picture, spacer, graphic, icon, thumnail eller spacer.

#### Om bildet inneholder tekst
Oppdager ikke bilde av tekst, og om alternativteksten gjengir innholdet i bildet på en god måte.

#### Om alt-teksten er villedende
Krever manuell vurdering

#### Om Aria-labelledby fungerer for alle brukerne våre. 
I følge dokumentasjonen til SortSite fungerer ikke Aria-labelledby for alle skjermlesere.

#### Om Aria-describedby er blir brukt som et alternativ til alt-tag

## Struktur

### Det verktøyene tester på struktur

<table>
  <caption>Automatisert test av struktur</caption>
  <tr>
    <th scope="col">Test</th>
    <th scope="col">SortSite</th>
    <th scope="col">ARCToolkit</th>
    <th scope="col">W3Cs kodesjekker</th>
    <th scope="col">Siteimprove (ikke testet enda)</th>
    <th scope="col">TECH</th>
    <th scope="col">WCAG</th>
  </tr>
  <tr>
    <th scope="row">Sidetittel. Nettsiden har en <title> som beskriver den aktuelle sidens emne eller formål.</th>
    <td>✅</td>
    <td>❌</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/H25.html">H25</a></td>
    <td><a href"https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-title.html">2.4.2</a></td>
  </tr>
  <tr>
    <th scope="row">Line break (&lt;br&gt;) skal ikke benyttes for å formatere avsnitt (&lt;p&gt;)</th>
    <td>❌</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <th scope="row">Språk. Siden mangler lang attribute . (lang=....)</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-doc-lang-id.html">3.1.1</a></td>
  </tr>
   <tr>
    <th scope="row">Kodefeil (markup errors) (MLT, Heading should not bee empty linje 10, p001)</th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-parses.html">4.1.1</a></td>
  </tr>
</table>

### Det verktøyene ikke tester på struktur
- Om sidetittelen gir relevant beskrivning av emne eller formål med siden (sk 2.4.2, tech G88 og F25)
- Om sidetittelen inneholder tekst som "Untitled" eller filnavnet (WAVE)

## Farger / kontrast

### Det verktøyene tester på farge og kontrast

<table>
  <caption>Automatisert test av farge og kontrast</caption>
  <tr>
    <th scope="col">Test</th>
    <th scope="col">SortSite</th>
    <th scope="col">ARCToolkit</th>
    <th scope="col">W3Cs kodesjekker</th>
    <th scope="col">Siteimprove (ikke testet enda)</th>
    <th scope="col">TECH</th>
    <th scope="col">WCAG</th>
  </tr>
  <tr>
    <th scope="row">Tekst og bakgrunn har god nok kontrast.</th>
    <td>❌</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html">1.4.3</a></td>
  </tr>
  <tr>
    <th scope="row">Tekst og bakgrunn har en kontrast på 7:1</th>
    <td>❌</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast7.html">1.4.6 (AAA)</a</td>
    <td></td>
  </tr>
  <tr>
    <th scope="row">Alt-teksten skal ikke inneholder farger. Antagelse: SortSite sjekker kun engelske ord (f.eks <lang="en">red, blue..</lang>)</th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">1.1.1 </a></td>
  </tr>
</table>

### Det verktøyene ikke sjekker på farge og kontrast
- Om kontrasten mellom tekst og bakgrunn 7:1
- Om alt-teksten inneholder farger
- Om siden inneholder kun farger og fargekombinasjoner som er godkjent og del av designsystemet

## Overskrifter
<table>
  <caption>Automatisert test av overskrifter</caption>
  <tr>
    <th scope="col">Test</th>
    <th scope="col">SortSite</th>
    <th scope="col">ARCToolkit</th>
    <th scope="col">W3Cs kodesjekker</th>
    <th scope="col">Siteimprove (ikke testet enda)</th>
    <th scope="col">TECH</th>
    <th scope="col">WCAG</th>
  </tr>
  <tr>
    <th scope="row">Finnes det tomme overskriftstagger på siden( &lt;h*&gt;&lt;/h*&gt;)?</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html">2.4.6 </a></td>
  </tr>
  <tr>
    <th scope="row">Har overskriftsnivåene korrekt rekkefølge?</th>
    <td>❌</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1 (AAA)</a></td>
  </tr>
  <tr>
    <th scope="row">Overskrifter skal ikke inne holde andre overskrifter.</th>
    <td>❌</td>
    <td>❌</td>
    <td>✅</td>
    <td>?</td>
    <td></td>
    <td></td>
  </tr>
   <tr>
    <th scope="row"><lang="en">Use HTML headings instead of applying CSS heading styles to non-headings.</lang></th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F2.html">F2</a></td>
    <td></td>
  </tr>
</table>

### Det verktøyene ikke tester på overskrifter
- Om innholdet på siden organisert ved hjelp av overskrifter, og hvis hensiktsmessig underoverskrifter?
- Om overskriften inngår i et visuelt overskriftshierarki og om den da er kodet med samme nivå som den visuelle overskriften
- Om all tekst som ser ut som overskrifter, kodet med overskriftstag (&lt;h*&gt;) 1.3.1
- Beskriver overskriftene innholdet? 2.4.6

(NB! Skjema og tabeller har også overskrifter/ledetekster. Disse må også evalueres)

## Lenker

### Det verktøyene tester på lenker
Hverken SortSite, ARCToolkit eller W3Cs kodesjekker tester lenker automatisk. Siteimprove har noen muligheter, vi oppdaterer når vi har testet Siteimprove nærmere.

### Det verktøyene ikke tester på lenker
- Om lenker er fremhevet med noe mer enn bare farge 1.4.1
- Om brukeren forstår hva som skjer når du trykker på lenken
- Om lenker er plassert i som f.eks et ord i en setning eller et avsnitt.
- Om det kommer tydelig fram ut fra teksten, lenketeksten og lenkonteksten sammen, hva som er lenkens mål og funksjon (2.4.4.)
- Om det interne lenker er brutt

## Tabeller

### Det verktøyene tester på tabeller

<table>
  <caption>Automatisert test av tabeller</caption>
  <tr>
    <th scope="col">Test</th>
    <th scope="col">SortSite</th>
    <th scope="col">ARCToolkit</th>
    <th scope="col">W3Cs kodesjekker</th>
    <th scope="col">Siteimprove (ikke testet enda)</th>
    <th scope="col">TECH</th>
    <th scope="col">WCAG</th>
  </tr>
  <tr>
    <th scope="row">Kompleks tabell. Krever manuell verifisering</th>
    <td>✅ Sjekker for tabeller som har to eller flere nivåer med overskrifter og <lang="en">nested tables</lang></td>
    <td>✅ Sjekker for <lang="en">table nested in non-layout table</lang></td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F49.html">F49</a></td>
    <td><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-programmatic.html">1.3.1</a></td>
  </tr>
  <tr>
    <th scope="row">Layout-tabeller skal ikke ha SUMMARY eller CAPTION. En tabell som mangler th kan se ut som en layout-tabell.
</th>
    <td>✅</td>
    <td>✅ Tabeller ska ikke kodes med både Role="presentation" og (&lt;th&gt;,&lt;caption&gt; eller &lt;summary&gt;). (Krever manuel verifisering)</td>
    <td>x</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F46.html">F46</a></td>
    <td></td>
  </tr>
  <tr>
    <th scope="row">Tabeller som mangler overskrifer (&lt;th&gt;) er mest sannsynligvis kodet feil. Vi bruker av prinsipp ikke layout-tabeller (role="presentation). (Krever manuel verifisering)</th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F91.html">F91</a></td>
    <td></td>
  </tr>
   <tr>
    <th scope="row">role='presentation' har blir brukt i en tabell med th. Vi skal som prinsipp aldri bruke role='presentation'. (Krever manuel verifisering)</th>
    <td>✅</td>
    <td>✅</td>
    <td>xz</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F92.html">F92</a></td>
    <td></td>
  </tr>
     <tr>
    <th scope="row">HEADERS attributet referer til en table header ID som ikke eksiterer.</th>
    <td>✅</td>
    <td>x</td>
    <td>x</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F90.html">F90</a></td>
    <td></td>
  </tr>
  <tr>
    <th scope="row">Using spaces to create columns results in screen readers reading columns in the wrong order</th>
    <td>✅ Det ser ut som SortSite reagerer på pre og ascii</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/F33.html">F33</a>, <a href="https://www.w3.org/TR/WCAG20-TECHS/F34.html">F34</a>, <a href="https://www.w3.org/TR/WCAG20-TECHS/F48.html">F48</a></td>
    <td><a href="https://www.w3.org/TR/2008/REC-WCAG20-20081211/#content-structure-separation-programmatic">1.3.1</a></td>
  </tr>
  <tr>
    <th scope="row"><td> skal ikke ha scope="row" eller scope="column"</th>
    <td>x</td>
    <td>v</td>
    <td>x</td>
    <td>?</td>
    <td></td>
    <td></td>
  </tr>
</table>

### Det verktøyene ikke tester på tabeller
- Om en tabell er lagt i et bilde
- Om tabellen er en layout-tabell eller om den presenterer data.
- Om rad / kolonneoverskriftene er beskrivende
- Om overskriftene i tabellen er kodet korrekt. (Er det som ser ut som en overskrift kodet som en overskrift?)

Komplekse tabeller må undersøkes manuelt.

