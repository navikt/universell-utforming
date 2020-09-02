OBS! Denne siden er under arbeid og ikke fullstendig. Du finner oversikten til nå på [NAV-intern Confluence-side](https://confluence.adeo.no/display/MEBO/Automatisert+testing).

# Hvilket verktøy er best?
## Bilder

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Alt-teksten skal ikke være et filnavn</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>AREA element må ha et ALT Attribute </td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>IMG elementer må ha en ALT Attribute</td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Input TYPE = IMAGE må ha et beskrivende ALT Attribute</td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>ALT-tekst skal ikke bruke ASCII ART (inkludert smileys)</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>BUTTON elements som bare inneholder IMG skal ha et ALT attribute for bildet</td>
            <td>✅</td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Alt-teksten er lik lenketeksten</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
</table>

## Struktur

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Sidetittel - Nettsiden har en <title> som beskriver den aktuelle sidens emne eller formål.</td>
            <td>✅</td>
            <td></td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Line break - "<code><br /></code>" skal ikke benyttes for å formatere avsnitt (<p>)</td>
            <td></td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>Språk - Siden ma ha lang-attribute (lang=....)</td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Kodefeil (markup errors)</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
</table>

## Farger / Kontrast

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Tekst og bakgrunn har god nok kontrastn (4,5:1, nivå AA).</td>
            <td></td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>Tekst og bakgrunn har en kontrast på 7:1 (nivå AAA)</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Alt-teksten skal ikke inneholder farger. Antagelse: SortSite sjekker kun engelske ord (f.eks red, blue..)</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
</table>

## Overskrifter

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Finnes det tomme overskriftstagger på siden(<h*></h*>)?</td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Har overskriftsnivåene korrekt rekkefølge?</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Overskrifter skal ikke inne holde andre overskrifter</td>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Det brukes HTML-overskrifter (<h*>). Det brukes ikke CSS til å formattere ikke-overskrifter til å se ut som overskrifter.</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Alenestående end-tag ("stray end tag"</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
</table>

## Tabeller

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Komplekse tabeller, krever manuell verifisering(</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>Layout-tabeller skal ikke ha SUMMARY eller CAPTION</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>Tabeller som mangler overskrifer (<th>) er mest sannsynligvis kodet feil.</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>role='presentation' har blir brukt i en tabell med <th>. Krever manuel verifisering.</td>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>HEADERS-attributet referer til en table header-ID som ikke eksiterer</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Bruk av tomrom for å skape kolonner resulerer i at skjermlesere leser kolonner i feil rekkefølge.</td>
            <td>✅</td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
    <th>"<code><td></code>" skal ikke ha scope="row" eller scope="col"</td>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
</table>

## Innhold

<table>
    <thead>
        <tr>
            <th>Reglene som testes</th>
            <th>SortSite</th>
            <th>ARCToolkit</th>
            <th>W3C</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Siden inneholder et LANGattribute(</td>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Er teksten på siden skrevet på et annet språk enn det som står i lang attributet? (må verifiseres)</td>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Sidens title skal ikke være tom</td>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Innhold som er i et annet språk bør være i en SPAN eller DIV med et LANG attribute .</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
</table>
