# Durch Linux Distros verteilte Packete

Die Anki Versionen, die durch Linux Distros verteilt werden, sind teilweise
modifiziert worden. Wir konnten einige Probleme feststellen, die auf diese
Modifikationen zurückzuführen sind:

- Anki ist von Drittanbieter-Bibliotheksdateien wie Qt abhängig. Linux Distros
  ersetzen diese häufig mit anderen Versionen dieser Bibliotheksdateien, ohne
  die Auswirkungen hiervon zu überprüfen.
- Manchmal ist die Anki Version, die durch Linux Distros zur Verfügung gestellt
  wird, mehrere Jahre alt oder es handelt sich um alpha/beta Versionen, die
  nicht für die normale Nutzung gedacht sind. Außerdem wird oft die eingebaute
  Überprüfung für Software-Aktualisierungen deaktiviert. Hierdurch werden Sie
  nicht benachrichtigt, wenn neue Anki Versionen veröffentlicht werden.

Kompilierte Anki Versionen stehen unter <https://apps.ankiweb.net> zur
Verfügung. Die meisten Bibliotheksdateien, die von Anki benötigt werden, sind in
diesen bereits enthalten. Außerdem wurde Anki mit diesen Bibliotheksdateien
getestet. Wenn Sie Probleme mit der Anki Version haben, die durch Linux Distros
verteilt wird, dann sollten Sie zunächst überprüfen, ob die Probleme
verschwinden, wenn Sie die aktuelle und offizielle Anki Version verwenden.

Sie können gerne die Anki Version weiterverwenden, die durch ihr Linux Distro
verteilt wird. Sollten allerdings Probleme auftreten, müssten Sie diese Probleme
an die Packetverwalter Ihres Distros melden.
