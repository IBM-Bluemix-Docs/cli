---

copyright:

  years: 2017

lastupdated: "2017-06-29"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# IBM Developer Tools for Visual Studio Code
{: #ibm-dev-tools-for-vscode}

IBM Developer for Visual Studio Code est une extension de l'éditeur qui permet d'accéder aux fonctions à partir de l'interface de ligne de commande de développement IBM directement dans la palette de commandes de l'éditeur Visual Studio Code.  Vous pouvez ainsi accéder rapidement à un sous-ensemble de commandes `bx dev` pour les flux de travaux Docker et CloudFoundry, notamment le déploiement d'applications, le démarrage/l'arrêt/le redémarrage d'applications sur Bluemix, l'affichage de journaux d'applications distants, etc., le tout sans avoir à quitter le contexte de l'éditeur.
{:shortdesc}

![Capture d'écran illustrant l'écran de téléchargement de l'extension IBM Developer Tools.](ibm-dev-tools-for-vscode.png "Ecran de téléchargement de l'extension dans Visual Studio Code")

## Dépendances
{: #dependencies}

Pour utiliser l'extension IBM Developer Tools for Visual Studio Code, vous devez également installer le plug-in de l'[interface de ligne de commande Bluemix](https://plugins.ng.bluemix.net/ui/home.html) et de l'[interface de ligne de commande IBM Developer](/docs/cloudnative/dev_cli.html) sur votre système.

## Installation
{: #installation}

Le moyen le plus simple pour installer l'extension IBM Developers Tools consiste à utiliser la palette de commandes 'quick open' de Visual Studio Code :

1. Ouvrez la palette de commandes 'quick open' à l'aide de la combinaison de touches suivantes dans l'éditeur :

  * **Mac :** `cmd + p`
  * **Windows/Linux :** `ctrl + p`

2. Tapez la commande `ext install ibm-developer` et appuyez sur Entrée pour installer l'extension IBM Developer Tools dans l'éditeur Visual Studio Code.

Vous pouvez aussi installer l'extension IBM Developer Tools via le panneau de gestion "Extensions" :

1. Ouvrez la barre d'options latérale **Extensions** de l'éditeur Visual Studio Code, puis effectuez une recherche sur la chaîne `publisher:IBM Developer`.  L'extension IBM Developer Tools apparaît dans les résultats de la recherche;  
2. Cliquez sur le bouton **Install** pour lancer l'installation.

Vous pouvez également accéder à l'extension [IBM Developer Tools directement dans Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer).


## Syntaxe
{: #usage}

Vous appelez les commandes d'extension à l'aide de la palette de commandes de Visual Studio Code.

Commencez par ouvrir la palette de commandes en utilisant la combinaisons de touches suivante :

* **Mac :** `cmd + maj + p`
* **Windows/Linux :** `ctrl + maj + p`

Ensuite, tapez ou sélectionnez la commande que vous souhaitez appeler. Vous pouvez taper ‘bx’ dans la palette de commandes pour afficher la liste de toutes les commandes disponibles. 

### Utilisation des flux de travaux IBM Developer Extension for Docker (conteneurs Docker)
{: #usage-docker}

Vous pouvez vous familiariser avec les flux de travaux bx dev en quelques étapes seulement :
* Créez un projet en utilisant l'une des deux méthodes suivantes :
  * Utilisez la [console Web Bluemix](https://console.ng.bluemix.net/developer/getting-started/) et téléchargez le code généré.
  * Utilisez l'[interface de ligne de commande Bluemix Developer](/docs/cloudnative/dev_cli.html) et générez un projet à l'aide de la commande `bx dev create`.
* Ouvrez le dossier du projet localement dans l'éditeur Visual Studio Code.
* Utilisez la commande `bx dev build` pour générer l'application dans une image Docker.
* Utilisez la commande `bx dev debug` pour exécuter l'application dans un conteneur Docker local en mode développement.
> Remarque : pour déboguer une application Node.js qui s'exécute dans le conteneur Docker local, vous devez [ajouter une configuration de débogage pour le conteneur local](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container).
* Utilisez la commande `bx dev run` pour exécuter l'application dans un conteneur Docker local en mode édition.
* Utilisez la commande `bx dev deploy` pour déployer l'application dans un environnement d'exécution Cloud Foundry sur Bluemix *(IBM Container Support, bientôt disponible).*

### Utilisation des flux de travaux IBM Developer Extension for Cloud Foundry
{: #usage-cloud-foundry}

Pour les utilisateurs qui déploient actuellement des applications dans des environnements d'exécution Cloud Foundry sur IBM Bluemix, nous fournissons également du support pour les opérations `cf` set.

Vous pouvez vous familiariser avec les flux de travaux CloudFoundry en quelques étapes seulement :
* Créez une nouvelle application CloudFoundry.
  * Utilisez la [console Web](https://console.ng.bluemix.net/dashboard/cf-apps) et téléchargez le code de démarrage.
  * Créez une nouvelle application CloudFoundry manuellement.
* Ouvrez le dossier du projet localement dans l'éditeur Visual Studio Code.
* Utilisez `bx cf apps` pour afficher la liste de toutes vos applications.
* Utilisez `bx cf push` pour envoyer par commande push une génération de votre application sur l'environnement d'exécution Cloud Foundry.
* Utilisez bx `cf <start/stop/restage/restart>` pour modifier le statut de votre application.
* Utilisez `bx cf logs` pour afficher le flux de journalisation opérationnel pour votre application.
  * Utilisez `bx cf logs` pour arrêter le flux de journalisation.




