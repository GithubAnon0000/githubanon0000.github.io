# Anzeigeprobleme unter Windows

<!-- toc -->

Unter Windows gibt es drei Möglichkeiten, Inhalte auf dem Bildschirm anzuzeigen.
Der Standard ist _software_, was am langsamsten aber kompatibelsten ist. Die
beiden anderen Optionen, _OpenGL_ und _ANGLE_, sind schneller. Allerdings
funktionieren diese gegebenenfalls nicht oder es treten Anzeigeprobleme auf.
Beispiele hierfür sind fehlende Menüleisten, leere Fenster und andere. Welche
dieser Optionen bei Ihnen am besten funktioniert, ist von Ihrem Computer
abhängig.

Sollten Anzeigeprobleme auftreten, können Sie zu _software_ wechseln, indem Sie
den nachfolgenden Befehl ausführen:

```bat
echo software > %APPDATA%\Anki2\gldriver6
```

Oder Sie nutzen stattdessen PowerShell:

```powershell
echo software > $env:APPDATA\Anki2\gldriver6
```

Dies wird nichts anzeigen. Anschließend starten Sie Anki neu.

Um zum Standardverhalten zurück zu wechseln, ändern Sie `software` zu `auto`
oder löschen Sie diese Datei.

In Anki 23.10+, können Sie die Grafikkartentreiber auch von den Einstellungen
aus ändern.

## Vollbild

Anki 2.1.50+ enthält einen Vollbildmodus, welcher allerdings aufgrund von
einigen Problemen deaktiviert werden musste, wenn `OpenGL` verwendet wird.
Wird stattdessen `software` verwendet (wie oben beschrieben), dann kann die
Vollbildfunktion verwendet werden. Beachten Sie jedoch, dass die
Anzeigegeschwindigkeit dadurch leiden könnte.

In Anki 23.10+ wird Vollbild mit dem standard Direct3D Driver unterstützt.
