---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 使用插件扩展 {{site.data.keyword.Bluemix_notm}} CLI
{: #plug-ins}

{{site.data.keyword.Bluemix_notm}} CLI 支持通过插件框架来扩展其功能。您可以从存储库或 Web URL 安装插件，也可以本地安装插件二进制文件。 

[{{site.data.keyword.Bluemix_notm}} CLI 插件存储库](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![外部链接图标](../../../icons/launch-glyph.svg) 是用于托管插件的官方存储库。

## 从存储库安装插件

* 查找插件

  使用“bluemix plugin repo-plugins -r REPO_NAME”命令在存储库中查找插件。
  
  缺省情况下，{{site.data.keyword.Bluemix_notm}} CLI 具有名为 `Bluemix` 的官方存储库。可以列出官方 `Bluemix` 存储库中的插件，如下所示。

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* 安装插件

  使用“bx plugin install PLUGIN_NAME -r REPO_NAME”安装插件，例如：

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## 本地安装插件

  使用 `bluemix plugin install LOCAL_FILE_NAME` 命令在本地计算机上安装插件二进制文件，例如：

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## 从 Web URL 安装

  使用 `bluemix plugin install URL` 命令直接从 Web URL 安装插件，例如：

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


有关管理插件的更多命令，请运行 `bluemix plugin` 以查看帮助消息。
