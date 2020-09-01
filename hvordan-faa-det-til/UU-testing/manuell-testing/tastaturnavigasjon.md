# Tastaturnavigasjon

## Hvorfor det er viktig
At alt lar seg navigere bare med tastatur, er en viktig forutsetning for at løsningen fungerer med skjermleser og andre hjelpemidler. Det er også viktig for personer som ikke ønsker eller ikke kan bruke musepeker, som superbrukere eller personer som opplever skjelving i hendene.

## Teststeg
Dette må du alltid teste manuelt:

1. Får alle lenker, knapper, skjema-elementer osv. tydelig fokusmarkering?
2. Er fokusmarkeringen i tråd med NAVs designsystem? Den skal være som på [design.nav.no](https://design.nav.no/).
3. Er det mulig å bruke siden kun med tastatur?  Se om du kan nå og betjene alle interaktive elementer som knapper, lenker og menyer.
4. Er tastaturrekkefølgen den samme som den visuelle rekkefølgen på innholdet? 
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
		<td>Du kan også filterer ved å taste bokstaver, men oppførseln varierer avhengig av nettleser. Noen vil filtrerer mens du taster, som autocomplete. You can also filter by typing letters, but this behavior varies by browser. Some will filter as you type, like autocomplete. Andre vil bare sorterer basert på første bokstav, som for eksemepl i en liste med Norske fylker, da vil taste <span class="keycap">V</span> then <span class="keycap">I</span> ta deg til <strong>V</strong>iken, eller det kan ta deg til <strong>Vestfold og Telemark/strong> and then <strong>I</strong>nlandet.</td>
	</tr>
	<tr>
		<td>Autocomplete</td>
		<td>
			<ul>
				<li>Type to begin filtering</li>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - navigate to an option</li>
				<li><span class="keycap">Enter</span> - select an option</li>
			</ul>
		</td>
		<td></td>
	</tr>
	<tr>
		<td>Dialog</td>
		<td><span class="keycap">Esc</span> - close</td>
		<td>
			<ul>
				<li>Modal dialogs should maintain keyboard focus.</li>
				<li>Non-modal dialogs should close automatically when they lose focus.</li>
				<li>When a dialog closes, focus should usually return to the element that opened the dialog.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>Slider</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> or <span class="keycap">←</span>/<span class="keycap">→</span> - increase or decrease slider value</li>
				<li><span class="keycap">Home</span>/<span class="keycap">End</span> - beginning or end</li>
			</ul>								
		</td>
		<td>
			<ul>
				<li>For double-sliders (to set a range), <span class="keycap">Tab</span>/<span class="keycap">Shift</span> + <span class="keycap">Tab</span> should toggle between each end.</li>
				<li>In some sliders <span class="keycap">PageUp</span>/<span class="keycap">PageDown</span> can move by a larger increment (e.g., by 10).</li>
			</ul>								
		</td>
	</tr>
	<tr>
		<td>Menu bar</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - Previous/next menu option</li>
				<li><span class="keycap">Enter</span> - expand the menu (optional) and select an option.</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - expand/collapse submenu</li>
			</ul>
		</td>
		<td>
			<ul>
				<li>Not all menus should have these controls. Simpler menus should usually rely on <span class="keycap">Tab</span>/<span class="keycap">Enter</span>.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>Tab panel</td>
		<td>
			<ul>
				<li><span class="keycap">Tab</span> - once to navigate into the group of tabs and once to navigate out of the group of tabs</li>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> or <span class="keycap">←</span>/<span class="keycap">→</span> - previous/next tab.</li>									
			</ul>
		</td>
		<td>
			<ul>
				<li>This is for 'application' tabs that change without loading a new page. If a menu looks like a group of tabs, but is actually a group of links to different pages, <span class="keycap">Tab</span> and <span class="keycap">Enter</span> are more appropriate.</li>
				<li>The tab content should update automatically when pressing the arrow keys. You should not hit Enter to activate the tab.</li>
			</ul>
		</td>
	</tr>
	<tr>
		<td>'Tree' menu</td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - Navigate Previous/next menu option</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - expand/collapse submenu, move up/down one level.</li>
			</ul>
		</td>
		<td></td>
	</tr>
	<tr>						
		<td>Scroll </td>
		<td>
			<ul>
				<li><span class="keycap">↑</span>/<span class="keycap">↓</span> - scroll vertically</li>
				<li><span class="keycap">←</span>/<span class="keycap">→</span> - scroll horizontally</li>
				<li><span class="keycap">Spacebar</span>/<span class="keycap">Shift</span> + <span class="keycap">Spacebar</span> - scroll by page</li>
			</ul>
		</td>
		<td>
			<p>Minimize horizontal scrolling.</p>
		</td>
	</tr>
</tbody></table>

## Automatisert testing


## Andre ressurser
* [Lær mer om hvordan teste tastaturnavigasjon på Tilsynets veiledningssider.. ](https://uu.difi.no/krav-og-regelverk/kom-i-gang/hvordan-teste-universell-utforming-av-ditt-nettsted#tastaturnavigering)
