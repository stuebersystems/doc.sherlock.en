![Build status](https://ci.appveyor.com/api/projects/status/t0s34bkrdwvc9ouh?svg=true)

# CONFIRE SHERLOCK Documentation

This is the German documentation for [CONFIRE SHERLOCK](https://sherlock.stueber.co.uk). The documentation is Open Source and we have implemented it using [MkDocs](https://www.mkdocs.org) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material). Push-Requests in the master-branch are triggered in [AppVeyor](https://www.appveyor.com) so that each change is published automatically.

## Install MkDocs for Windows

1. Install [Python](https://www.python.org). Go to the [Python downloads page](https://www.python.org/downloads/) and download the latest version for Windows. For example, for Version 3.7.2 this would be the link: [Windows x86-64 executable installer](https://www.python.org/ftp/python/3.7.2/python-3.7.2-amd64.exe).

2. Start the installer and follow the on-screen instructions.

3. Run the command prompt as Administrator.

4. Enter the command `python --version` and `pip --version` to check the Python installation. In both cases a version number should appear as an output in the command prompt.

5. Enter the command `pip install mkdocs` to insteall the Python-Package MkDocs.

6. Final test: Enter the command `mkdocs --version`. A version nummer in the command prompt will let you know if everything has been installed correctly.

## Clone Repository

This repository is a Git-Repository. To clone the repository on a local commputer you will need a Git client. Either install [Git for Windows](https://gitforwindows.org/) and use the command prompt or install one of the many GUIs. We recommend [GitHub Desktop](https://desktop.github.com) or [SourceTree](https://www.sourcetreeapp.com).

1. Create a local directory for the documentation e.g. `c:\docs\sherlock`.

2. Open the command prompt and change to directory `c:\docs\sherlock`.

3. Enter the command `git clone https://github.com/stuebersystems/doc.sherlock.de.git` to clone the repository.

## Download Repository as Zip Archive

Willst du mit Git erstmal nichts zu tun haben, kannst Du das Repository auch als Zip-Archiv herunterladen:

1. Öffne die URL `https://github.com/stuebersystems/doc.sherlock.de` in deinem Webbrowser

2. Klicke auf die Schaltfläche `Clone or download` und dann auf `Download ZIP`.

3. Entpacke das Zip-Archiv in einen lokalen Ordner Deiner Wahl, z.B. `c:\docs\sherlock`.

## Mit MkDocs arbeiten

Du hast Python und das Package MkDocs installiert, Du hast dieses Repository geklont oder als Zip-Archiv heruntergeladen. Jetzt kannst Du die Dokumentation lokal auf deinem Rechner generieren:

1. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\sherlock`.

2. Tippe den Befehl `mkdocs build` ein. Die CONFIRE SHERLOCK Dokumentation wird neu generiert.

3. Um Dir das Ergebnis anzeigen zu lassen, tippe den Befehl `mkdocs serve` ein und öffne die Url `http://127.0.0.1:8000` in Deinem Webbrowser.

Das Inhaltsverzeichnis findest Du in der Datei `mkdocs.yml`, die einzelnen Kapitel im Unterordner `docs`. 

## Weitere Informationen

+ [Alles zum Thema Git](https://git-scm.com/book/de/v2)
+ [MkDocs Overview](https://www.mkdocs.org/#overview)

## Kann ich mithelfen?

Ja, sehr gerne. Der beste Weg mitzuhelfen ist es, Rückmeldung per Issue-Tracker zu geben und/oder Korrekturen per Pull-Request zu übermitteln.

## Code of conduct (Verhaltensregeln)

In diesem Projekt wurde der [STÜBER SYSTEMS Code of conduct](https://www.stueber.de/code-of-conduct.php) übernommen.
