## Playbook um endlessh zu installieren

siehe [Techgoat.net](https://techgoat.net)-Artikel: [Ein TARPIT erstellen](https://techgoat.net/index.php?id=168)

### Features ###
* es wird sichergestellt, dass die benötigten Programme installiert sind
* Installation der Pakete unabhängig vom Paketmanager
* Prüfung ob die Binary bereits existiert   
  * falls nicht, wird das github-Repo geklont, die Binary kompilliert und anschließend verschoben
* Prüfung ob bereits eine `screen`-Session läuft
  * falls nicht, wird eine entsprechende `screen`-Session gestartet
* Es lassen sich viele Werte bequem in der entsprechenden `group_vars` Datei setzen

**Aufruf:**
```
$ ansible-playbook -i <inventory-Datei> playbook.yml
```
