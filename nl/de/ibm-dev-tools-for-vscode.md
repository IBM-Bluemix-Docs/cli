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

IBM Developer Tools for Visual Studio Code ist eine Erweiterung für den Editor, die den Zugriff auf die Funktionen der IBM Developer-Befehlszeilenschnittstelle direkt in der Befehlspalette des Visual Studio Code-Editors zur Verfügung stellt.  Dies ermöglicht einen schnellen Zugriff auf ein Subset von `bx dev`-Befehlen für Docker- und Cloud Foundry-Workflows (wie z. B. Bereitstellen von Apps, Starten/Stoppen/Neustarten von Apps unter Bluemix, Anzeigen von Protokollen ferner App-Protokolle usw.), ohne dass die Editorumgebung verlassen werden muss.
{:shortdesc}

![Screenshot der Download-Anzeige der IBM Developer Tools-Erweiterung.](ibm-dev-tools-for-vscode.png "Download-Anzeige der Erweiterung in Visual Studio Code")

## Abhängigkeiten
{: #dependencies}

Um die IBM Developer Tools-Erweiterung für Visual Studio Code nutzen zu können, muss das Plug-in für die [Bluemix-Befehlszeilenschnittstelle](https://plugins.ng.bluemix.net/ui/home.html) und die [IBM Developer-Befehlszeilenschnittstelle](/docs/cloudnative/dev_cli.html) auf Ihrem System installiert sein.

## Installation
{: #installation}

Das einfachste Verfahren zur Installation von IBM Developer Tools ist die Verwendung des Visual Studio Code-Befehls 'quick open':

1. Öffnen Sie die 'quick open'-Befehlspalette im Editor mit den folgenden Tastenkombinationen:

  * **Mac:** `cmd + p`
  * **Windows/Linux:** `ctrl + p`

2. Geben Sie den Befehl `ext install ibm-developer` ein und drücken Sie die Eingabetaste, um die IBM Developer Tools-Erweiterung im Visual Studio Code-Editor zu installieren.

Alternativ können Sie die IBM Developer Tools-Erweiterung über die Verwaltungsanzeige "Extensions" installieren:

1. Öffnen Sie die Seitenleiste **Extensions** im Visual Studio Code-Editor und suchen Sie anschließend nach der Zeichenfolge `publisher:IBM Developer`.  Die IBM Developer Tools-Erweiterung wird in den Suchergebnissen angezeigt.  
2. Klicken Sie auf die Schaltfläche **Install**, um mit der Installation zu beginnen.

Sie können auf die [IBM Developer Tools-Erweiterung auch direkt in Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer) zugreifen.


## Verwendung
{: #usage}

Sie können die Befehle der Erweiterung über die Befehlspalette von Visual Studio Code aufrufen.

Öffnen Sie zunächst die Befehlspalette unter Verwendung der folgenden Tastenkombination:

* **Mac:** `cmd + shift + p`
* **Windows/Linux:** `ctrl + shift + p`

Geben Sie als Nächstes den aufzurufenden Befehl ein oder wählen Sie ihn aus. Sie können ‘bx’ in der Befehlspalette eingeben, um die Liste aller verfügbaren Befehle anzuzeigen. 

### Mithilfe der IBM Developer Extension for Docker-Workflows (Docker-Container)
{: #usage-docker}

Sie können die Arbeit mit 'bx dev'-Workflows in wenigen Schritten beginnen:
* Erstellen Sie ein Projekt unter Verwendung einer der beiden folgenden Methoden:
  * Verwenden Sie die [Bluemix-Webkonsole](https://console.ng.bluemix.net/developer/getting-started/) und laden Sie den generierten Code herunter.
  * Verwenden Sie die [Bluemix Developer-Befehlszeilenschnittstelle](/docs/cloudnative/dev_cli.html) und generieren Sie ein Projekt mit dem Befehl `bx dev create`.
* Öffnen Sie den Ordner des Projekts lokal im Visual Studio-Code-Editor.
* Verwenden Sie den Befehl `bx dev build`, um die App in ein Docker-Image umzuwandeln.
* Verwenden Sie den Befehl `bx dev debug`, um die App in der lokalen Docker-Umgebung für die Entwicklung auszuführen.
> Hinweis: Um eine Node.js-Anwendung zu debuggen, die im lokalen Docker-Container ausgeführt wird, müssen Sie [eine Debugkonfiguration für den lokalen Container hinzufügen](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container).
* Verwenden Sie den Befehl `bx dev run`, um die App in der lokalen Docker-Umgebung im Freigabemodus ausführen.
* Verwenden Sie den Befehl `bx dev deploy`, um die Anwendung für eine Cloud Foundry-Laufzeitumgebung unter Bluemix bereitzustellen*(IBM Container Support in Kürze verfügbar).*

### Mithilfe der IBM Developer Extension for Cloud Foundry-Workflows
{: #usage-cloud-foundry}

Für Benutzer, die zurzeit Apps für Cloud Foundry-Laufzeitumgebungen unter IBM Bluemix bereitstellen, ist auch Unterstützung für `cf`-Operationen verfügbar.

Sie können die Arbeit mit Cloud Foundry-Workflows nach wenigen Schritten beginnen:
* Erstellen Sie eine neue Cloud Foundry-Anwendung.
  * Verwenden Sie die [Webkonsole](https://console.ng.bluemix.net/dashboard/cf-apps) und laden Sie den Starter-Code herunter.
  * Erstellen Sie manuell eine neue Cloud Foundry-Anwendung.
* Öffnen Sie den Ordner des Projekts lokal im Visual Studio Code-Editor.
* Verwenden Sie den Befehl `bx cf apps`, um alle Ihre Anwendungen aufzulisten.
* Verwenden Sie den Befehl `bx cf push`, um einen Build Ihrer Anwendung in die Cloud Foundry-Laufzeitumgebung zu übertragen.
* Verwenden Sie bx `cf <start/stop/restage/restart>`, um den Status Ihrer Anwendung zu ändern.
* Verwenden Sie den Befehl `bx cf logs`, um den Protokolldatenstrom für Ihre Anwendung live anzuzeigen.
  * Verwenden Sie den Befehl `bx cf logs`, um den Protokolldatenstrom zu stoppen.




