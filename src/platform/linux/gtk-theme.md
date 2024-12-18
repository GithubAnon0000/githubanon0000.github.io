# Anki übernimmt das GTK Thema unter Gnome/Linux nicht

Sie können dieses Problem umgehen, indem Sie Anki explizit mitteilen, welches
das GTK Thema ist. Führen Sie hierfür die nachfolgenden Befehle im Terminal aus:

```shell
theme=$(gsettings get org.gnome.desktop.interface gtk-theme)
echo "gtk-theme-name=$theme" >> ~/.gtkrc-2.0
echo "export GTK2_RC_FILES=$HOME/.gtkrc-2.0" >> ~/.profile
```

Anschließend melden Sie sich an Ihrem Computer ab und wieder an. Anki sollte nun
das richtige GTK Thema verwenden.
