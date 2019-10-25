---

copyright:
  years: 2015, 2019
lastupdated: "2019-09-30"

keywords: command line interface, cli, getting started, getting started with IBM Cloud CLI, getting started with IBM Cloud CLI and developer tools tutorial, IBM Cloud Developer Tools CLI, ibmcloud cli, download cli, ibmcloud dev, cloud cli, dev plugin, dev plug-in, cloud command line, developer tools, dev tools, install cloud cli, getting started cli

subcollection: cloud-cli

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:external: target="_blank" .external}
{:new_window: target="_blank"}
{:note: .note}

# Getting started with the {{site.data.keyword.cloud_notm}} CLI and {{site.data.keyword.dev_cli_short}}
{: #getting-started}

In this tutorial, you install a set of {{site.data.keyword.cloud}} developer tools that include the latest {{site.data.keyword.cloud_notm}} CLI, verify the installation, and configure the environment. The {{site.data.keyword.dev_cli_notm}} offer a command line interface (CLI) approach to creating, developing, and deploying cloud applications.
{: shortdesc}

The installation command in this tutorial installs the latest stand-alone {{site.data.keyword.cloud_notm}} CLI version available, plus the following tools:

* `Homebrew` (Mac only)
* `Git`
* `Docker`
* `Helm`
* `kubectl`
* `curl` (Linux&trade; only)
* {{site.data.keyword.dev_cli_notm}} plug-in
* {{site.data.keyword.IBM_notm}} {{site.data.keyword.openwhisk_short}} plug-in
* {{site.data.keyword.cos_full_notm}} plug-in
* {{site.data.keyword.registrylong_notm}} plug-in
* {{site.data.keyword.containerlong_notm}} plug-in

## Before you begin
{: #idt-prereq}

You need an [{{site.data.keyword.cloud_notm}} account](https://cloud.ibm.com/){: external} and the following system requirements:

* You must use the stable channel for Docker with a minimum version of 1.13.1.
* For Linux&trade;, install the [curl](https://curl.haxx.se/download.html){: external} command for downloading packages through the command line. If `curl` is already installed, the installer updates it to the latest version.
* For Windows&trade;, some functions are not supported unless you are running Windows&trade; 10 Pro.

## Step 1. Run the installation command
{: #step1-install-idt}

The latest version of the {{site.data.keyword.cloud_notm}} CLI is installed when you run the command.

* For Mac and Linux&trade;, run the following command:
  ```
  curl -sL https://ibm.biz/idt-installer | bash
  ```
  {: codeblock}

* For Windows&trade; 10 Pro, run the following command as an administrator:
  ```
  [Net.ServicePointManager]::SecurityProtocol = "Tls12"; iex(New-Object Net.WebClient).DownloadString('https://ibm.biz/idt-win-installer')
  ```
  {: codeblock}

  Right-click the Windows&trade; PowerShell icon, and select **Run as administrator**.
  {: tip}

* For automating DevOps installations, you can also access the installer script directly from this [GitHub repo](https://github.com/IBM-Cloud/ibm-cloud-developer-tools){: external}.

If you need to use a 32-bit version of the CLI, or a previous version other than the latest for {{site.data.keyword.cloud_notm}} Dedicated environments, see [{{site.data.keyword.cloud_notm}} CLI releases](https://github.com/IBM-Cloud/ibm-cloud-cli-release/releases/){: external}.
{: note}

## Step 2. Verify the installation
{: #step2-verify-idt}

To verify that the CLI and Developer tools were installed successfully, run the `help` command:
```
ibmcloud dev help
```
{: codeblock}

The output lists the usage instructions, the current version, and the supported commands.
If the output is `'dev' is not a registered command`, then install the `dev` plugin:
```
ibmcloud plugin install dev -r bluemix
```

## Step 3. Configure your environment
{: #step3-configure-idt-env}

1. Log in to {{site.data.keyword.cloud_notm}} with your IBMid. If you have multiple accounts, you are prompted to select which account to use. If you do not specify a region with the `-r` flag, you must also select a region.
  ```
  ibmcloud login
  ```
  {: codeblock}
  
  If your credentials are rejected, you might be using a federated ID. To log in with a federated ID, use the `--sso` flag. See [Logging in with a federated ID](/docs/iam/federated_id?topic=iam-federated_id#federated_id) for more details.
  {: tip}

2. To access Cloud Foundry services, you must specify a Cloud Foundry org and space. You can run the following command to interactively identify the org and space:
  ```
  ibmcloud target --cf
  ```
  {: codeblock}

  Or, if you know which org and space that the service belongs to, you can use the following command:
  ```
  ibmcloud target -o <value> -s <value>
  ```
  {: codeblock}

## Next steps
{: #next-steps}

* You're now ready to develop and deploy your first app. For more information, see [Creating and deploying apps by using the CLI](/docs/apps?topic=creating-apps-create-deploy-app-cli#create-deploy-app-cli).

* You can receive notifications about new {{site.data.keyword.cloud_notm}} CLI releases. Subscribe to the [{{site.data.keyword.cloud_notm}} CLI releases repository](https://github.com/IBM-Cloud/ibm-cloud-cli-release/releases/){: external}.
