# Språk i koden

## Hvorfor det er viktig
Du må angi innholdets språk i koden for at opplesende hjelpemidler skal kunne velge riktig stemme for opplesing. Søkemotorer benytter dessuten språkangivelsen i koden for å avgjøre relevante treff (kilde: [uu.difi.no](https://www.uutilsynet.no/wcag-standarden/sprak-i-koden/223)).

## Teststeg
[Automatiserte testverktøy](/hvordan-faa-det-til/UU-testing/automatisert-testing/) kan teste om siden mangler lang attribute . (lang=....), men de sjekker ikke om det er korrekt språk som er angitt.

Dette må du alltid teste manuelt:

1. Er språket til innholdet angitt i koden?
2. Hvis det finnes det tekst på siden som er et annet enn hovedinnholdet: er det markert i koden?

## Verktøy du kan bruke
Du bør sjekke for språk-kode i tittelen, og undersøke enkelte avsnitt eller fraser som er skrevet i et annet språk. Dette kan du gjøre direkte i koden, ved å høyreklikke og velge "inspiser".

Her et eksempel der enkelte ord har et annet språk, uten at det ble markert i koden:

![Norsk ord i engelsk tekst uten passende lang-tag i koden](https://github.com/navikt/universell-utforming/blob/master/hvordan-faa-det-til/UU-testing/manuell-testing/spraak.png)

## Andre ressurser
* [Tilsynets veileder for Språk i koden](https://www.uutilsynet.no/wcag-standarden/sprak-i-koden/223)
