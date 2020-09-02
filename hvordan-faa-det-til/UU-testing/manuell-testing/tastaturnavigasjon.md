# Tastaturnavigasjon

## Hvorfor det er viktig
At alt lar seg navigere bare med tastatur, er en viktig forutsetning for at løsningen fungerer med skjermleser og andre hjelpemidler. Det er også viktig for personer som ikke ønsker eller ikke kan bruke musepeker, som superbrukere eller personer som opplever skjelving i hendene.

## Teststeg
Dette må du alltid teste manuelt:

1. Får alle interaktive elementer som lenker, knapper og skjema-elementer en tydelig fokusmarkering?
2. Er fokusmarkeringen i tråd med NAVs designsystem? Den skal være som på [design.nav.no](https://design.nav.no/).
3. Er det mulig å bruke siden kun med tastatur?  Se om du kan nå og betjene alle interaktive elementer som knapper, lenker og menyer. Du skal hverken "sitte fast" eller oppleve at fokuset flytter seg uforventet.
4. Er tastaturrekkefølgen den samme som den visuelle rekkefølgen på innholdet? (se også lengre ned under "automatisert testing")
5. Får du tilgang til alt innhold og alle funksjoner, med kun bruk av tastatur, dersom du forstørrer siden til 200%? 
6. Har siden snarveislenkene «til hovedmeny» , «til hovedinnhold», og "til toppen" og fungerer de som de skal?  

### Slik bør siden fungere med bare tastatur
For å navigere med bare tastatur brukes det som oftest en kombinasjon av noen enkelte taster som tab, space og enter. Se gjerne hvordan enkelte elementer bør fungere på [WebAIMs side om tastaturnavigasjon](https://webaim.org/techniques/keyboard/#testing). 

## Verktøy du kan bruke
Automatiserte verktøy kan mest vise tab-rekkefølgen, slik at man selv kan se om det samsvarer med den visuelle rekkefølgen. Se gjerne [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md) der vi viser hva SortSite, ARC Toolkit og W3C tester. 

Her som eksempel hvordan ARC toolkit viser tab-rekkefølgen:
![Tabrekkefølge med ARC toolkit](/hvordan-faa-det-til/UU-testing/manuell-testing/tabrekkefolge.png)

## Andre ressurser
* [Lær mer om hvordan teste tastaturnavigasjon på Tilsynets veiledningssider](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tastaturnavigasjon)
* [WebAIMs veileder for tastatur](https://webaim.org/techniques/keyboard/)
