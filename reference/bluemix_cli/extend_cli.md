---

copyright:

  years: 2015, 2017
lastupdated: "2017-10-20"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# Extending {{site.data.keyword.Bluemix_notm}} CLI with plug-ins
{: #plug-ins}

{{site.data.keyword.Bluemix_notm}} CLI supports a plug-in framework to extend its capability. You can install a plug-in from a repository, a web URL, or install a plug-in binary locally. 

[{{site.data.keyword.Bluemix_notm}} CLI plug-ins repository](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![External link icon](../../../icons/launch-glyph.svg) is the official repository where plug-ins are hosted.

For more commands to manage plug-ins, run `bluemix plugin` to see the help messages.
{: tip}

## Install a plug-in from the {site.data.keyword.Bluemix_notm}} CLI repository

### Step 1: Search for the plug-in

1. Use the command `bluemix plugin repo-plugins -r REPO_NAME` to look for a plugin in the repository.
2. The {{site.data.keyword.Bluemix_notm}} CLI uses the name `Bluemix` by default. You can list the plug-ins in the official `Bluemix` repository. For example:
  
  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   IBM Cloud CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            IBM Cloud Network Security Group plugin          0.1.1

  ```

### Step 2: Install the plug-in

Use the `bx plugin install PLUGIN_NAME -r REPO_NAME` command to install the plugin. For example:

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## Install a plug-in locally

Use the `bluemix plugin install LOCAL_FILE_NAME` command to install a plugin-in binary on your local machine. For example:

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## Install a plug-in from a web URL

Use the `bluemix plugin install URL` command to install a plugin directly from a web URL. For example

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```
