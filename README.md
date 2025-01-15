# ZHAW IUNR Template

LaTeX-Vorlage für studentische Arbeiten am Institut für Umwelt und Natürliche Ressourcen (IUNR) der Zürcher Hochschule für Angewandte Wissenschaften (ZHAW).
Die Vorlage basiert auf https://gpmpublic.zhaw.ch/GPMDocProdDPublic/Vorgabedokumente_Dept/N_AA_Writing_student_assignments.pdf

## Inhalt
- `zhaw_template.tex`: Hauptdatei des Dokuments, in der der Inhalt der Arbeit geschrieben wird. Diese Datei lädt automatisch die Präambel und weitere Einstellungen.
- `preamble_zhaw.tex`: Präambeldatei mit den wichtigsten Einstellungen und Formatierungsanweisungen, anpassbar
- Bibliothek.bib: Bibliografie aus Zotero exportiert mit Better Bibtex, automatische Synchronisierung möglich siehe Anleitung https://retorque.re/zotero-better-bibtex/
## Features
- **Kapitel, Abschnitte und Unterabschnitte** fortlaufend nummeriert.
- unterschiedliche **Kopf- und Fusszeilen** für gerade und ungerade Seiten (eher für Print)
- Automatische Erstellung von Verzeichnissen wie Inhalts-, Abbildungs- und Tabellenverzeichnissen.
- Einbindung eines **Literaturverzeichnisses** mit BibLaTeX.
- Einfache Anpassung von Schriftart, Abständen und weiteren Formatierungen.

## Verwendung

1. **Klonen des Repositories:**
   ```bash
   git clone https://github.com/ptrgslr/zhaw_iunr_template.git

2. LaTeX-Compiler verwenden:
Für das Literaturverzeichnis muss biblatex verwendet werden.
Hauptdatei bearbeiten: Text in der Datei zhaw_template.tex schreiben, bei Bedarf die Einstellungen in preamble_zhaw.tex anpassen.

3. Anpassungen
Präambel
Die Datei preamble_zhaw.tex enthält zentrale Einstellungen wie:

Schriftart (Standard: serifenlos wie Arial)
Seitenränder
Zeilenabstand
Definitionen für Kopf- und Fußzeilen
Einstellungen für Verzeichnisse (Inhalts-, Abbildungs-, Tabellen- und Literaturverzeichnis)
Kapitelstruktur

4. Befehle in zhaw_template.tex, um Abschnitte zu erstellen:
   \section{}: Abschnitt
   \subsection{}: Unterabschnitt
   \subsubsection{}: Unter-Unterabschnitt

5. Verzeichnisse
Die Vorlage erstellt automatisch:
Inhaltsverzeichnis mit \tableofcontents
Abbildungsverzeichnis mit \listoffigures
Tabellenverzeichnis mit \listoftables
Literaturverzeichnis mit \printbibliography


6. Beispiel
```r
\documentclass[a4paper,12pt,twoside]{article}
\input{preamble_zhaw}

\begin{document}

\input{titlepage} % Titelblatt

\section{Einleitung}
blablabla

\section{Methoden}
blablabla

\section{Ergebnisse}
blablabla

\section{Diskussion}
blablabla

\printbibliography % Literaturverzeichnis

\end{document}
```
## Lizenz
This project is licensed under the MIT License.
