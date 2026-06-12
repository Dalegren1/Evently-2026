Innehåll


index.html — sidans struktur (header, hero, filter, events-grid, benefits, footer)
style.css — all styling


Teknik

Ren HTML & CSS, ingen byggprocess eller paketberoenden.


Layout: Flexbox och CSS Grid (events-grid och benefits-grid)
Namnkonvention: BEM (block__element--modifier)
Färger: oklch()-värden via CSS custom properties
Typografi: Skalbar via clamp() för rubriker, variabler för storlekar och vikter
Responsivitet: Media queries vid 1024px (tablet) och 480px/640px (mobil), ingen mobile-first-strategi


CSS-struktur

Filen är uppdelad i kategorier i ordning:


Variabler
Reset & bas
Typografi
Layout (.container)
Knappar
Formulär
Header / navbar
Hero
Filter-sektion
Events grid & kort
Benefits-sektion
Footer


Kända begränsningar / medvetna avgränsningar


Inga JS-funktioner — formulär, sök och "spara evenemang"-hjärtan är visuella, ej funktionella
Footer kollapsar till en kolumn under 640px; hamburgermeny för navbar är inte byggd (samma princip skulle kunna tillämpas på footern i en senare iteration)
--gray-950 och --gray-900 har identiska värden — troligen en kvarvarande dubblett, påverkar inget visuellt


Tillgänglighet


Semantiska landmärken (header, nav, main, footer) med aria-label där flera nav-element finns
Alla dekorativa SVG-ikoner har aria-hidden="true"
Ikon-knappar har aria-label
Bilder har beskrivande alt-texter
<time datetime=""> används för datum i events-grid