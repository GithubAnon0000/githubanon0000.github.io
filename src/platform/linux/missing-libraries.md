# Fehlende Bibliotheksdateien

Sollte Anki nicht starten können, führen Sie es bitte im Terminal mit `anki`
aus. Wenn es Sie darüber informiert, dass Bibliotheksdateien fehlen, dann
installieren Sie diese bitte und versuchen Sie es erneut.


Wenn Anki Ihnen mitteilt, dass keine Plattform verfügbar ist, dann starten Sie
Anki bitte mit dem folgenden Befehl:

```shell
QT_DEBUG_PLUGINS=1 anki
```

Dies sollte Auskunft über eine fehlende Bibliotheksdatei geben.

Nachdem Sie die fehlenden Bibliotheksdateien mit `apt-get` oder ähnlichem
installiert haben, führen Sie den obigen Prozess erneut aus. Möglichweise müssen
Sie dies einige Male wiederholen, bevor alle notwendigen Bibliotheksdateien
installiert sind.
