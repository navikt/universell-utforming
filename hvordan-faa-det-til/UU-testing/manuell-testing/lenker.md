# Lenker

## Hvorfor det er viktig
Mange mennesker orienterer seg på nettsider gjennom å skanne overskrifter og lenker. De vil raskt kunne se om de er på riktig side, eller hvilken lenke som eventuelt kan være riktig vei videre til ønsket innhold. Skjermleserbrukere tar ofte opp lenkelister, som viser alle lenker på siden. Her et eksempel med VoiceOver på MAC på nav.no:

![Lenkeliste nav.no](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/lenkeliste1.png)


## Teststeg
Verktøy som ARC toolkit kan vise hva som er kodet som lenke, så det blir lettere å se hva som burde være tydelig klikkbar. Noen verktøy kan også teste for brudde lenker. Det meste krever en manuell sjekk:

1. Har dere brukt [Designsystemet og NAV frontend](https://design.nav.no/)?
  - Sjekk skjermbildet. 
    - Er det lett å forstå at lenken er klikkbar?
    - Er lenker i tekst understreket eller skiller de seg fra annen tekst med mer enn bare farge (for eksempel ikoner)?
  - Sjekk at fokusmarkering ved hover og mouse over  er tydelig og i henhold til designsystemet.
2. Kommer det tydelig frem av lenketeksten hva som kommer til å skje når du trykker på den? Unngå "Les mer" og liknende. 
3. Fungerer lenken? 
4. Når du trykker på lenken, er det samsvar mellom lenketeksten og overskriften på siden du kommer til? 

## Verktøy du kan bruke
Et eksempel på hvordan ARC toolkit kan vise hva som er kodet som lenke:

![Lenkemarkering i ARC toolkit](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/arc-lenke.png)

## Andre ressurser
* [Lær mer om hvordan teste lenker på Tilsynets veiledningssider.](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#lenker)


