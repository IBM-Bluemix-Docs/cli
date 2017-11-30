---

copyright:

  years: 2017

lastupdated: "2017-06-29"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# IBM Developer Tools per Visual Studio Code
{: #ibm-dev-tools-for-vscode}

IBM Developer per Visual Studio Code è un'estensione per l'editor che fornisce l'accesso alle funzionalità della CLI IBM Developer direttamente all'interno del riquadro comandi dell'editor di Visual Studio Code.  Ti consente di accedere rapidamente a un sottoinsieme di comandi `bx dev` sia per i flussi di lavoro Docker che CloudFoundry, che includono la distribuzione dell'applicazione, l'avvio/arresto/riavvio di applicazioni in Bluemix, la visualizzazione dei log di applicazioni remote e altro ancora, il tutto senza la necessità di uscire dal contesto dell'editor.
{:shortdesc}

![Acquisizione della schermata di download dell'estensione IBM Developer Tools.](ibm-dev-tools-for-vscode.png "Schermata di download dell'estensione in Visual Studio Code")

## Dipendenze
{: #dependencies}

Per utilizzare l'estensione IBM Developer Tools per Visual Studio Code, sul tuo sistema dovrai installare anche la [CLI Bluemix](https://plugins.ng.bluemix.net/ui/home.html) e il plug-in [CLI IBM Developer](/docs/cloudnative/dev_cli.html).

## Installazione
{: #installation}

Il modo più semplice per installare l'estensione IBM Developers Tools è quello di utilizzare il comando 'quick open' di Visual Studio Code:

1. apri il riquadro comandi 'quick open' utilizzando la seguente combinazione di tasti dall'interno dell'editor:

  * **Mac:** `cmd + p`
  * **Windows / Linux:** `ctrl + p`

2. Immetti il comando `ext install ibm-developer` e premi Invio per installare l'estensione IBM Developer Tools all'interno dell'editor Visual Studio Code.

In alternativa, puoi installare l'estensione IBM Developer Tools attraverso il pannello di gestione "Extensions":

1. Apri la barra laterale **Extensions** nell'editor Visual Studio Code ed effettua la ricerca utilizzando la stringa `publisher:IBM Developer`.  L'estensione IBM Developer Tools verrà visualizzata nei risultati della ricerca.  
2. Fai clic sul pulsante **Install** per avviare l'installazione.

Puoi anche accedere all'[estensione IBM Developer Tools direttamente da Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer).


## Utilizzo
{: #usage}

Puoi richiamare i comandi dell'estensione utilizzando il riquadro comandi di Visual Studio Code.

Per prima cosa, apri il riquadro comandi utilizzando la seguente combinazione di tasti:

* **Mac:** `cmd + shift + p`
* **Windows / Linux:** `ctrl + shift + p`

Successivamente, immetti o seleziona il comando da richiamare. Puoi digitare ‘bx’ all'interno del riquadro comandi per visualizzare l'elenco di tutti i comandi disponibili. 

### Utilizzo dell'estensione IBM Developer per i flussi di lavoro Docker (contenitori Docker)
{: #usage-docker}

Puoi iniziare a utilizzare i flussi di lavoro bx dev in pochi passi:
* Crea un progetto utilizzando uno dei due metodi indicati di seguito:
  * Utilizza la [console web Bluemix](https://console.ng.bluemix.net/developer/getting-started/) e scarica il codice generato
  * Utilizza la [CLI Bluemix Developer](/docs/cloudnative/dev_cli.html) e genera un progetto utilizzando il comando `bx dev create`
* Apri la cartella del progetto in locale nell'editor Visual Studio Code
* Utilizza il comando `bx dev build` per creare l'applicazione in un'immagine Docker
* Utilizza il comando `bx dev debug` per eseguire l'applicazione nel Docker locale per lo sviluppo
> Nota: per eseguire il debug di un'applicazione Node.js in esecuzione nel contenitore Docker locale, dovrai [aggiungere una configurazione di debug per il contenitore locale](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container).
* Utilizza il comando `bx dev run` per eseguire l'applicazione nel Docker locale in modalità di rilascio
* Utilizza il comando `bx dev deploy` per distribuire l'applicazione a un runtime Cloud Foundry su Bluemix *(il supporto per IBM Container sarà presto disponibile).*

### Utilizzo dell'estensione IBM Developer per i flussi di lavoro Cloud Foundry
{: #usage-cloud-foundry}

Per gli utenti che attualmente distribuiscono le applicazioni ai runtime Cloud Foundry su IBM Bluemix, forniremo supporto anche per la serie di operazioni `cf`.

Puoi iniziare a utilizzare i flussi di lavoro CloudFoundry in pochi passi
* Crea una nuova applicazione CloudFoundry
  * Utilizza la [console web](https://console.ng.bluemix.net/dashboard/cf-apps) e scarica il codice di starter
  * Crea una nuova applicazione CloudFoundry manualmente
* Apri la cartella del progetto in locale nell'editor Visual Studio Code
* Utilizza `bx cf apps` per elencare tutte le tue applicazioni
* Utilizza `bx cf push` per distribuire una creazione della tua applicazione al runtime Cloud Foundry
* Utilizza bx `cf <start/stop/restage/restart>` per modificare lo stato della tua applicazione
* Utilizza `bx cf logs` per visualizzare il flusso di log dal vivo per la tua applicazione
  * Utilizza `bx cf logs` per arrestare il flusso di log




