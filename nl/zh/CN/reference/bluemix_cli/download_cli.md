---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# 下载并安装 {{site.data.keyword.Bluemix_notm}} CLI
{: #download_install}

您可以使用 [installer](#installers) 或 [shell](#shell_install) 来安装 {{site.data.keyword.Bluemix_notm}} CLI。

## 下载安装程序
{: #installers}

转至[所有版本](all_versions.html){: new_window}页面以下载适合您操作系统的最新安装程序。

对于 macOS 和 Windows，只需运行安装程序即可。对于 Linux，下载安装程序包后，将其解压缩并以 root 用户许可权运行安装脚本。

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## 从 shell 安装
{: #shell_install}


### macOS

将以下命令复制并粘贴到 mac OS 终端，然后执行该命令。

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

将以下命令复制并粘贴到 Linux 操作系统终端，然后执行该命令。

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

将以下命令复制并粘贴到 [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} 终端控制台，然后执行该命令。

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

