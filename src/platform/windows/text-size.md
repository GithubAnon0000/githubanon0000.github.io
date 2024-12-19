# Textgröße

Sollten Sie der Meinung sein, dass die Textgröße inkorrekt ist, können Sie
versuchen, zwei Umgebungsvariablen zu verändern:

- ANKI_NOHIGHDPI=1 wird so manche high dpi Unterstützung von Qt deaktivieren.

- ANKI_WEBSCALE=1 wird die Skalierung von Ankis Webviews verändern. Hierunter
  zählen die Stapelübersicht, der Lernbildschirm usw. Andere Elemente der
  Benutzeroberfläche (wie beispielsweise das Menu) werden hiervon nicht
  beeinflusst. Ersetzen Sie 1 mit der gewünschten Skalierung, wie beispielsweise
  1.5 oder 0.75.

Bei Windows können Sie dies zu einer Batch Datei hinzufügen, sodass es einfacher
ist, Anki mit diesen Einstellungen zu öffnen. Erstellen Sie beispielsweise eine
Datei mit dem Namen startanki.bat auf ihrem Desktop mit dem folgenden Inhalt:
```
set ANKI_WEBSCALE=0.75
start "Anki" "C:\Program Files\Anki\anki"
```

Nach dem Speichern, können Sie hierauf doppelklicken um Anki mit diesen
Einstellungen zu starten.
