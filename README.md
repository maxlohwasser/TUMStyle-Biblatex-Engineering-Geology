# TUMStyle-Biblatex-Engineering-Geology
German BibLaTeX citation style for academic documents at the Chair of Engineering Geology, Technical University of Munich (TUM).
# TUMStyle

Ein deutschsprachiger BibLaTeX-Zitierstil für wissenschaftliche Arbeiten.

## Übersicht

TUMStyle ist ein benutzerdefinierter Zitierstil für LaTeX. Er legt die Formatierung von Kurzbelegen im Text sowie die Darstellung der Einträge im Literaturverzeichnis fest. Der Stil orientiert sich an den Anforderungen eines TUM-orientierten Lehrstuhls.

## Projektdateien

| Datei | Beschreibung |
|---|---|
| `tumstyle.bbx` | Definiert die Formatierung des Literaturverzeichnisses. |
| `tumstyle.cbx` | Definiert die Formatierung der Zitate im Text. |
| `Dokumentation.pdf` | Enthält Erläuterungen, Hinweise und Anwendungsbeispiele. |

## Installation und Einbindung

Lege die Dateien `tumstyle.bbx` und `tumstyle.cbx` im selben Verzeichnis wie die Hauptdatei deines LaTeX-Projekts ab. Alternativ kannst du sie in einem Verzeichnis speichern, das von deiner LaTeX-Installation durchsucht wird.

Binde anschließend `biblatex` in der Präambel ein:

```latex
\usepackage[ngerman]{babel}
\usepackage{csquotes}
\usepackage[backend=biber,style=tumstyle]{biblatex}
\addbibresource{literatur.bib}
```

Passe den Namen `literatur.bib` gegebenenfalls an den Namen deiner eigenen Literaturdatenbank an. Weitere Optionen für `biblatex` können je nach Projekt ergänzt werden.

## Kompilierung

Für die Erstellung des Literaturverzeichnisses wird Biber als Backend verwendet. Der übliche Kompilierablauf lautet:

1. LaTeX-Compiler ausführen.
2. Biber ausführen.
3. LaTeX-Compiler erneut ausführen (bei Bedarf ein weiteres Mal).

Der Zitierstil selbst ist grundsätzlich unabhängig vom LaTeX-Compiler und kann mit pdfLaTeX, LuaLaTeX oder XeLaTeX verwendet werden. Voraussetzung ist, dass das jeweilige Dokument und alle zusätzlich verwendeten Pakete mit dem gewählten Compiler kompatibel sind.

## Sprache

**Hinweis:** Der Zitierstil ist derzeit ausschließlich für deutschsprachige Dokumente ausgelegt. Eine Unterstützung weiterer Sprachen ist aktuell noch nicht implementiert, soll aber zu einem späteren Zeitpunkt geprüft und gegebenenfalls ergänzt werden.

## Dokumentation

Eine ausführlichere Beschreibung der Einbindung, der Zitierbefehle und der unterstützten Literaturtypen findest du in der Datei [`Dokumentation.pdf`](Dokumentation.pdf).

## Verwendung und Weiterentwicklung

Der Zitierstil wird fortlaufend gepflegt. Fehlerhinweise und Verbesserungsvorschläge sind willkommen.
