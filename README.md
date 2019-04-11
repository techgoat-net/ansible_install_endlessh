## Playbook um endlessh zu installieren

### Features ###
* es wird sichergestellt, dass die benötigten Programme installiert sind
* Installation der Pakete unabhängig vom Paketmanager
* Prüfung ob die Binary bereits existiert   
  * falls nicht, wird das github-Repo geklont, die Binary kompilliert und anschließend verschoben
* Prüfung ob bereits eine `screen`-Session läuft
  * falls nicht, wird eine entsprechende `screen`-Session gestartet


**Aufruf:**
```
$ ansible-playbook -i <inventory-Datei> playbook.yml
```