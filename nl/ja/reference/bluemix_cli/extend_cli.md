---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# プラグインを使用した {{site.data.keyword.Bluemix_notm}} CLI の拡張
{: #plug-ins}

{{site.data.keyword.Bluemix_notm}} CLI は、機能を拡張するためにプラグイン・フレームワークをサポートしています。リポジトリーまたは Web URL からプラグインをインストールしたり、ローカルにプラグイン・バイナリーをインストールしたりすることができます。 

[{{site.data.keyword.Bluemix_notm}} CLI プラグイン・リポジトリー](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window} ![外部リンク・アイコン](../../../icons/launch-glyph.svg) は、プラグインをホストする公式リポジトリーです。

## リポジトリーからのプラグインのインストール

* プラグインを検索します。

  リポジトリー内のプラグインを検索するには、「bluemix plugin repo-plugins -r REPO_NAME」コマンドを使用します。
  
  {{site.data.keyword.Bluemix_notm}} CLI には、`Bluemix` という名前の公式リポジトリーがデフォルトで構成されています。以下のように、公式の `Bluemix` リポジトリー内のプラグインをリストすることができます。

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* プラグインのインストール

  プラグインをインストールするには、「bx plugin install PLUGIN_NAME -r REPO_NAME」を使用します。例えば、以下のようになります。

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## ローカルでのプラグインのインストール

  ローカル・マシンにプラグイン・バイナリーをインストールするには、コマンド `bluemix plugin install LOCAL_FILE_NAME` を使用します。例えば、以下のようになります。

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## Web URL からのインストール

  Web URL から直接プラグインをインストールするには、コマンド `bluemix plugin install URL` を使用します。例えば、以下のようになります。

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


プラグインを管理するためのその他のコマンドについては、`bluemix plugin` を実行してヘルプ・メッセージを表示してください。
