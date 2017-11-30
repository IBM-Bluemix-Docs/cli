---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# 下載並安裝 {{site.data.keyword.Bluemix_notm}} CLI
{: #download_install}

您可以使用[安裝程式](#installers)或 [Shell](#shell_install) 來安裝 {{site.data.keyword.Bluemix_notm}} CLI。

## 下載安裝程式
{: #installers}

移至[所有版本](all_versions.html){: new_window}頁面，以下載您 OS 的最新安裝程式。

若為 macOS 及 Windows，僅執行安裝程式。
若為 Linux，在下載安裝程式套件之後，解壓縮該套件，並使用 root 許可權來執行安裝 Script。

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## 從 Shell 安裝
{: #shell_install}


### macOS  

複製下列指令，並將其貼入 mac OS 的終端機，然後予以執行。

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

複製下列指令，並將其貼入 Linux OS 的終端機，然後予以執行。

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

複製下列指令，並將其貼入 [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} 終端機主控台，然後執行它。

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

