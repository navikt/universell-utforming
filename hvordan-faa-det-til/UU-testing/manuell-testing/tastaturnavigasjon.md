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
<table>
	<tbody><tr>
		<th scope="col">Interaksjon </th>
		<th scope="col">Tastetrykk</th>
		<th scope="col">Kommentar</th>
	</tr>
	<tr>
		<td>Naviger til interaktive elementer</td>
		<td><ul>
			<li><span class="keycap">Tab</span></li>
			<li><span class="keycap">Shift</span> + <span class="keycap">Tab</span> - naviger tilbake</li>
		</ul>			</td>
		<td>
			<ul>
				<li>Det må være en synlig fokusindikator.</li>
				<li>Navigasjonsrekkefølgen bør være logisk og intuitiv.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>Lenke</td>
		<td><span class="keycap">Enter</span></td>
		<td></td>
	</tr>
	<tr>
		<td>Knapp</td>
		<td><span class="keycap">Enter</span> or <span class="keycap">Spacebar</span></td>
		<td>Ensure elements with ARIA <code>role="button"</code> can  be activated with both key commands.</td>
	</tr>
	<tr>
		<td>Sjekkboks</td>
		<td><span class="keycap">Spacebar</span> - velg / avveg en sjekkboks</td>
		<td>Sjekkbokser burde brukes når man kan velge én eller flere opsjoner.</td>
	</tr>
	<tr>
		<td>Radioknapper</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> or <span class="keycap">←</span>/<span class="keycap">→</span> - velg en opsjon. </li>
				<li><span class="keycap">Tab</span> - gå til neste element.</li>
			</ul>
		</td>
		<td>Radioknapper bør brukes når man bare kan velge en opsjon i en gruppe.</td>
	</tr>
	<tr>
		<td>Select (dropdown) meny</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - naviger mellom menyopsjoner</li>
				<li><span class="keycap">Spacebar</span> - expander</li>
			</ul>
		</td>
		<td>Du kan også filterer ved å taste bokstaver, men oppførseln varierer avhengig av nettleser. Noen vil filtrerer mens du taster, som autocomplete. You can also filter by typing letters, but this behavior varies by browser. Some will filter as you type, like autocomplete. Andre vil bare sorterer basert på første bokstav, som for eksemepl i en liste med Norske fylker, da vil taste <span class="keycap">V</span> then <span class="keycap">I</span> ta deg til <strong>V</strong>iken, eller det kan ta deg til <strong>Vestfold og Telemark/strong> and then <strong>I</strong>nnlandet.</td>
	</tr>
	<tr>
		<td>Autocomplete</td>
		<td>
			<ul>
				<li>Tast for å starte filtering</li>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - naviger til en opsjon</li>
				<li><span class="keycap">Enter</span> - velg en opsjon</li>
			</ul>
		</td>
		<td></td>
	</tr>
	<tr>
		<td>Dialog</td>
		<td><span class="keycap">Esc</span> - steng</td>
		<td>
			<ul>
				<li>Modalbokser bør få tastaturfokus.</li>
				<li>Dialoger som ikker modalbokser bør stenges automatisk når de mister fokus.</li>
				<li>Når en dialog stenges, bør fokuset til vanlig gå tilbake til elementet som åpnet dialogen.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>Slider</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> or <span class="keycap">←</span>/<span class="keycap">→</span> - øke eller redusere slider-verdi</li>
				<li><span class="keycap">Home</span>/<span class="keycap">End</span> - Start eller slutt</li>
			</ul>								
		</td>
		<td>
			<ul>
				<li>For double-sliders (for å definere et område/range), <span class="keycap">Tab</span>/<span class="keycap">Shift</span> + <span class="keycap">Tab</span> burde toggle mellom ekstremverdiene</li>
				<li>I noen sliders kan <span class="keycap">PageUp</span>/<span class="keycap">PageDown</span> øke /redusere verdien i større bolker (for eksempel med 10).</li>
			</ul>								
		</td>
	</tr>
	<tr>
		<td>Menu bar</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - Forrige/neste meny-opsjon</li>
				<li><span class="keycap">Enter</span> - ekspander menyen (opsjonal) og velg en opsjon.</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - ekspander/kollaps submeny</li>
			</ul>
		</td>
		<td>
			<ul>
				<li>Ikke alle menyer burde ha disse controls. Enklere menyer burde vanligvis fungere med <span class="keycap">Tab</span>/<span class="keycap">Enter</span>.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>Tab panel</td>
		<td>
			<ul>
				<li><span class="keycap">Tab</span> - når man navigerer inn i tab-gruppen og når man navigerer ut av tab-gruppen</li>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> eller <span class="keycap">←</span>/<span class="keycap">→</span> - forrige/neste tab.</li>									
			</ul>
		</td>
		<td>
			<ul>
				<li>Dette her gjelder for "application"-tabs som endrere seg uten at siden lastes på nytt. Når en meny ser ut som en tab-liste, men er egentlig en lenkeliste til forskjellige sider, er <span class="keycap">Tab</span> og <span class="keycap">Enter</span> bedre valget.</li>
				<li>Tab-innholdet bør oppdaters automatisk når piltastene trykkes. Du burde ikke bruke Enter for å aktivere tab-en.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>'Tre'-meny</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - Naviger til forrige/neste opsjon</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - Ekspander/kollaps submeny, gå opp/ned et nivå.</li>
			</ul>
		</td>
		<td></td>
	</tr>
	<tr>						
		<td>Skrolle</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - skroll vertikalt</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - skroll horisontalt</li>
				<li><span class="keycap">Spacebar</span> / <span class="keycap">Shift</span> + <span class="keycap">Spacebar</span> - skroll ned omtrent en vindustørrelse</li>
			</ul>
		</td>
		<td>
			<p>Minimer horisontal skrolling.</p>
		</td>
	</tr>
</tbody></table>

Tabellen er oversatt fra [WebAIMs side om tastaturnavigasjon](https://webaim.org/techniques/keyboard/). 

## Verktøy du kan bruke
Automatiserte verktøy kan mest vise tab-rekkefølgen, slik at man selv kan se om det samsvarer med den visuelle rekkefølgen. Se gjerne [Hvilket verktøy er best?](/hvordan-faa-det-til/UU-testing/automatisert-testing/hvilket-verktøy-er-best.md) der vi viser hva SortSite, ARC Toolkit og W3C tester. 

Her som eksempel hvordan ARC toolkit viser tab-rekkefølgen:
![Tabrekkefølge med ARC toolkit](/hvordan-faa-det-til/UU-testing/manuell-testing/tabrekkefolge.png)

## Andre ressurser
* [Lær mer om hvordan teste tastaturnavigasjon på Tilsynets veiledningssider](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tastaturnavigasjon)
* [WebAIMs veileder for tastatur](https://webaim.org/techniques/keyboard/)
