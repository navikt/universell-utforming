# Tastaturnavigasjon

## Hvorfor det er viktig
At alt lar seg navigere bare med tastatur, er en viktig forutsetning for at løsningen fungerer med skjermleser og andre hjelpemidler. Det er også viktig for personer som ikke ønsker eller ikke kan bruke musepeker, som superbrukere eller personer som opplever skjelving i hendene.

## Teststeg
Automatiserte verktøy kan mest vise tab-rekkefølgen, slik at man selv kan se om det samsvarer med den visuelle rekkefølgen. Se gjerne [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md) der vi viser hva SortSite, ARC Toolkit og W3Cs kodesjekker tester. 

Ellers er tastaturnavigasjon noe som stort sett må testes manuelt:

1. Får alle interaktive elementer som lenker, knapper og skjema-elementer en tydelig fokusmarkering?
2. Er fokusmarkeringen i tråd med NAVs designsystem? Den skal være som på [design.nav.no](https://design.nav.no/).
3. Er det mulig å bruke siden kun med tastatur?  Se om du kan nå og betjene alle interaktive elementer som knapper, lenker, nedtrekkslister, datovelgere og menyer. Du skal hverken "sitte fast" eller oppleve at fokuset flytter seg uforventet.
4. Er tastaturrekkefølgen den samme som den visuelle rekkefølgen på innholdet? (se også lengre ned under "Verktøy du kan bruke")
5. Har siden snarveislenkene «til hovedmeny» , «til hovedinnhold», og "til toppen" og fungerer de som de skal? De skal være de første elementene som får fokus på siden (bortsett fra "til toppen"), fokus skal være i tråd med designsystemet, og de skal lede til riktig sted på siden.

### Slik bør siden fungere med bare tastatur
For å navigere med bare tastatur brukes det som oftest en kombinasjon av noen enkelte taster som tab, space og enter. Se gjerne hvordan enkelte elementer bør fungere på [WebAIMs side om tastaturnavigasjon](https://webaim.org/techniques/keyboard/#testing). 

## Verktøy du kan bruke
Her som eksempel hvordan ARC toolkit viser tab-rekkefølgen:
![Tabrekkefølge med ARC toolkit](/hvordan-faa-det-til/UU-testing/manuell-testing/tabrekkefolge.png)

## Andre ressurser
* [Lær mer om hvordan teste tastaturnavigasjon på Tilsynets veiledningssider](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tastaturnavigasjon)
* [WebAIMs veileder for tastatur](https://webaim.org/techniques/keyboard/)
