## Anzeigeprobleme unter Linux

Die Hardware Beschleunigung ist standardmäßig aktiviert. Sollten Sie Probleme
wie leere Fenster oder andere Anzeigeprobleme feststellen, können Sie versuchen,
Software-Rendering zu aktivieren. Öffnen Sie hierfür ein Terminalfenster und
tippen Sie das folgende ein:

```
echo software > ~/.local/share/Anki2/gldriver6
```

Möchten Sie wieder zu dem Standardwert zurückwechseln, dann ändern Sie bitte
`software` zu `auto` oder entfernen Sie die Datei.

In Anki 23.10+ können Sie die Grafikkartentreiber außerdem in den
Einstellungen ändern.
