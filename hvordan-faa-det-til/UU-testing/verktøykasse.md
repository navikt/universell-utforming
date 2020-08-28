# Verktøykasse

<alertstripe type="advarsel">
    <strong>VIKTIG!</strong> Før du tar i bruk noen av verktøyene nedenfor, må du huske at sikkerhet og personvern SKAL ivaretas. Sørg derfor for at du tester på testmiljøer og lignende som har fiktiv testdata. En av grunnene til dette er at noen av utvidelsene til nettlesere KAN sende data til servere utenfor NAV.
</alertstripe>

## Tastatur
Det er svært viktig at alt fungerer bare med tastatur. Test dette jevnlig. WAI har laget en [veileder om hvordan elementer bør oppføre seg når man bruker tastatur](https://webaim.org/techniques/keyboard/).

## Før- og etter-sider
W3C har laget noen før- og etter-sider. Sidene ser ganske like ut, men "før"-sidene har en rekke uu-feil, som er fikset i "etter"-sidene. Test gjerne verktøyene på disse sidene: https://www.w3.org/WAI/demos/bad/. 

## Skjermlesere

- [**Voice over**](https://webaim.org/articles/voiceover/) - Gratis innebygd skjermleser på Mac og iPhone.
    - Se video: [*Screen Reader Basics: VoiceOver -- A11ycasts #07*](https://www.youtube.com/watch?v=5R-6WvAihms)
    - Se video: [*Assistive Tech: VoiceOver on iOS*](https://www.youtube.com/watch?v=bCHpdjvxBws)
    - Guide med shortcuts og mer info: [*Using VoiceOver to Evaluate Web Accessibility*](https://webaim.org/articles/voiceover/) 
- [**JAWS**](https://webaim.org/articles/jaws/) - Den mest populære skjermleseren til Windows. Kan være kostbar. Standard-skjermleser til våre interne ansatte på jobb.
    - Guide med shortcuts og mer info: [*Using JAWS to Evaluate Web Accessibility*](https://webaim.org/articles/jaws/)
- [**NVDA**](https://webaim.org/articles/nvda/) - Populær og gratis skjermleser til Windows.
    - Se video: [*Screen Reader Basics: NVDA -- A11ycasts #09*](https://www.youtube.com/watch?v=Jao3s_CwdRU)
    - Guide med shortcuts og mer info: [*Using NVDA to Evaluate Web Accessibility*](https://webaim.org/articles/nvda/)
    - [*Download NVDA*](https://www.nvaccess.org/)
- [**TalkBack**](https://support.google.com/accessibility/android/answer/6283677?hl=en) - Gratis skjermleser til Android.
    - Se video: [*Assistive Tech: TalkBack*](https://www.youtube.com/watch?v=0Zpzl4EKCco)

## Lese- og skrivevansker

- [**Dyslexia Formatter**](https://chrome.google.com/webstore/detail/dyslexia-formatter/kggkghfhlppjclojgphbploiaipgogoc) - gratis utvidelse til Chrome som gjør det enklere å tilegne seg informasjon og bruke nettbaserte tjenester for folk med dysleksi

## Kontrastforhold

- [**http://contrastchecker.com/**](http://contrastchecker.com/)  - her kan du legge inn fargekodene dine og få et konkret svar om kontrastforholdet er i tråd med WCAG-kravene. Du kan også se gråtoner som fargeblind (arkfaner øverst til høyre)
- [**https://webaim.org/resources/contrastchecker/**](https://webaim.org/resources/contrastchecker/)
- [**http://accessible-colors.com/**](http://accessible-colors.com/)

## Automatisk analyse

- [**W3Cs kodevalidator**](https://validator.w3.org/) - W3Cs verktøy for å teste om markup-en er valide (ikke direkte uu-tester, men sjekker om koden er i tråd med HTML-standarden, som er en viktig forutsetning for å møte uu-krav). Har blitt brukt i tilsyn.
- [**Chrome DevTools**](https://developers.google.com/web/tools/chrome-devtools/) - gratis sett med webutviklerverktøy som ligger integrert i Google Chrome-nettleseren. Kan hjelpe deg med å redigere/manipulere en hvilken som helst nettside/tjeneste og raskt diagnostisere problemer. 
    - Se video: [*The new way to test accessibility with Chrome DevTools - A11ycasts #23*](https://www.youtube.com/watch?v=b0Q5Zp_yKaU)
- [**Lighthouse**](https://developers.google.com/web/tools/lighthouse/) (del av Chrome DevTools) - gir rask og detaljert analyse av nettsider med kriterier for ytelse, tilgjengelighet, progressive webapps, beste praksis, søkemotoroptimalisering for både mobile og desktop. Kan kjøres rett i Chrome DevTools, fra kommandolinjen, eller som en nodemodul
- **Web Developer Toolbar** ([Chrome](https://chrome.google.com/webstore/detail/web-developer-toolbar/deeboegbjcnfgidliakhpoapnpomphji)/[Firefox](https://addons.mozilla.org/en-US/firefox/addon/web-developer/)) - gratis utvidelse med et hav av muligheter til å manipulere og validere nettsider.
- [**ARC Toolkit**](https://chrome.google.com/webstore/detail/arc-toolkit/chdkkkccnlfncngelccgbgfmjebmkmce) - gratis utvidelse til Chrome med rike verktøy for å teste opp mot WCAG 2.0, WCAG 2.1, EN 301 549, Section 508.
- [**Visual Aria**](https://chrome.google.com/webstore/detail/visual-aria/lhbmajchkkmakajkjenkchhnhbadmhmk) - gratis utvidelse til Chrome som gir en visuell oversikt over ARIA-attributter som brukes på en nettside, inkludert live regioner, roller, nøsting og fokushåndtering.
- [**WAVE**](https://wave.webaim.org/) - gratis utvidelse til Chrome og Firefox som evaluerer tilgjengeligheten på nettsider og gir en veldig visuell tilbakemelding.
- [**AXE Coconut**](https://chrome.google.com/webstore/detail/axe-coconut/iobddmbdndbbbfjopjdgadphaoihpojp) - gratis utvidelse for Chrome
    - Se video: [*Testing Shadow DOM with aXe Coconut - A11ycasts #26*](https://www.youtube.com/watch?v=1uyQdC3LqLo)
- [**SortSite**](https://www.powermapper.com/products/sortsite/) - godt verktøy for validering av grensesnittkode opp mot W3C-standarder som WCAG 2.0/2.1, HTML5, CSS3, etc. Gir en god oversikt sammen med en god beskrivelse av hva som er feil, hvor feilen er og hvordan den kan fikses. Pris ca NOK 8000,- per lisens. 
- [**SiteImprove**](https://siteimprove.com/nb-no/) - godt verktøy som gir deg en lettfattelig og god oversikt over problemer og forbedringsområder. Som f.eks. dårlig kodekvalitet og kvalitetsfeil som brutte lenker og stavefeil, kontrastforhold som er for dårlig, m.m. Verktøy tester opp mot W3Cs standarder som f.eks. HTML5 og WCAG 2.0/2.1 og man kan filtrere funnene på roller (utvikler, redaktør, etc). God beskrivelse for hva som er feil og hvordan det kan fikses. Har blitt brukt i tilsyn.
- [**Total Validator Pro**](http://www.totalvalidator.com/) - et av de bedre verktøyene til validering av kildekode og støtte for universell utforming. Pro-versjonen til kr 250,- (NAV har 30 lisenser).
- [**Adobe Acrobat DC (PDF)**](https://helpx.adobe.com/no/acrobat/user-guide.html?topic=/no/no/acrobat/morehelp/accessibility_tags_and_reflow.ug.js) - validering av PDF-skjema opp mot W3C standarder som WCAG 2.0/2.1 (Verktøy>Tilgjengelighet>Tilgjengelighetskontroll eller Full kontroll. NAV har lisenser på dette.

## Automatisk testing

<alertstripe type="advarsel">Det er viktig å være klar over at automatisk testing vanligvis bare avdekker ~30% av feil, og at man helst bør kombinere disse med både brukertester og manuelle ekspertevalueringer i tillegg.</alertstripe>

### Linting

- [**Vue ESLint**](https://github.com/maranran/eslint-plugin-vue-a11y) - Static AST checker for accessibility rules on elements in .vue.
- [**JSX ESLint**](https://github.com/evcohen/eslint-plugin-jsx-a11y) - Static AST checker for a11y rules on JSX elements.
- [**JSX TSLint**](https://github.com/joaovieira/tslint-react-a11y#readme) - JSX a11y lint rules for TSLint.
- [**Angular Codelyzer**](https://github.com/mgechev/codelyzer#readme) - A set of tslint rules for static code analysis of Angular TypeScript projects.

### Enhetstester

- [**Jest Axe**](https://github.com/nickcolley/jest-axe) - Custom Jest matcher for aXe for testing accessibility.

### Ende-til-ende

- [**axe-core**](https://github.com/dequelabs/axe-core) - Accessibility engine for automated Web UI testing https://www.deque.com/axe/

### CI/CD

- [**Pa11y**](https://github.com/pa11y/pa11y) - Pa11y is your automated accessibility testing pal. It runs accessibility tests on your pages via the command line or Node.js, so you can automate your testing process.

Takk til Kristoffer Nordström for denne flotte oversikten i [hans artikkel på Kode24.no](https://www.kode24.no/kodenytt/5-verktoy-for-bedre-tilgjengelighet/72149017).
