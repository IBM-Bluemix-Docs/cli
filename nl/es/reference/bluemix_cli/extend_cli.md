---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Ampliación de la CLI de {{site.data.keyword.Bluemix_notm}} con plug-ins
{: #plug-ins}

La CLI de {{site.data.keyword.Bluemix_notm}} da soporte a una infraestructura de plug-in para ampliar su capacidad. Puede instalar un plug-in desde un repositorio, un URL web, o instalar un binario del plug-in de forma local. 

[Repositorio de plug-ins de CLI de {{site.data.keyword.Bluemix_notm}}](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![Icono de enlace externo](../../../icons/launch-glyph.svg) es el repositorio oficial para alojar los plugins.

## Instale un plugin desde el repositorio

* Busque el plug-in

  Utilice el mandato 'bluemix plugin repo-plugins -r REPO_NAME' para buscar un plugin en el repositorio.
  
  La CLI de {{site.data.keyword.Bluemix_notm}} tiene el repositorio oficial con el nombre `Bluemix` configurado de forma predeterminada. Puede listar los plug-ins en el repositorio oficial de `Bluemix` como se indica a continuación.

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* Instale el plug-in

  Utilice 'bx plugin install PLUGIN_NAME -r REPO_NAME' para instalar el plugin, por ejemplo:

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## Instale un plug-in de forma local

  Utilice el mandato `bluemix plugin install LOCAL_FILE_NAME` para instalar un binario de plugin-in en su máquina local, por ejemplo

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## Instalar desde un URL web

  Utilice el mandato `bluemix plugin install URL` para instalar un plugin directamente desde un URL web, por ejemplo

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


Para obtener más mandatos para gestionar plug-ins, ejecute `bluemix plugin` para ver los mensajes de ayuda.
