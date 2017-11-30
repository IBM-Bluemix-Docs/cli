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

The IBM Developer Extension for Visual Studio code is an extension for the editor that provides access to capabilities from the IBM developer CLI directly within the Visual Studio Code editor’s command palette.  It enables you to quickly access a subset of `bx dev` commands for both Docker and CloudFoundry workflows, including app deployment, starting/stopping/restarting apps on {{site.data.keyword.Bluemix_notm}}, viewing remote app logs, and more – all without the need to leave the editor’s context.
{:shortdesc}

![Screen capture of the IBM Developer Tools extension download screen.](ibm-dev-tools-for-vscode.png "Extension download screen within Visual Studio Code")

## Dependencies
{: #dependencies}

To utilize the IBM Developer Tools extension for Visual Studio Code, you will also need the [{{site.data.keyword.Bluemix_notm}} CLI](https://plugins.ng.bluemix.net/ui/home.html) and the [IBM Developer CLI](/docs/cloudnative/dev_cli.html) plugin installed on your system.

## Installation
{: #installation}

The simplest way to install the IBM Developers Tools extension is to use Visual Studio Code’s 'quick open' command:

1. open the 'quick open' command palette using the following key combinations from within the editor:

  * **Mac:** `cmd + p`
  * **Windows / Linux:** `ctrl + p`

2. Enter the `ext install ibm-developer` command and press enter to install the IBM Developer Tools extension inside the Visual Studio Code editor.

Alternatively, you can install the IBM Developer Tools extension through the "Extensions" management panel:

1. Open the **Extensions** sidebar inside of the Visual Studio Code editor, and then search using the string `publisher:IBM Developer`.  The IBM Developer Tools extension will be displayed in the search results.  
2. Click the **Install** button to begin the installation.

You can also access the [IBM Developer Tools extension directly within the Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer).


## Usage
{: #usage}

You invoke extension commands using Visual Studio Code’s command palette.

First, open the command palette using the following key combination:

* **Mac:** `cmd + shift + p`
* **Windows / Linux:** `ctrl + shift + p`

Next, enter or select the command you want to invoke. You can type ‘bx’ within the command palette to see the list of all available commands. 

### Using the IBM Developer Extension for Docker workflows (Docker containers)
{: #usage-docker}

You can get started with bx dev workflows in just a few steps:
* Create a project using one of the two methods below:
  * Use the [{{site.data.keyword.Bluemix_notm}} web console](https://console.ng.bluemix.net/developer/getting-started/) and download the generated code
  * Use the [{{site.data.keyword.Bluemix_notm}} Developer CLI](/docs/cloudnative/dev_cli.html) and generate a project using the `bx dev create` command
* Open the project’s folder locally in the Visual Studio Code editor
* Use the `bx dev build` command to build the app into a Docker image
* Use the `bx dev debug` command to run the app in local Docker for development
> Note: To debug a Node.js application running inside the local Docker container, you’ll need to [add a debug configuration for the local container](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container).
* Use the `bx dev run` command to run the app in local Docker in release mode
* Use the `bx dev deploy` command to deploy the application to a Cloud Foundry runtime on {{site.data.keyword.Bluemix_notm}} *(IBM Container Support coming soon).*

### Using the IBM Developer Extension for Cloud Foundry workflows
{: #usage-cloud-foundry}

For users that are currently deploying apps to Cloud Foundry runtimes on IBM {{site.data.keyword.Bluemix_notm}}, we are also providing support for the `cf` set of operations.

You can get started with CloudFoundry workflows in just a few steps:
* Create a new CloudFoundry application
  * Use the [web console](https://console.ng.bluemix.net/dashboard/cf-apps) and download the starter code
  * Create a new CloudFoundry application manually
* Open the project folder locally in the Visual Studio Code editor
* Use `bx cf apps` to list all of your applications
* Use `bx cf push` to push a build of your application to the Cloud Foundry runtime
* Use bx `cf <start/stop/restage/restart>` to change the status of your application
* Use `bx cf logs` to view the live log stream for your application
  * Use `bx cf logs` to stop the log stream




