---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Ampliamento della CLI {{site.data.keyword.Bluemix_notm}} con i plug-in
{: #plug-ins}

La CLI {{site.data.keyword.Bluemix_notm}} supporta un framework di plug-in per ampliarne la funzionalità. Puoi installare un plug-in da un repository, un URL web o installare un file binario del plug-in localmente. 

[Il repository di plug-in della CLI {{site.data.keyword.Bluemix_notm}} ](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![Icona link esterno](../../../icons/launch-glyph.svg)è il repository ufficiale per ospitare i plug-in.

## Installa un plug-in dal repository

* Cerca il plug-in

  Utilizza il comando 'bluemix plugin repo-plugins -r NOME_REPOSITORY' per cercare i plug-in nel repository.
  
  La CLI {{site.data.keyword.Bluemix_notm}} ha il repository ufficiale con il nome `Bluemix` configurato per impostazione predefinita. Puoi elencare i plug-in nel repository `Bluemix` ufficiale come di seguito.

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Acquisizione dei plugin dal repository 'Bluemix' in corso...

  Repository: Bluemix
  Nome           Descrizione                                        Versioni
  auto-scaling   Plug-in CLI Bluemix per il servizio Auto-Scaling   0.2.1, 0.2.2
  nsg            Plug-in Bluemix Network Security Group             0.1.1

  ```

* Installa il plug-in

  Utilizza 'bx plugin install NOME_PLUGIN -r NOME_REPOSITORY' per installare il plug-in; ad esempio:

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Ricerca di 'auto-scaling' dal repository 'Bluemix'...
  9857792 byte scaricati
  Installazione del plug-in '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2' in corso...
  OK
  Il plug-in 'auto-scaling 0.2.2' è stato installato correttamente.
  ```

## Installa un plug-in localmente

  Utilizza il comando `bluemix plugin install NOME_FILE_LOCALE` per installare un file binario del plug-in nella macchina locale; ad esempio:

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installazione del plug-in './auto-scaling-darwin-amd64-0.2.2' in corso...
  OK
  Il plug-in 'auto-scaling 0.2.2' è stato installato correttamente.
  $
  ```

## Installa da un URL web

  Utilizza il comando `bluemix plugin install URL` per installare un plug-in direttamente da un URL web; ad esempio

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Tentativo di scaricare il file binario in corso...
  9857792 byte scaricati
  Installazione del plug-in '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2' in corso...
  OK
  Il plug-in 'auto-scaling 0.2.2' è stato installato correttamente.
  ~$
  ```


Per ulteriori comandi per gestire i plug-in, esegui `bluemix plugin` per visualizzare i messaggi della guida.
