---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# {{site.data.keyword.Bluemix_notm}}-CLI herunterladen und installieren
{: #download_install}

Sie können das [Installationsprogramm](#installers) oder die [Shell](#shell_install) verwenden, um die {{site.data.keyword.Bluemix_notm}}-CLI zu installieren.

## Installationsprogramme herunterladen
{: #installers}

Rufen Sie die Seite [Alle Versionen](all_versions.html){: new_window} auf, um das aktuellste Installationsprogramm für Ihr Betriebssystem herunterzuladen.

Führen Sie unter Mac OS und Windows einfach das Installationsprogramm aus. 
Für Linux müssen Sie nach dem Herunterladen des Pakets mit dem Installationsprogramm die Dateien aus diesem Paket extrahieren und das Installationsscript mit Rootberechtigung ausführen.

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## Über Shell installieren
{: #shell_install}


### Mac OS

Kopieren Sie den folgenden Befehl und fügen Sie ihn auf einem Terminal Ihres Mac OS ein und führen Sie ihn aus.

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

Kopieren Sie den folgenden Befehl und fügen Sie ihn auf einem Terminal Ihres Linux-Betriebssystems ein und führen Sie ihn aus.

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

Kopieren Sie den folgenden Befehl und fügen Sie ihn in eine [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window}-Terminalkonsole ein und führen Sie ihn aus.

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

