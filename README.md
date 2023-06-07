# Dokumentation des WaldorfConnect-Projekts

> Durch Versionierung in einem [Git](https://de.wikipedia.org/wiki/Git)-Repository machen wir Änderungen an der Dokumentation nachvollziehbar.

## Organisatorische Dokumentation: [Organisation.md](Organisation.md)

## Technische Dokumentation: [Dokumentation.md](Dokumentation.md)

---

## Hinweise zum Bearbeiten der Dokumente  `(.md)`

Die Dokumente mit der Datei-Endung ".md" sind in [Markdown](https://de.wikipedia.org/wiki/Markdown) geschrieben, so dass wir sie ganz einfach mit Texteditoren oder Entwicklungsumgebungen bearbeiten und in eine Versionskontrolle (z.B. Git) einpflegen können.

- GitHub bietet eine [Dokumentation zur Grundlegenden Schreib- und Formatierungssyntax mit vielen Beispielen](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) an.
- bei Verwendung des Texteditors `Visual Studio Code` ist die Extension `Markdown All in One` empfehlenswert

## Hinweise zum Bearbeiten der Diagramme `(.drawio)`

- die Diagramme sind mit dem kostenlosen Open-Source Zeichenprogramm [draw.io](https://www.drawio.com/) erstellt.
- die Diagramme sind im Format .drawio.svg, d.h. es sind `drawio`-Dateien, die man so bearbeiten kann und gleichzeitig `svg`-Dateien die man als Bild einbinden kann.
- bei Verwendung des Texteditors `Visual Studio Code` bietet sich die Extension `Draw.io Integration` an, mit der man die Diagramme direkt dort im Texteditor bearbeiten kann.
- die in den Diagrammen verwendeten Elemente stammen aus dem vom [Fraunhofer IESE ](https://de.wikipedia.org/wiki/Fraunhofer-Institut_f%C3%BCr_Experimentelles_Software_Engineering_IESE) entwickelten [Architecture Decomposition Framework (ADF)](https://www.iese.fraunhofer.de/blog/softwarearchitekturen-einfacher-designen-und-verstaendlicher-dokumentieren-mit-dem-fraunhofer-adf/).
  - um die Elemente in der Online-Version von diagrams.net auszuprobieren kann man [diesen Link](https://app.diagrams.net/?splash=0&libs=general&clibs=Uhttps%3A%2F%2Fraw.githubusercontent.com%2Farchitecture-decomposition-framework%2Fadf-diagramsnet%2Fmain%2Flibraries%2FADF_SW%40RT.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Farchitecture-decomposition-framework%2Fadf-diagramsnet%2Fmain%2Flibraries%2FADF_Env%40RT.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Farchitecture-decomposition-framework%2Fadf-diagramsnet%2Fmain%2Flibraries%2FADF_SW%40DT.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Farchitecture-decomposition-framework%2Fadf-diagramsnet%2Fmain%2Flibraries%2FADF_Env%40DT.xml) verwenden
  - um die Elemente auf dem eigenen Computer im Draw.io Programm verfügbar zu machen, muss man die XML-Dateien im Ordner `Diagramme/adf-elements/libraries/` als Libraries laden, via `File -> Open library`
  - um die Elemente auf dem eigenen Computer in `Visual Studio Code` in der `Draw.io Integration` einzubinden, muss man in VS Code in die `File -> Preferences -> Settings` gehen, oben rechts die JSON-Ansicht aktivieren und die Einstellungen einfügen (nicht alles ersetzen!), die unter `Diagramme/adf-elements/settingsForLinux.txt` bzw. `settingsForWindows.txt` zu finden sind (die Pfadtrenner sind unterschiedlich: `/` <-> `\\`)
    - WICHTIG: die Pfade musst du so anpassen! (du kannst hier z.B. in VS Code auf die entsprechende Datei im Ordner `Diagramme/adf-elements/libraries/` rechtsklicken > `Copy path`)
    - ein Beispiel für eine vollständige VSCode Settings Datei liegt unter `Diagramme/adf-elements/settingsForLinuxFullExample.txt`
    - HINWEIS: Wenn auch nur ein Pfad nicht stimmt oder es sonst einen Fehler im JSON gibt, startet die `Draw.io Integration` Extension überhaupt nicht.
    - TIPP:  nachhaltige Lösung: verschiebe die 4 XML-Dateien an irgendeinen anderen Ort auf deinem PC - sonst ist die Funktionsfähigkeit der `Draw.io Integration` daran gekoppelt, dass du niemals dieses Projekt verschiebst oder löschst.
  - in Draw.io können die Elemente dann in der Palette links hinzugefügt werden durch Klicken auf `+ More Shapes` > `undefined` auswählen > `Apply`