Projektdokumentation Gruppe2 - LaTeX-Quellen
============================================

Inhalt
------
master.tex            Hauptdatei (hier kompilieren)
titlepage.tex         Titelseite
ewerkl.tex            Ehrenwoertliche Erklaerung
acronyms.tex          Abkuerzungsverzeichnis
introduction.tex      Einleitung
a1_referenz.tex ...   Teil I  - Projekt A (GuardX), Kapitel
a7_installation.tex
b1_ueberblick.tex ... Teil II - Projekt B (SunShine Tours), Kapitel
b5_installation.tex
conclusion.tex        Fazit
bibliography.bib      Literaturquellen
img/logo.jpg          DHBW-Mannheim-Logo (Titelseite)
master.pdf            Bereits kompilierte Fassung

Kompilieren
-----------
Voraussetzung: TeX-Live/MiKTeX mit biber sowie deutschen Sprachpaketen.

Einfachster Weg:
    latexmk -pdf master.tex

Manuell:
    pdflatex master
    biber    master
    pdflatex master
    pdflatex master
