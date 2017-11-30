---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.Bluemix_notm}}-CLI mit Plug-ins erweitern
{: #plug-ins}

Die {{site.data.keyword.Bluemix_notm}}-CLI unterstützt ein Plug-in-Framework zur Erweiterung der verfügbaren Funktionalität. Sie können ein Plug-in aus einem Repository oder über eine Web-URL installieren oder eine Plug-in-Binärdatei lokal installieren. 

Das [{{site.data.keyword.Bluemix_notm}}-CLI-Plug-in-Repository](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![Symbol für externen Link](../../../icons/launch-glyph.svg) ist das offizielle Repository zum Hosten der Plug-ins.

## Plug-in aus Repository installieren

* Suchen Sie das Plug-in.

  Verwenden Sie den Befehl 'bluemix plugin repo-plugins -r REPO_NAME', um ein Plug-in im Repository zu suchen.
  
  In der {{site.data.keyword.Bluemix_notm}}-CLI ist standardmäßig das offizielle Repository mit dem Namen `Bluemix` konfiguriert. Sie können die Plug-ins im offiziellen `Bluemix`-Repository wie folgt auflisten.

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* Installieren Sie das Plug-in.

  Verwenden Sie zum Installieren des Plug-ins den Befehl 'bx plugin install PLUGIN_NAME -r REPO_NAME'. Beispiel:

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## Plug-in lokal installieren

  Verwenden Sie den Befehl `bluemix plugin install LOCAL_FILE_NAME`, um eine Plug-in-Binärdatei auf der lokalen Maschine zu installieren. Beispiel:

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## Installation über Web-URL ausführen

  Verwenden Sie den Befehl `bluemix plugin install URL`, um ein Plug-in direkt über eine Web-URL zu installieren. Beispiel:

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


Wenn Sie weitere Informationen zu den Befehlen zur Verwaltung von Plug-ins benötigen, dann führen Sie den Befehl `bluemix plugin` aus, um die Hilfenachrichten anzuzeigen.
