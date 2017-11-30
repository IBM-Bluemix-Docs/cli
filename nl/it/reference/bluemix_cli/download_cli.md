---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Scarica e installa la CLI {{site.data.keyword.Bluemix_notm}}
{: #download_install}

Puoi utilizzare il [programma di installazione](#installers) o la [shell](#shell_install) per installare la CLI {{site.data.keyword.Bluemix_notm}}.

## Scarica i programmi di installazione
{: #installers}

Vai alla pagina [Tutte le versioni](all_versions.html){: new_window} per scaricare il programma di installazione più recente del tuo sistema operativo.

Per macOS e Windows, esegui solo il programma di installazione. 
Per Linux, dopo che hai scaricato il pacchetto del programma di installazione, eseguine l'estrazione ed esegui lo script di installazione con l'autorizzazione root.

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## Installa dalla shell
{: #shell_install}


### macOS

Copia e incolla il seguente comando in un terminale del tuo macOS ed eseguilo.

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

Copia e incolla il seguente comando in un terminale del tuo sistema operativo Linux ed eseguilo.

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

Copia e incolla il seguente comando in una console del terminale [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} ed eseguilo.

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

