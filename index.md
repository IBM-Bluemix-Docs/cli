---



copyright:

  years: 2015, 2017

lastupdated: "2017-06-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}

# Manual CLI installation
{: #cli}

{{site.data.keyword.Bluemix}} CLI provides a command line experience to manage your {{site.data.keyword.Bluemix_notm}} environment. It also includes a Cloud Foundry command-line interface, cf, in its installation, for managing Cloud Foundry applications and services.
{:shortdesc}

Both CLI tools use 443 port by default. If you have HTTP proxy between the CLI tools and {{site.data.keyword.Bluemix_notm}} environment, you must configure the `HTTP_PROXY` environment variable with the actual HTTP proxy URL and port if there is one. See [Using the CLI with an HTTP Proxy Server ![External link icon](../icons/launch-glyph.svg)](http://docs.cloudfoundry.org/cf-cli/http-proxy.html){: new_window} for more details.

[Download {{site.data.keyword.Bluemix_notm}} CLI ![External link icon](../icons/launch-glyph.svg)](https://github.com/IBM-Bluemix/bluemix-cli-release/releases/){: new_window}

If you're on macOS, the easiest way to get started with IBM Cloud tools is by using [IBM Cloud Application Tools 2](/docs/cli/icat.html).
{: tip}

## ![](./images/CLI_Plugin.svg) Command line interface plug-ins
{: #cliplugins notoc}

Easily extend your {{site.data.keyword.Bluemix_notm}} command line interface with more commands. To access the {{site.data.keyword.Bluemix_notm}} command line interface plug-ins, see the [CLI Plug-in Repository ![External link icon](../icons/launch-glyph.svg)](https://plugins.ng.bluemix.net/){: new_window}.

### Extend your {{site.data.keyword.Bluemix_notm}} command-line interface: bx
{: #cli_bluemix_ext notoc}


After you install the {{site.data.keyword.Bluemix_notm}} cli tool, the [CLI Plug-in Repository ![External link icon](../icons/launch-glyph.svg)](https://plugins.ng.bluemix.net/){: new_window} is pre-configured with a repository alias `Bluemix` by default. You can install available plug-ins directly.

```
bluemix plugin install plugin_name -r Bluemix
```

| *{{site.data.keyword.autoscaling}} CLI* |  *IBM Bluemix Container Service*  |
|-----|-----|
| Plug-in name: auto-scaling <br> [View Docs](/docs/cli/plugins/auto-scaling/index.html) |  Plug-in name: container-service  <br> [View Docs](/docs/containers/cs_cli_devtools.html) |
{: caption="Table 2. Plug-ins" caption-side="top"}

|  *Private network peering* | *Schematics* | *VPN*  |
|-----|-----|-----|
| Plug-in name: private-network-peering  <br> [View Docs](/docs/cli/plugins/pnp/index.html) | Plug-in name: Schematics  <br> [View Docs](/docs/services/schematics/schematics_reference.html) | Plug-in name: VPN  <br> [View Docs](/docs/cli/plugins/bx_vpn/index.html) |
{: caption="Table 3. Plug-ins" caption-side="top"}

You can also add plug-ins from other repositories that complies with the {{site.data.keyword.Bluemix_notm}} cli architecture.
1. To install {{site.data.keyword.Bluemix_notm}} CLI plug-ins from another repository, set the plug-in registry endpoint:
```
bluemix plugin repo-add bluemix-other-repo [repo_url]
```
where `repo_url` is the https url of the plugin repository.

2. Run the following command to install a plug-in:
```
bluemix plugin install plugin_name -r bluemix-other-repo
```

### Extend Cloud Foundry command-line interface: bx cf
{: #cli_cf_ext notoc}

After you install the {{site.data.keyword.Bluemix_notm}} command-line interface, a Cloud Foundry command-line interface is also installed inside the {{site.data.keyword.Bluemix_notm}} CLI directory. Run the Cloud Foundry CLI commands using `bluemix cf`.

* To install cf CLI plug-ins from the {{site.data.keyword.Bluemix_notm}} registry, set the plug-in registry endpoint:

```
bluemix cf add-plugin-repo bluemix-cf-repo https://plugins.ng.bluemix.net
```
{: codeblock}

* Then, run the following command to install a plug-in:

```
bluemix cf install-plugin plugin_name -r bluemix-cf-repo
```
{: codeblock}

| *Admin Console* | *VPN* |
|-----------------|-----------------|
|  Plug-in name: bluemix-admin <br> [View Docs](/docs/cli/plugins/bluemix_admin/index.html) | Plug-in name: VPN <br> [View Docs](/docs/cli/plugins/vpn/index.html) |
{: caption="Table 4. Plug-ins" caption-side="top"}


## ![](./images/Integrated_Dev_Tools.svg) Integrated development tools
{: #ide notoc}

Download and install plug-ins to integrate your favorite {{site.data.keyword.Bluemix_notm}} services.

| *Liberty for Java* | *MobileFirst* | *{{site.data.keyword.rules_short}}* | *API Connect* | *Eclipse Tools for Bluemix* |
|----------|----------|----------|----------|----------|
| [Liberty Eclipse Plug-in ![External link icon](../icons/launch-glyph.svg)](https://developer.ibm.com/wasdev/downloads/liberty-profile-using-eclipse/){: new_window} | [Eclipse Plug-in ![External link icon](../icons/launch-glyph.svg)](https://marketplace.eclipse.org/content/ibm-mobilefirst-platform-studio){: new_window} | [Rules Designer Eclipse Plug-in](../services/rules/index.html#rulov002) | [Developer Toolkit](/docs/services/apiconnect/creating_apis.html#install_dev_tk ) | [Bluemix Eclipse Plug-in](/docs/manageapps/eclipsetools/eclipsetools.html) |
{: caption="Table 5. Plug-ins" caption-side="top"}
