# Startprobleme unter Windows

<!-- toc -->

## Kein Fehler, aber App erscheint nicht

Wenn Sie Anki starten, aber Anki nicht erscheint und keine Fehlernachricht
angezeigt wird, dann können Sie das Nachfolgende versuchen:

- Mehrere/Externe Bildschirme entfernen.
- Installieren Sie die [neueste Anki Version](https://apps.ankiweb.net/).
- Ändern Sie [Ihr Dezimaltrennzeichen
  ](https://forums.ankiweb.net/t/windows-update-broke-anki/1822/75), falls
  dieser kein Punkt sein sollte.
- Installieren Sie die alte [2.1.35-alternate Version
  ](https://github.com/ankitects/anki/releases/tag/2.1.35) von Anki.

## Windows Updates

Wenn Anki startet, erhalten Sie vielleicht eine Fehlernachricht wie die
folgenden:

- _Error loading Python DLL_
- _The program can't start because api-ms-win.... is missing_
- _Failed to execute script runanki_
- _Failed to execute script pyi_rth_multiprocessing_
- _Failed to execute script pyi_rth_win32comgenpy_

Diese Fehler treten für gewöhnlich auf, da Ihr Computer ein Windows Update
benötigt oder Windows Bibliotheksdateien fehlen.

Öffnen Sie bitte Windowaktualisierung und gehen Sie sicher, dass Ihr System alle
Aktualisierungen installiert hat. Sollten Aktualisierungen installiert worden
sein, starten Sie ihr Gerät bitte neu.

## Windows 7/8

Unter Windows 7/8, müssen Sie vielleicht zusätzliche Aktualisierungen manuell
vornehmen. Versuchen Sie bitte:

- <https://www.microsoft.com/en-us/download/details.aspx?id=48234>
- <https://aka.ms/vs/15/release/vc_redist.x64.exe>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4474419>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4490628>

## Video driver Probleme

Lesen Sie bitte [Anzeigeprobleme](./display-issues.md).

## Mehrere Bildschirme

Wenn Sie den Fehler _LoadLibrary failed with error 126_ erhalten, könnte das
daran liegen, dass das Toolkit, welches Anki verwendet, Probleme mit [mehreren
Bildschirmen](https://forums.ankiweb.net/t/error-126-on-open-anki-desktop/13967)
hat.

## Antivirus/Firewall Programme

Drittanbieterprogramme können Anki daran hindern, ausgeführt zu werden. Sie
können versuchen eine Ausnahme für Anki hinzuzufügen oder die Antivirus/Firewall
vorübergehend zu deaktivieren.

## Administrator Zugang

Manche Nutzer haben berichtet, das Anki erst dann funktioniert hat, als sie
einen Rechtsklick auf das Anki Icon ausgeführt haben und _Als Administrator
ausführen_ ausgewählt haben. Anki speichert alle Daten in Ihrem Nutzerordner und
sollte keine Administratorrechte benötigen, allerdings können Sie dies
versuchen, wenn alles andere nicht funktioniert hat.

## Mehrere Anki Installationen nach einer Aktualisierungen vorhanden

Sollten nach der Aktualisierung mehrere Anki Versionen installiert sein (z. B.
in `C:\Program Files\Anki` und `C:\Program Files (x86)\Anki`), dann kann es
sein, dass Anki deshalb nicht mehr startet und keine Fehlernachricht anzeigt.

Versuchen Sie, alle Kopien von Anki zu deinstallieren. Hierzu gehen Sie zu
Windows Einstellungen > Anwendungen & features (oder Apps > Installierte
Anwendungen) und and deinstallieren. Sie können auch `uninstall.exe` in jedem
Anki Programmordner ausführen. Anschließend installieren Sie Anki erneut.

## Fehlersuche

Anki vom Terminal aus zu starten, kann einige zusätzliche Informationen über
Fehler offenlegen. Nachdem Sie die neueste Anki Version installiert haben und
sichergestellt haben, dass alle Windowaktualisierungen installiert sind, drücken
Sie die <kbd>Windows</kbd> Taste (oder öffnen Sie das Startmenü), tippen Sie
`cmd` und führen Sie die Kommandozeile aus. Wenn das Terminalfenster erscheint,
kopieren Sie den folgenden Befehl hinein und tippen Sie <kbd>Enter</kbd>
(Der Pfad könnte anders sein, wenn Anki an einem Ort installiert worden ist, der
nicht der Standardort ist).

```
%LocalAppData%\Programs\Anki\anki-console.bat
```

Vermutlich wird Anki weiterhin nicht starten, allerdings können nun wichtige
Informationen im Terminalfenster erscheinen, die darüber Auskunft geben, was
das Problem verursacht.

## Wenn nichts funktioniert

Sollten Sie Anki weiterhin nicht starten können, obwohl Sie die obigen Schritte
zur Fehlerbehebung durchgeführt haben, haben Sie zwei weitere Optionen:

- Sie können Anki [mit Python ausführen
  ](https://faqs.ankiweb.net/running-from-python.html).
- Sie können eine ältere Anki Version versuchen, die ein älteres Toolkit
  verwendet, wie beispielsweise [2.1.35-alternate
  ](https://github.com/ankitects/anki/releases/tag/2.1.35) oder [2.1.15
  ](https://github.com/ankitects/anki/releases/tag/2.1.15).
