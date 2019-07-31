# NinaReleases

> **Note:** If you came here from one of my other public repositories: This repository is used to provide my sister Nina with a piece of software that I wrote for her. My sister is a jouranlist and needs to copy and paste some information from the internet and put it in a given format every week. So I wrote this software that does exactly that for her, but in 2 minutes instead of 2 hours ;) The following docs are meant to help her to install the software.

## Anleitung

### Schritt 1: Java installieren

Zur Ausführung des Programms benötigt man die aktuellste Version von Java.
Die kann hier runtergeladen werden: [Download](https://www.java.com/de/).

### Schritt 2: Programm runterladen

Um das Programm runterzuladen oben auf den grünen Button "Clone or Download" und dann auf "Download ZIP" klicken.
Das .zip-File muss auf dem Computer entpackt werden.

### Schritt 3: Chrome runterladen und aktualisieren

Der "Roboter" benutzt Chrome um die Seite aufzurufen und "durchzulesen". Wenn du das also noch nicht getan hast,
solltest du jetzt die neuste Version herunterladen: [Download](https://www.google.de/chrome/browser/desktop/).
Falls du irgendeine Version von Chrome bereits installiert hast, solltest du in den Einstellungen prüfen, ob du
ein Update runterladen kannst.

### Schritt 4: ChromeDriver runterladen und in das Verzeichnis legen

Der ChromeDriver kann die Befehle von meinem Programm in Befehle, die Chrome versteht übersetzen. Du kannst den
[hier](https://sites.google.com/a/chromium.org/chromedriver/downloads) runterladen. Einfach auf den Link neben
"Latest Release" klicken und dann auf `chromedriver_win32.zip`. Die Datei musst du bei dir entpacken. Da ist eine
`chromedriver.exe` drin, mit der du erstmal nichts machen kannst. Wichtig ist nur, dass du die in das gleiche
Verzeichnis legst, wie die `Nina.jar` und die `*.properties` Dateien.

### Schritt 5: Ausführen des Programms

Wenn du alles richtig gemacht hast, müsste sich nach einem Doppelklick auf
die Nina.jar ein Browserfenster von Google Chrome öffnen. Wenn du jetzt kurz
wartest, sollte sich das nach wenigen Minuten wieder schließen.

### Schritt 6: Ergebnisse

Das Programm legt die Ergebnisse in einer .txt Datei in genau dem Ordner ab, in dem es gestartet wurde. Die Zahl vor dem .txt sind die vergangenen Millisekunden seit dem 1.1.1970. Das ist einfach nur, damit die Dateien einander nicht überschreiben. Wenn man die nicht mehr braucht, können die .txt-Dateien aber auch ohne Weiteres gelöscht werden. Die Zusammenfassung für das Wochenende findest du ganz unten in der Datei.

### Schritt 7: .properties Dateien

In der `telNummern.properties` befinden sich die Kinos mit den dazugehörigen Telefennummern. Bei jedem Programmaufruf guckt das Programm in die Datei um die Telefonnummern einzutragen. Wenn sich die Nummer eines Kinos ändert, kann man das in der Datei nachpflegen. Das Programm trägt dann fortan die neue Nummer ein. Die Namen der Kinos müssen die gleichen sein wie auf kino.de, aber ohne Leerzeichen. Also `Mein Kino` ist in der Datei `MeinKino`.

In der `namen.properties` sind die Anzeigenamen der Kinos eingetragen. Angezeigt wird der Wert rechts vom ":". Der linke Wert darf nie verändert werden.

In der `ads.properties` sind die ids einiger Elemente der Seite eingetragen, die den Programmfluss stören und deswegen zur Laufzeit entfernt werden. Um die Datei zu öffnen, eignet sich jeder TextEditor, wie Notepad.
