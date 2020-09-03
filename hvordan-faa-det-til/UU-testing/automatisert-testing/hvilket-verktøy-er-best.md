<alertstripe type="advarsel">Denne siden er under arbeid og ikke fullstendig. Du finner oversikten til nå på <a href="https://confluence.adeo.no/display/MEBO/Automatisert+testing">NAV-intern Confluence-side</a>.</alertstripe>

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
            <th>Alt-teksten skal ikke være et filnavn</th>
            <td>&#10003;</td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>AREA element må ha et ALT Attribute </th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>IMG elementer må ha en ALT Attribute</th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Input TYPE = IMAGE må ha et beskrivende ALT Attribute</th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>ALT-tekst skal ikke bruke ASCII ART (inkludert smileys)</th>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>BUTTON elements som bare inneholder IMG skal ha et ALT attribute for bildet</th>
            <td>✅</td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Alt-teksten er lik lenketeksten</th>
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
            <th>Sidetittel - Nettsiden har en <code>&#x3C;title&#x3E;</code> som beskriver den aktuelle sidens emne eller formål.</th>
            <td>✅</td>
            <td></td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Line break - "<code><br /></code>" skal ikke benyttes for å formatere avsnitt (<p>)</th>
            <td></td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>Språk - Siden ma ha lang-attribute (lang=....)</th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Kodefeil (markup errors)</th>
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
            <th>Tekst og bakgrunn har god nok kontrastn (4,5:1, nivå AA).</th>
            <td></td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>Tekst og bakgrunn har en kontrast på 7:1 (nivå AAA)</th>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Alt-teksten skal ikke inneholder farger. Antagelse: SortSite sjekker kun engelske ord (f.eks red, blue..)</th>
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
            <th>Finnes det tomme overskriftstagger på siden(<code>&#x3C;h*&#x3E;&#x3C;/h*&#x3E;</code>)?</th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Har overskriftsnivåene korrekt rekkefølge?</th>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Overskrifter skal ikke inne holde andre overskrifter</th>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Det brukes HTML-overskrifter (<code>&#x3C;h*&#x3E;</code>). Det brukes ikke CSS til å formattere ikke-overskrifter til å se ut som overskrifter.</th>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Alenestående end-tag ("stray end tag"</th>
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
            <th>Komplekse tabeller, krever manuell verifisering(</th>
            <td>✅</td>
            <td>✅</td>
            <td></td>     
        </tr>
        <tr>
            <th>Layout-tabeller skal ikke ha SUMMARY eller CAPTION</th>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>Tabeller som mangler overskrifer (<code>&#x3C;th&#x3E;</code>) er mest sannsynligvis kodet feil.</th>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>role='presentation' har blir brukt i en tabell med <code>&#x3C;th&#x3E;</code>. Krever manuel verifisering.</th>
            <td>✅</td>
            <td>✅</td>
            <td></td>
        </tr>
        <tr>
            <th>HEADERS-attributet referer til en table header-ID som ikke eksiterer</th>
            <td>✅</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Bruk av tomrom for å skape kolonner resulerer i at skjermlesere leser kolonner i feil rekkefølge.</th>
            <td>✅</td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th><code>&#x3C;th&#x3E;</code> skal ikke ha <code>scope="row"</code> eller <code>scope="col"</code></th>
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
            <th>Siden inneholder et LANGattribute(</th>
            <td>✅</td>
            <td>✅</td>
            <td>✅</td>     
        </tr>
        <tr>
            <th>Er teksten på siden skrevet på et annet språk enn det som står i lang attributet? (må verifiseres)</th>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Sidens title skal ikke være tom</th>
            <td></td>
            <td></td>
            <td>✅</td>
        </tr>
        <tr>
            <th>Innhold som er i et annet språk bør være i en SPAN eller DIV med et LANG attribute .</th>
            <td></td>
            <td></td>
            <td></td>
        </tr>
</table>
