# Arkboy Homepage

Die Funnel-Seite von **Arkboy Operations** — eine einzige, eigenständige HTML-Datei (`index.html`).
Kein Build, kein Framework, keine Abhängigkeiten außer Google Fonts. Datei öffnen genügt.

## Inhalt

| Datei | Zweck |
|---|---|
| `index.html` | Die komplette Seite: Markup, CSS, JavaScript und die beiden Aufnahmen als Data-URI |

## Aufbau der Seite

Hero → Laufband (Leistungen) → 01 Die Lücke → Statement-Streifen → 02 Das Modell →
03 Wer operiert → 04 Der Plan (5 Schritte) → Risiko-Umkehr → 05 Für wen → 06 Fragen (17 in drei Gruppen) →
Abschluss-Block → Fuß.

Inhaltlich speist sich die Seite aus dem Pitchdeck (Stages 01–04). Bewusst draußen: jede Bepreisung
und die Onboarding-Agenda. Das Prinzip „Ich verdiene erst, wenn du verdienst" steht ohne Zahlen drin.

## Gestaltung

- **Grund `#000`, Signalfarbe `#A7FF9C`** — genau eine Signalfarbe, fest. Sie läuft über vier
  CSS-Variablen (`--signal`, `--signal-ink`, `--signal-wash`, `--signal-hair`) in `:root`.
  Eine neue Farbe ist eine Änderung an vier Zeilen.
- **Schrift:** Inter Tight (700/300) für den Fließtext, IBM Plex Mono für Labels und Kennzahlen.
- **Systematik:** Geisterziffern je Sektion, stehende Schiene links mit Sektionsnummer,
  Asymmetrie als Prinzip (Spaltenversätze), Laufband unter dem Hero, Odometer auf den Kennzahlen.
- **Responsiv:** Umbruchpunkte bei 1279 / 960 / 900 / 700 / 600 / 480 px;
  `prefers-reduced-motion` schaltet Animationen ab.

### Aufnahmen in Sektion 03

Zwei Studioaufnahmen, als WebP (q92, zusammen ~78 KB) eingebettet. Regeln bei Änderungen:

- **Keine Filter** — keine Entsättigung, keine Aufhellung, keine Tonung, keine Blend-Ebene.
- **Kein Beschnitt** — Flexbox 40/60 im Verhältnis der Seitenverhältnisse, gleiche Höhe ohne `cover`.
- **Nur ein Verlauf** nach unten ins Schwarz (`mask-image`, ab 58 %; mobil ab 72 %).

## Veröffentlichen

GitHub Pages: Settings → Pages → Branch `main`, Ordner `/ (root)`.
`index.html` wird dann direkt unter der Repo-URL ausgeliefert.

## Offen

- Kein Impressum und keine Datenschutzerklärung — vor einer öffentlichen Domain nötig.
- Das Pitchdeck nennt in Stage 03 noch die entfernten Zahlen und die alte Signalfarbe `#FF6831`.
- „Arkboy Web Design v1.0" (PDF) nennt weiterhin `#FF6831` als Signalfarbe; für die Website gilt `#A7FF9C`.
