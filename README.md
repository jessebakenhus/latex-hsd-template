# LaTeX-Template: Hausarbeit / Projektdokumentation (HSD)

Wiederverwendbares LaTeX-Template mit Titelseite, APA-Zitierweise (biblatex-apa) und automatischem KI-Verzeichnis.

## Benutzung

1. Metadaten (Titel, Autoren, Modul, Betreuer, ...) im Block `METADATEN` in `template.tex` anpassen.
2. Optional Logo als `hsd-logo.png` in den Ordner legen und `\logodatei` anpassen.
3. Inhalt ab dem Block `INHALT` ersetzen, Literatur in `lib.bib` pflegen.
4. Kompilieren: `pdflatex` -> `biber` -> `pdflatex` -> `pdflatex`

## KI-Verzeichnis

Mit `\KIfn{Tool}{Prompt}{Verwendungszweck}` wird eine Fußnote gesetzt und die Zeile automatisch in die Tabelle am Ende übernommen. Nach Floats (Abbildungen, Listen) `\KIfntext{...}{...}{...}` verwenden.

## Dateien

- `template.tex` – das Template
- `lib.bib` – Beispiel-Literaturdatei
