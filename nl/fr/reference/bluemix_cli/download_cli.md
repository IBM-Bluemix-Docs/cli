---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Téléchargement et installation de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}
{: #download_install}

Vous pouvez utiliser [installer](#installers) ou [shell](#shell_install) pour installer l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

## Téléchargement des programmes d'installation
{: #installers}

Accédez à la page contenant [toutes les versions](all_versions.html){: new_window} pour télécharger le dernier programme d'installation de votre système d'exploitation.

Pour Mac OS et Windows, exécutez simplement le programme d'installation. 
Pour Linux, après avoir téléchargé le package du programme d'installation, procédez à l'extraction de son contenu et exécutez le script d'installation avec les droits root.

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## Installation depuis un interpréteur de commandes
{: #shell_install}


### Mac OS

Copiez et collez la commande suivante vers un terminal Mac OS et exécutez-la.

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

Copiez et collez la commande suivante vers un terminal Linux et exécutez-la.

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

Copiez et collez la commande suivante dans une console de terminal [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} et exécutez-la.

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

