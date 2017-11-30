---



copyright:

  years: 2015, 2017
lastupdated: "2017-010-13"

---

{:codeblock: .codeblock} 
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Download and install {{site.data.keyword.Bluemix_notm}} CLI
{: #download_install}

You can use an [installer](#installers) or [install from the shell](#shell_install) to install {{site.data.keyword.Bluemix_notm}} CLI.

## Download installers
{: #installers}

See the [{{site.data.keyword.Bluemix_notm}} CLI Installer (all versions)](all_versions.html){: new_window} page to download the latest installer of your OS.

For macOS and Windows, simply run the installer. 

For Linux, after downloading the installer package, extract it and run the installation script with root permission.

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
  
## Install from shell
{: #shell_install}


### macOS

Copy and paste the following command to a terminal of your mac OS and execute it:

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```
{: codeblock}

### Linux

Copy and paste the following command to a terminal of your Linux OS and execute it:

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```
{: codeblock}

### Windows PowerShell

Copy and paste the following command into a [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} terminal console and execute it:

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```
{: codeblock}
