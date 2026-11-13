# Hinweise für Claude

Persönliche One-Page-Website: reines HTML/CSS/JS, keine Build-Tools, kein Backend. Deploy über GitHub Actions (`.github/workflows/pages.yml`) bei Push auf `main`. Live unter `mario.aininger.com`.

## README und Wiki aktuell halten (wichtig)

Die `README.md` ist die einzige Quelle für das interne Wiki (`marioaininger-bot/wiki`). Das Wiki zieht sie jede Nacht vom Branch `main`, schreibt sie aber nie selbst um. Veraltet die README, veraltet das Wiki.

**Passe die README im selben Commit an, wenn du Folgendes änderst:**

- **Deployment** (Workflow, Pages-Einstellung) oder **Domain** (`CNAME`)
- **Technik** der Seite, etwa wenn ein Build-Schritt, ein Backend oder eine externe Quelle dazukommt
- Dann zusätzlich im Wiki-Repo `docs/architektur.md` und `docs/betrieb/accounts.md` nachtragen.

Reine Textänderungen an der Seite brauchen keine README-Änderung.

## Regeln

- Keine Build-Tools und keine Abhängigkeiten einführen, ohne es zu begründen und in der README zu vermerken.
- **Nie Geheimnisse in Dateien schreiben.**
- Die Seite ist öffentlich und persönlich: nichts Privates in Texte, Metadaten, `sitemap.xml` oder Bilder (auch nicht in Bild-Metadaten) aufnehmen.
- Sprache der Doku: Deutsch (Österreich).
