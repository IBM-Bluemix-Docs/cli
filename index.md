---

copyright:

  years: 2015, 2018

lastupdated: "2018-010-03"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}

# Getting started with the {{site.data.keyword.Bluemix_notm}} CLI
{: #overview}

In this tutorial, you install a set of {{site.data.keyword.Bluemix}} developer tools, verify the installation, and configure your environment. {{site.data.keyword.Bluemix}} developer tools offer a command-line approach to creating, developing, and deploying end-to-end web, mobile, and microservice applications.
{:shortdesc}

With this installation, you get the stand-alone {{site.data.keyword.Bluemix_notm}} CLI, plus the following tools:

* `Homebrew` (Mac only)
* `Git`
* `Docker`
* `Helm`
* `kubectl`
* `curl`
* {{site.data.keyword.dev_cli_notm}} plug-in
* {{site.data.keyword.IBM_notm}} {{site.data.keyword.openwhisk_short}} plug-in
* {{site.data.keyword.registrylong_notm}} plug-in
* {{site.data.keyword.containerlong_notm}} plug-in
* `sdk-gen` plug-in

## Before you begin
{: #prereq}

You need an [{{site.data.keyword.Bluemix_notm}} account](https://console.bluemix.net/){: new_window} ![External link icon](../icons/launch-glyph.svg "External link icon") and the following system requirements:

* If you are running Windows, some functionality may not be supported if you are not running Windows 10 Pro.
* You must use the stable channel for Docker with a minimum version of 1.13.1.

## Step 1. Run the install command
{: #step1}

* For Mac and Ubuntu, run the following command:

  ```
  curl -sL https://ibm.biz/idt-installer | bash
  ```
  {: codeblock}

* For Windows 10 Pro, run the following command as an administrator:

  ```
  Set-ExecutionPolicy Unrestricted; iex(New-Object Net.WebClient).DownloadString('http://ibm.biz/idt-win-installer')
  ```
  {: codeblock}

  Right-click the Windows PowerShell icon, and select **Run as administrator**.
  {: tip}

  You may also download the installer script from our [GitHub repo](https://github.com/IBM-Cloud/ibm-cloud-developer-tools).

  For the steps to install these tools manually, see [Reinstalling tools](/docs/cli/ts_createapps.html#appendix).

## Step 2. Verify the installation
{: #step2}

To verify that the CLI and developer tools were installed successfully, run the `help` command:

```
ibmcloud dev help
```
{: codeblock}
<br>
The output lists the usage instructions, the current version, and the supported commands.

## Step 3. Configure your environment
{: #step3}

1. Connect to an API endpoint in your {{site.data.keyword.Bluemix_notm}} region. For example, enter the following command to connect to the {{site.data.keyword.Bluemix_notm}} US South region:

	```
	ibmcloud api https://api.ng.bluemix.net
	```
	{: codeblock}

2. Log in to {{site.data.keyword.Bluemix_notm}} with your IBMid.

	```
	ibmcloud login
	```
	{: codeblock}
    <br>

	If your credentials are rejected, you might be using a federated ID. See [Logging in with a federated ID](/docs/iam/login_fedid.html#federated_id) for more details.
	{: tip}

3. Set your org and space.

	```
	ibmcloud target --cf
	```
	{: codeblock}

	Optionally, you can use the output from the command above to manually set your org and space with the following command:

	```
	ibmcloud target -o <value> -s <value>
	```
	{: codeblock}

## Next steps
{: #next-steps}

You're now ready to develop and deploy your first application. See [Creating and deploying apps by using the CLI](/docs/apps/create-deploy-cli.html) for more information.
