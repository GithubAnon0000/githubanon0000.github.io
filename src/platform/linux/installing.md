# Installation & Aktualisierung von Anki unter Linux

<!-- toc -->

## Voraussetzungen

Die Paketversion erfordert ein aktuelles 64-Bit Intel/AMD Linux mit glibc und
üblichen Bibliotheksdateien wie libwayland-client und systemd. Sollten Sie eine
andere Architektur verwenden (z. B. ARM/AArch64) oder ein minimales Linux
Distro, dann können Sie die Paketversion nicht verwenden. Stattdessen können Sie
die [Python wheels](https://betas.ankiweb.net/#via-pypipip) Version nutzen.

Debian und Derivate, wie beispielsweise Ubuntu und [Chromebooks mit aktiviertem
Linux](https://support.google.com/chromebook/answer/9145439?),
führen bitte das Nachfolgende vor der Installation von Anki aus:

```shell
sudo apt install libxcb-xinerama0 libxcb-cursor0 libnss3
```

Sollte Anki nach der Installation nicht starten, fehlen Ihnen vielleicht
[weitere Bibliotheksdateien](./missing-libraries.md).

Wenn Sie Ubuntu 24.04 verwenden und Anki nicht startet, lesen Sie bitte
[diesen englischen Forenpost]
(https://forums.ankiweb.net/t/issues-running-on-ubuntu-24-04/40974).

Ankis Buildsystem unterstützt nur glibc; auf musl basierende Distros werden
gegenwärtig nicht unterstützt.

## Installation

Um Anki zu installieren:

1. Laden Sie Anki von <https://apps.ankiweb.net> in Ihren Downloads Ordner
   herunter.
2. Wenn zstd nicht bereits installiert ist, müssen Sie es installieren
   (z. B. `sudo apt install zstd`).
3. Öffnen Sie ein Terminalfenster und führen Sie die folgenden Befehle aus.
   Bitte ersetzen Sie dabei den Dateinamen entsprechend.

```shell
tar xaf Downloads/anki-2XXX-linux-qt6.tar.zst
cd anki-2XXX-linux-qt6
sudo ./install.sh
```

Bei manchen Linuxsystemen werden Sie gegebenenfalls
`tar xaf --use-compress-program=unzstd` nutzen müssen.

4. Anschließend können Sie Anki starten, indem Sie 'anki' eintippen und Enter
   drücken. Lesen Sie bitte die Links auf der linken Seite, falls Probleme
   auftreten.

## Aktualisierung

Wenn Sie Anki in der Vergangenheit von einer .deb/.rpm/usw. Datei ausgeführt
haben, entfernen Sie bitte die Systemversion, bevor Sie das hier bereitgestellte
Paket installieren.

Wenn Sie die Aktualisierung von einem früheren Paket durchführen, wiederholen
Sie einfach die Installationsschritte, um auf die neueste Version zu
aktualisieren. Ihre Nutzerdaten bleiben dabei erhalten.

Möchten Sie ein Downgrade zu einer älteren Version durchführen, folgenden Sie
bitte den [Downgrade Anweisungen](http://changes.ankiweb.net).

## Kompatibilität von Erweiterungen

Manche Erweiterungen funktionieren nicht immer mit der neuesten Anki-Version.
Wenn Sie Anki zur neuesten Version aktualisiert haben und eine für Sie
essentielle Erweiterungen nicht mehr funktioniert, können Sie eine ältere
Anki-Version von der
[Veröffentlichungsseite](https://github.com/ankitects/anki/releases)
herunterladen.

## Probleme

Wenn bei der Installation oder beim Starten von Anki Probleme auftreten, lesen
Sie bitte die folgenden Seiten:

- [Fehlende Bibliotheksdateien](missing-libraries.md)
- [Anzeigeprobleme](display-issues.md)
- [Leeres Hauptfenster](blank-window.md)
- [Linux Distro Pakete](distro-packages.md)
- [Falsches GTK Thema](gtk-theme.md)
- [Wayland](wayland.md)
- [Eingabemethoden](input-methods.md)
