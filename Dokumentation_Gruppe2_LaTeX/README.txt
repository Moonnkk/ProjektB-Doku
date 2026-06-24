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

Noch auszufuellen (im Quelltext rot als [..] markiert)
------------------------------------------------------
- Matrikelnummern aller vier Teammitglieder (titlepage.tex)
- Name des Studiengangsleiters (master.tex, Makro \DerStudiengangsleiter)
- Ort fuer die Ehrenwoertliche Erklaerung (ewerkl.tex)

Hinweise zur Abgabe
-------------------
- Projekt A: Fuer den Datenbank-Import nur db/users.sql verwenden
  (db/init_databases.sql ist veraltet).
- Projekt A: Die beiden Demo-Konten UdoErdmann / UdoAdmin sind noch
  nicht im SQL-Dump enthalten. Kapitel 8 (Installation und Zugangsdaten)
  enthaelt fertige INSERT-Statements (Passwort: AbgabeGruppe2), die nach
  dem Import auszufuehren sind - oder die Konten ueber die Registrierung
  anlegen und im Admin-Bereich hochstufen.
