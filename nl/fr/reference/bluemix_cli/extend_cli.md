---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Extension de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} avec des plug-ins
{: #plug-ins}

L'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} prend en charge une structure de plug-in destinée à étendre ses fonctionnalités. Vous pouvez installer un plug-in depuis un référentiel, une URL WEB, ou installer localement un fichier binaire de plug-in. 

Le [référentiel de plug-ins d'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![Icône de lien externe](../../../icons/launch-glyph.svg) est le référentiel officiel d'hébergement des plug-ins.

## Installation d'un plug-in à partir d'un référentiel

* Recherche du plug-in

  Utilisez la commande 'bluemix plugin repo-plugins -r REPO_NAME' pour rechercher un plug-in dans le référentiel.
  
  L'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} comporte le référentiel officiel `Bluemix` configuré par défaut. Vous
pouvez afficher la liste des plug-ins du référentiel `Bluemix` officiel en procédant comme suit :

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* Installation du plug-in

  Utilisez la commande 'bx plugin install PLUGIN_NAME -r REPO_NAME' pour installer le plug-in, par exemple :

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## Installation locale d'un plug-in

  Utilisez la commande `bluemix plugin install LOCAL_FILE_NAME` pour installer un fichier binaire de plugin dans votre machine locale. Par exemple :

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## Installation depuis une URL Web

  Utilisez la commande `bluemix plugin install URL` pour installer un plug-in directement à partir d'une URL Web. Par exemple :

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


Pour découvrir d'autres commandes de gestion de plug-ins, exécutez `bluemix plugin` afin d'afficher les messages d'aide.
