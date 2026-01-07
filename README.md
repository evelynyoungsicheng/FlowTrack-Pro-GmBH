# Datenrecht  — Statische Website

## Überblick
- Zweck: Universitätsprojekt-Website zu Themen des Daten- und IT‑Rechts mit den erforderlichen Rechts- und Datenschutzseiten.
- Umfang: Rein statische, clientseitige Website. Kein Backend, keine Datenbank.
- Seiten: Startseite, Über das Projekt, Kontakt, Datenschutzerklärung, Impressum, Barrierefreiheit, Lizenz.

## Live‑Hosting (GitHub Pages)
- Empfohlenes Hosting: GitHub Pages (Repository → Settings → Pages → Deploy from branch → `main` → `/`).
- Nach der Aktivierung ist die Seite unter `https://<username>.github.io/<repository>/` erreichbar.
- Falls bereits veröffentlicht, verwenden Sie die Pages‑URL des Repositories.

## Lokale Vorschau
Sie können die Seite direkt über [index.html](index.html) im Browser öffnen. Für realistischere Tests starten Sie einen lokalen Server:

```bash
# Option A: VS Code Live Server (empfohlen)
# Erweiterung "Live Server" installieren, dann Rechtsklick auf index.html → "Open with Live Server".

# Option B: Python 3 (eingebauter Server)
py -m http.server 5500
# oder, je nach Setup
python -m http.server 5500

# Option C: Node.js (statischer Server)
npx serve .
```

Anschließend http://localhost:5500 (oder die im Terminal ausgegebene URL) öffnen.

## Projektstruktur
- [index.html](index.html): Startseite
- [about.html](about.html): Hintergrund und Ziel des Projekts
- [contact.html](contact.html): Kontaktformular‑UI (ohne Funktion, siehe „Simulierte Prozesse“)
- [privacy.html](privacy.html): Datenschutzerklärung
- [impressum.html](impressum.html): Impressum
- [barrierefreiheit.html](barrierefreiheit.html): Erklärung zur Barrierefreiheit
- [license.html](license.html): Lizenz und Nutzungsbedingungen für Inhalte
- [style/styles.css](style/styles.css): Globale Styles
- [style/about.css](style/about.css), [style/contact.css](style/contact.css), [style/privacy.css](style/privacy.css), [style/impressum.css](style/impressum.css), [style/barrierefreiheit.css](style/barrierefreiheit.css), [style/license.css](style/license.css): Seitenspezifische Styles
- `img/`: Bilder und Icons

## Verwendete Technologien
- HTML5: Semantisches Markup und strukturierte Inhalte
- CSS3: Responsives Layout und seitenspezifisches Styling
- Keine JavaScript‑ oder Server‑Komponenten erforderlich

## Barrierefreiheit
- Ziel: Orientierung an WCAG 2.1 AA im Rahmen einer statischen Website.
- Ansatz: Semantisches HTML, aussagekräftige Seitentitel, beschreibende Linktexte und tastaturbedienbare Navigation.
- Details und bekannte Einschränkungen sind in [barrierefreiheit.html](barrierefreiheit.html) dokumentiert.

## Rechtliche Seiten
- Datenschutzerklärung: Siehe [privacy.html](privacy.html).
- Impressum: Siehe [impressum.html](impressum.html).
- Lizenz/Nutzungsbedingungen: Siehe [license.html](license.html).

## Simulierte Prozesse (Wichtig)
- Die Website erhebt, speichert oder verarbeitet keine personenbezogenen Daten.
- Das Kontaktformular und etwaige interaktive Elemente dienen nur der Demonstration; es werden keine Daten gesendet oder übertragen.

## Bearbeitung & Mitarbeit
- Globale Styles in [style/styles.css](style/styles.css) anpassen; seitenspezifische Styles in den jeweiligen Dateien unter `style/`.
- Assets in `img/` hinzufügen/ersetzen; bitte nur Materialien verwenden, für die Nutzungsrechte vorliegen.
- Überschriftenhierarchie einhalten (H1 → H2 → H3), Alt‑Texte für Bilder vergeben und ausreichende Farbkontraste sicherstellen.

## Lizenz & Quellenangaben
- Hinweise zur Lizenzierung der Inhalte und Assets finden sich in [license.html](license.html).
- Bei Drittinhalten bitte Quellenangabe und Lizenzhinweise in der Lizenzseite oder beim Asset ergänzen.

## Hinweise für Prüfer:innen
- Dies ist ein statisches Lehrprojekt zur akademischen Bewertung.
- Bitte interne Verlinkungen prüfen, Lesbarkeit und Kontrast bewerten sowie die Auffindbarkeit von Barrierefreiheit‑ und Rechtsseiten über die Navigation verifizieren.



