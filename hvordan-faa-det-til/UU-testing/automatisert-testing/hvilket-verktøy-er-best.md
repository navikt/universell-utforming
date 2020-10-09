# Hvilket verktøy er best?

Her skal vi legge ut en sammenlikning mellom hva som testes med SortSite, ARC toolkit og W3Cs kodesjekker.

<alertstripe type="advarsel">Denne siden er ikke ferdig enda. Inntil videre finner du den fullstendige oversikten på <a href="https://confluence.adeo.no/display/MEBO/Automatisert+testing">NAV-intern Confluence-side</a>.</alertstripe>



## Bilder

### Det verktøyene tester på bilde
<table>
  <caption>Automatisert test av bilder</caption>
  <tr>
    <td></td>
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
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">AREA-elementer må ha et ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">IMG-elementer uten ALT-Attribute skal ikke ha Title eller ARIA-Label-Attributes</th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2010/WD-WCAG20-TECHS-20100708/F39">F39</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
   <tr>
    <th scope="row">IMG-elementer må ha en ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
     <tr>
    <th scope="row">Input TYPE = IMAGE må ha et beskrivende ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">ALT-tekst skal ikke bruke ASCII ART (inkluderer Smileys)</th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">BUTTON-elementer som bare inneholder en IMG skal ha et ALT-attribute for bildet</th>
    <td>✅</td>
    <td>❌</td>
    <td>✅</td>
    <td>?</td>
    <td></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">Alt-teksten er lik lenketeksten. Dette fører til at skjermlesen leser opp samme teksten to ganger. Dette ønsker vi å unngå. Bruk Alt="" evt. annen teknikk.</th>
    <td>✅</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/TR/WCAG20-TECHS/H2.html">H2</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a>, <a href="https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html">2.4.4</a>, <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-link.html">2.4.9</a></td>
  </tr>
  <tr>
    <th scope="row">Dekorasjonsbilder (og Spacer images) skal ikke alt-tekst. Dokumentasjonen sier at SortSite tester dette....</th>
    <td>ℹ️</td>
    <td>❌</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2010/WD-WCAG20-TECHS-20100708/F39">F39</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
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
  <caption>Automatisert test av bilder</caption>
  <tr>
    <td></td>
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
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">AREA-elementer må ha et ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
  <tr>
    <th scope="row">IMG-elementer uten ALT-Attribute skal ikke ha Title eller ARIA-Label-Attributes</th>
    <td>✅</td>
    <td>✅</td>
    <td>❌</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2010/WD-WCAG20-TECHS-20100708/F39">F39</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
   <tr>
    <th scope="row">IMG-elementer må ha en ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
     <tr>
    <th scope="row">Input TYPE = IMAGE må ha et beskrivende ALT-Attribute</th>
    <td>✅</td>
    <td>✅</td>
    <td>✅</td>
    <td>?</td>
    <td><a href="https://www.w3.org/WAI/GL/2014/WD-WCAG20-TECHS-20140107/F65">F65</a></td>
    <td><a href"https://www.w3.org/TR/2008/REC-WCAG20-20081211/#text-equiv-all">1.1.1</a></td>
  </tr>
</table>

### Det verktøyene ikke tester på struktur
