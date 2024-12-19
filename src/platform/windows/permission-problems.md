# Windows Probleme mit Berechtigungen

<!-- toc -->

## Probleme mit Berechtigungen

Sollten Sie "Zugriff verweigert" Nachrichten erhalten, könnte es sein, dass
manche Dateien von Anki im Nur-Lese-Modus sind, was bedeutet, dass sie
schreibgeschützt sind.

Um das zu lösen, können Sie das nachfolgende machen:

- In der Suchleiste in der Startleiste von Windows, tippen Sie cmd.exe und
  drücken Sie Enter.
- In dem Fenster, dass sich öffnet, tippen Sie das folgende ein, um Ihren
  Nutzernamen anzuzeigen:

```
whoami
```

- Tippen Sie das folgende und drücken Sie Enter nach jeder Zeile un ersetzen Sie
  ____ mit Ihrem Nutzernamen aus dem vorherigen Befehl. Der Teil mit _:F_ muss
  beibehalten werden.

```
cd %APPDATA%
icacls Anki2 /grant ____:F /t
```

Dieser Befehl sollte die Berechtigungen für Ankis Datenordner korrigieren und
Sie sollten Anki nun nutzen können.

## Antivirus/Firewall/Anti-Malware

Manche Nutzer berichten von "Zugriff verweigert" oder "schreibgeschützt"
Fehlern, die durch Sicherheitssoftware ausgelöst worden sind. Sie möchten
vielleicht eine Ausnahme für Anki einrichten oder die Software vorübergehend
deaktivieren, um diese Möglichkeit auszuschließen. Manche Nutzer haben
berichtet, dass das Ausschalten dieser Software alleine nicht geholfen hat.
Sie mussten dann Anki entweder auf eine Ausnahmeliste hinzufügen oder die
Software deinstallieren.

## Fehlersuche bei Berechtigungsproblemen

Sollten die Probleme weiterhin bestehen, nachdem Sie die Antiviren- und
verwandte Programme ausgeschlossen haben, und Sie die obigen Schritte zum
Korrigieren der Berechtigungen durchgeführt haben und sollten Sie nicht OneDrive
verwenden, dann führen Sie bitte die folgenden Befehle in cmd.exe aus und
drücken Sie Enter nach jeder Zeile.

```
whoami
cd %APPDATA%
icacls Anki2 /t
```
Kopieren Sie dann bitte was Sie sehen in die Zwischenablage und fügen Sie es in
unserem Supportforum ein. Alternativ können Sie auch ein Bildschirmfoto machen.
