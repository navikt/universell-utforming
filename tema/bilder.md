# Bilder

## Kontrast

(tekst om kontrast her)

## Alt-tekster

Alle meningsbærende bilder skal ha en beskrivende alt-tekst.

## Hva er en alt-tekst?

En alt-tekst (kort for alternativ tekst) er en tekst som vises eller leses opp når bildet ikke vises for brukeren. Dette kan være fordi:

- Bildet ble ikke funnet
- Brukeren har skrudd av bildenedlasting
- Brukeren har dårlig internettoppkobling
- Brukeren bruker en skjermleser (for eksempel bilde)
- Brukeren bruker en rent tekstbasert nettleser (f.eks. Lynx)

Begrepet «bilde» favner i denne konteksten både fotografier, illustrasjoner, logoer, ikoner, grafer, infografikk og annen type grafikk.

### Bilder uten alt-tekst

Bilder som ikke er meningsbærende (for eksempel bare til pynt eller overflødig) skal ikke ha noe alt-text, men <strong>husk</strong> å gi dem et tomt alt-attributt:

|**Gjør:**|**Ikke gjør:**|
|:-|:-|
|`<img src="pynt.jpg" alt="" />`|`<img src="pynt.jpg" />`|

Skjermlesere trenger et tomt alt-attributt for å vite at de skal ignorere bildet. For bilder uten alt-attributt er det fare for at skjermlesere leser opp kilde-attributtet i stedet.

### Er bildet «meningsbærende»?

Det er ikke alltid enkelt å vite om bildet er meningsbærende eller rent dekorativt.

En god start kan være å «leke skjermleser»: prøv å les opp siden som den skulle blitt lest for en bruker med skjermleser. Går brukeren glipp av relevant informasjon hvis du hopper over bildene?

Hvis bildene bare gjentar informasjon som er tilgjengelig i nærheten som ren tekst er alt-tekster på disse overfødig.

#### Beslutningstre for alt-tekster

Hvis du er i tvil anbefaler vi å bruke [W3C sitt beslutningstre](https://www.w3.org/WAI/tutorials/images/decision-tree/) for å finne ut om man trenger alt-tekster eller ikke.

### Hvordan skrive alt-tekster

- [Tips &amp; tricks (W3C)](https://www.w3.org/WAI/tutorials/images/tips/)
- [E-læringskurs for redaktører og skribenter (Difi)](https://uu.difi.no/krav-og-regelverk/kom-i-gang/e-laeringskurs-om-universell-utforming-av-nettinnhold)
