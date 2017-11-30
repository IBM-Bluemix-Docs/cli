---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 使用外掛程式延伸 {{site.data.keyword.Bluemix_notm}} CLI
{: #plug-ins}

{{site.data.keyword.Bluemix_notm}} CLI 支援可延伸其功能的外掛程式架構。您可以從儲存庫或 Web URL 安裝外掛程式，或者在本端安裝外掛程式二進位檔。 

[{{site.data.keyword.Bluemix_notm}} CLI 外掛程式儲存庫](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![外部鏈結圖示](../../../icons/launch-glyph.svg) 是管理外掛程式的正式儲存庫。

## 從儲存庫安裝外掛程式

* 尋找外掛程式

  使用指令 'bluemix plugin repo-plugins -r REPO_NAME'，以尋找儲存庫中的外掛程式。
  
  依預設，{{site.data.keyword.Bluemix_notm}} CLI 會配置名稱為 `Bluemix` 的正式儲存庫。您可以列出正式 `Bluemix` 儲存庫中的外掛程式，如下所示。

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* 安裝外掛程式

  使用 'bx plugin install PLUGIN_NAME -r REPO_NAME' 來安裝外掛程式，例如：

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## 在本端安裝外掛程式

  使用指令 `bluemix plugin install LOCAL_FILE_NAME`，將外掛程式二進位檔安裝到本端機器，例如：

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## 從 Web URL 安裝

  使用指令 `bluemix plugin install URL`，直接從 Web URL 安裝外掛程式，例如：

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


如需其他可管理外掛程式的指令，請執行 `bluemix plugin` 以查看說明訊息。
