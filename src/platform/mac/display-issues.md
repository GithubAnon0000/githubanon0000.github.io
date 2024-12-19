# Anzeigeprobleme unter macOS

<!-- toc -->

## Qt6 Video Driver

Sollten Sie Anzeigeprobleme oder Abstürze in Anki 23.10+ erleben, können Sie
versuchen, die Video Driver in den Einstellungen zu ändern. Anschließend starten
Sie Anki neu.

Ältere Anki Versionen bieten keine Möglichkeit, dies in den Einstellungen
ändern. Stattdessen können Sie die Terminal.app öffnen und den unteren Befehl
einfügen. Führen Sie den Befehl aus, indem Sie die Enter Taste drücken.

```
echo software > ~/Library/Application\ Support/Anki2/gldriver6
```

Dies wird keinen Text anzeigen. Anschließend starten Sie Anki neu.

Möchten Sie wieder zum Standardwert zurückwechseln, ändern Sie `software` zu
`auto` oder entfernen Sie die Datei.

## eGPUs

Sollte Anki Ihnen leere Fenster anzeigen, während Sie eine externe Grafikkarte
verwenden, dann drücken Sie Strg+Klick auf die Anki App. Drücken Sie
anschließend auf "Informationen" und aktivieren Sie die "eGPU bevorzugen"
Option.

## Bildschirme mit unterschiedlicher Auflösung

Lesen Sie hierfür bitte [diesen englischen Forenpost
](https://forums.ankiweb.net/t/mac-known-issues-wording-suggestion/7331).
