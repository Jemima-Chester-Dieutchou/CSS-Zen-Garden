
# CSS Zen Garden – Autumn Editorial

## 1. Projektbeschreibung

Dieses Projekt ist eine individuelle Gestaltung der Website **CSS Zen Garden**. Ziel ist es, die Möglichkeiten von CSS zu zeigen und eine bestehende HTML-Seite durch ein eigenständiges Design visuell aufzuwerten.

Das Design trägt den Namen **Autumn Editorial**. Es orientiert sich an den Farben und der Atmosphäre des Herbstes und verbindet warme Farbtöne mit einer modernen, redaktionellen Gestaltung.

Die HTML-Struktur bleibt unverändert. Die Gestaltung erfolgt über das externe Stylesheet `style.css`.

## 2. Projektziele

- Entwicklung eines harmonischen und kreativen Herbstdesigns
- Gestaltung einer klaren und gut lesbaren Seitenstruktur
- Verwendung moderner CSS-Techniken
- Gestaltung von Karten, einer Sidebar und einem individuellen Footer
- Ergänzung visueller Effekte und Animationen
- Berücksichtigung unterschiedlicher Bildschirmgrößen
- Verbesserung der Kenntnisse in CSS, Layoutgestaltung und responsivem Webdesign

## 3. Verwendete Technologien

- **HTML5:** Vorgegebene Struktur der Website
- **CSS3:** Layout, Farben, Typografie, Animationen und Effekte
- **Google Fonts:** Einbindung der Schriftarten Fraunces und Inter
- **CSS Grid:** Anordnung von Inhalten in Spalten und Rasterlayouts
- **CSS Gradients:** Gestaltung von Farbverläufen
- **CSS Pseudo-Elemente:** Dekorative Elemente und zusätzliche Beschriftungen
- **CSS Keyframes:** Animationen der Blätter und des Erscheinens von Inhalten
- **Media Queries:** Anpassung an verschiedene Bildschirmgrößen und reduzierte Bewegung

## 4. Designkonzept und Farbpalette

Das Design verwendet eine warme, herbstliche Farbpalette. Terrakotta, Rostrot, Orange und Senfgelb werden mit cremefarbenen Flächen und dunklen Textfarben kombiniert.

| Farbe | Hex-Code | Verwendung |
|---|---|---|
| Terrakotta | `#B95735` | Überschriften, Akzente und Links |
| Dunkles Terrakotta | `#A9472C` | Farbverläufe und Hintergründe |
| Orange | `#D97745` | Akzente und Farbverläufe |
| Senfgelb | `#E4AA22` | Hervorhebungen und Buttons |
| Gold | `#D9B65D` | Dekorative Elemente |
| Cremeweiß | `#FFFDF8` | Karten und helle Flächen |
| Dunkelbraun | `#494039` | Fließtext |
| Beige | `#EFE3D2` | Hintergrund der Seite |

Der Hintergrund kombiniert mehrere radiale Farbverläufe. Dadurch entsteht eine warme, weiche Atmosphäre, die zum Herbstthema passt.

## 5. Typografie

Für die Website werden zwei Schriftarten verwendet:

- **Fraunces:** Eine Serifenschrift für Überschriften und ausgewählte Designelemente.
- **Inter:** Eine serifenlose Schrift für Fließtexte und kleinere Beschriftungen.

Die Kombination schafft einen Kontrast zwischen einer ausdrucksstarken Überschriftengestaltung und einer gut lesbaren Textdarstellung.

Die Größe der Hauptüberschriften wird teilweise mit `clamp()` angepasst, sodass sie sich flexibel an die Bildschirmbreite anpassen kann.

## 6. Gestaltung der einzelnen Bereiche

### 6.1 Einleitung – Intro

Der Intro-Bereich erhält einen warmen Terrakotta-Orange-Farbverlauf, abgerundete Ecken und einen weichen Schatten.

Weitere Gestaltungselemente sind:

- große, responsive Überschrift
- goldener Farbverlauf im Überschriftentext
- dekorativer Kreis im Hintergrund
- goldene Linie über der Hauptüberschrift
- animiertes Erscheinen der Überschrift und weiterer Inhalte

### 6.2 Textbereich – Preamble

Der Preamble-Bereich wird als halbtransparente Karte gestaltet. Ein dezenter Rahmen, abgerundete Ecken und ein Unschärfeeffekt sorgen für eine zusätzliche visuelle Ebene.

Der erste Buchstabe des ersten Absatzes wird mit `::first-letter` vergrößert und goldfarben hervorgehoben.

### 6.3 Inhaltskarten

Die Inhaltsbereiche erhalten helle, cremefarbene Hintergründe, abgerundete Ecken und dezente Schatten.

Die einzelnen Abschnitte werden durch farbige obere Rahmen unterschieden:

- Explanation: Terrakotta
- Participation: Senfgelb
- Benefits: Orange
- Requirements: Rostrot

Beim Darüberfahren mit der Maus bewegen sich die Karten leicht nach oben und erhalten einen stärkeren Schatten.

### 6.4 Sidebar

Die Sidebar wird mit einem Terrakotta-Orange-Farbverlauf gestaltet. Sie enthält halbtransparente Karten für die Designauswahl, Archive und Ressourcen.

Weitere Details:

- goldfarbene Überschriften
- dekorative Emojis als Icons
- feine Trennlinien zwischen Listeneinträgen
- Hover-Effekte für Links
- hervorgehobener Button für die Archivnavigation
- Sticky-Positionierung auf größeren Bildschirmen

### 6.5 Herbstblätter

Sechs dekorative Blattelemente ergänzen das Herbstthema.

Die Blätter werden als SVG-Grafik direkt im CSS eingebunden. Unterschiedliche Größen, Farben, Unschärfeeffekte und Animationszeiten sorgen für Abwechslung.

Zwei Animationen werden verwendet:

- `chute`: Bewegt die Blätter von oben nach unten.
- `balance`: Lässt die Blätter seitlich schwingen und rotieren.

Über `prefers-reduced-motion` werden die Animationen deaktiviert, wenn das Betriebssystem reduzierte Bewegung bevorzugt.

### 6.6 Footer

Der Footer erhält einen hellen Farbverlauf, abgerundete Ecken und einen Schatten.

Die Links werden als einzelne Kacheln in einem Raster angeordnet. Zusätzliche Beschriftungen werden über CSS-Pseudo-Elemente ergänzt.

Beim Darüberfahren mit der Maus ändern die Kacheln ihre Hintergrund- und Textfarbe und bewegen sich leicht nach oben.

## 7. Responsives Design

Das Stylesheet enthält eine Media Query für Bildschirmbreiten bis 800 Pixel.

In diesem Bereich wird das Layout der äußeren `.page-wrapper`-Struktur auf eine Spalte umgestellt. Außerdem werden bestimmte Positionierungen angepasst, damit die Inhalte auf kleineren Bildschirmen besser dargestellt werden können.

Die Überschriftengrößen werden teilweise flexibel über `clamp()` definiert.

## 8. Projektstruktur

```text
CSS-Zen-Garden/
├── index.html
├── style.css
└── README.md
```

- `index.html`: Vorgegebene HTML-Struktur
- `style.css`: Individuelles Design und sämtliche CSS-Gestaltungen
- `README.md`: Dokumentation des Projekts

## 9. Projekt starten

1. Das Repository lokal öffnen oder herunterladen.
2. Die Datei `index.html` in einem Webbrowser öffnen.
3. Die Gestaltung in `style.css` bearbeiten und speichern.
4. Die Website im Browser aktualisieren, um Änderungen zu überprüfen.

Für die Entwicklung kann ein Editor wie Visual Studio Code verwendet werden.

## 10. Versionsverwaltung mit Git

Git wird zur Versionsverwaltung des Projekts verwendet. Änderungen können schrittweise gespeichert und anschließend zum GitHub-Repository übertragen werden.

Beispiel für den Arbeitsablauf:

```bash
git status
git add style.css
git commit -m "Improve autumn CSS design"
git push
```

Nach Abschluss der Dokumentation kann auch die README-Datei separat hinzugefügt und übertragen werden.

## 11. Lernfortschritt

Im Rahmen dieses Projekts werden unter anderem folgende Kenntnisse angewendet und vertieft:

- CSS Grid und Layoutgestaltung
- Farbverläufe und Transparenzeffekte
- Schriftgestaltung mit Google Fonts
- Pseudo-Elemente und CSS-Selektoren
- Hover-Effekte und Transitionen
- Keyframe-Animationen
- Responsive Design mit Media Queries
- Strukturierte Dokumentation mit Markdown
- Versionsverwaltung mit Git und GitHub

## 12. Projektstatus

Das Projekt befindet sich in der Gestaltungs- und Dokumentationsphase. Die CSS-Datei enthält das individuelle Herbstdesign. Weitere Anpassungen und Tests können im Rahmen der Fertigstellung vorgenommen werden.
