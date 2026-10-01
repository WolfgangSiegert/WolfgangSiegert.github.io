# WolfgangSiegert.github.io

Statische Hauptseite für die eigene Domain. Das vertikale Hauptportfolio bleibt als separates GitHub-Pages-Projekt unter `/portfolio/` erreichbar; die horizontale Vue-Alternative wird als Showcase unter `/portfolio-vue/` angeboten.

`portfolio-vue/` enthält den geprüften Produktionsbuild aus dem eigenständigen Repository `WolfgangSiegert/portfolio-vue`. Nach Änderungen dort `npm run build` ausführen und den Inhalt von `dist/` hier vollständig ersetzen.

Die Domain-Startseite verlinkt ausschließlich die Hauptansicht des Portfolios. Die horizontale Showcase-Variante wird über den Ansichtsschalter innerhalb des Portfolios geöffnet; die Auswahl wird nicht gespeichert, `/portfolio/` bleibt der Standard-Einstieg.

Die Hauptseite ist öffentlich und wird über GitHub Pages aus `main` veröffentlicht. Als eigene Domain ist `tiny-bits.org` hinterlegt. Sobald die DNS-Umstellung abgeschlossen ist, liegt das Portfolio unter `https://tiny-bits.org/portfolio/`.

`portfolio-traffic.js` erfasst auf den Produktionsdomains einen minimalen Seitenaufruf der Domain-Startseite. Derselbe Build liegt unter `portfolio-vue/`. Beide senden ausschließlich an den eigenen Laravel-Endpunkt `https://atm.tiny-bits.org/api/portfolio-traffic`; die private Statistik wird nicht in diesem öffentlichen Repository gespeichert oder angezeigt. Den Domain-Build erst veröffentlichen, nachdem der Endpunkt bereitsteht.
