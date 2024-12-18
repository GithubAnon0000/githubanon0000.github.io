# Wayland

Seit Anki 2.1.48 können Sie Anki dazu zwingen, Wayland zu verwenden, indem Sie
ANKI_WAYLAND=1 definieren, bevor Sie Anki starten. Wayland bietet möglicherweise
eine bessere Darstellung über mehrere Bildschirme hinweg, ist allerdings
aufgrund der nachfolgenden Probleme standardmäßig deaktiviert:

- Bei manchen Distros werden Fenster ohne Rahmen dargestellt.
- Es ist nicht möglich, Fenster in den Vordergrund zu holen. Beispielsweise ist
  es dadurch nicht möglich auf _Hinzufügen_ zu klicken, um das bereits
  vorhandene _Neue Karten hinzufügen_ Fenster anzuzeigen.
