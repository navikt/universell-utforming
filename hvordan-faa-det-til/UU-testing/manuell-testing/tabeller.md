# Tabeller

## Hvorfor det er viktig
Tabeller skal utelukkende brukes til å presentere data, og ikke for å styre layout og utseende. 
Riktig bruk av tabeller er avgjørende for at informasjonen blir tolket riktig av hjelpemiddel og brukeren klarer å tolke kompleks informasjon. [uu.difi.no](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tabeller)


Ha gjerne tekst, bilder illustrasjoner og/eller diagrammer i tillegg til tabellen for å gjøre komplekst innhold mer forståelig.

## Teststeg
Automatiserte testverktøy kan ofte identifisere det som er kodet som tabeller.

1. Er alle tabeller kodet med &lt;table&gt;? 
2. Er rad- og/eller -kolonneoverskriftene er kodet med &lt;th&gt;?
3. Er tabeller som har både rad- og kolonneoverskrifter kodet med &lt;th scope="row"&gt; / &lt;th scope="col"&gt;?
  - Sjekk at tabellen innehar tilsvarende oppbygning slik som markert med uthevet tekst nedenfor:
    ```
    <table>
    <caption>Åpningstider</caption>
    <thead>
      <tr>
        <td></td>
        <th scope=”col”>September-April</th>
        <th scope=”col”>Mai-August</th>
    </tr>
    <thead>
    <tbody>
      <tr>
        <th scope=”row”>Mandag</th>
        <td>10-17</td>
        <td>09-19</td>
      </tr>
      …
    </tbody>
    </table>
```
4. Er tabellens tittel kodet med &lt;caption&gt;?
  - Sjekk at koden bygger på en lignende struktur som dette:
  ```
  <table>
  <caption>Mobilnummer hos NAV IT</caption>
  <thead>
   <tr>
   ...
  </table>
  ```

## Verktøy du kan bruke
Verktøy som ARC toolkit kan fremheve tabeller og hvordan kolonner og rader er kodet:

![test med ARCtoolkit på tabeller](hvordan-faa-det-til/UU-testing/manuell-testing/tabeller-arc.png)

## Andre ressurser
* Mange gode eksempler på [tilsynets veiledningsider for tabeller](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tabeller)
* W3Cs [web accessibility tutorial om tabeller](https://www.w3.org/WAI/tutorials/tables/)

