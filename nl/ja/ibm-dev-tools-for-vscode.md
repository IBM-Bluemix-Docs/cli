---

copyright:

  years: 2017

lastupdated: "2017-06-29"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# Visual Studio Code 用 IBM Developer Tools
{: #ibm-dev-tools-for-vscode}

IBM Developer Extension for Visual Studio Code は、Visual Studio Code エディターのコマンド・パレット内から直接、IBM Developer CLI の機能へのアクセスを提供する、エディターの拡張機能です。これにより、アプリのデプロイメント、Bluemix 上でのアプリの開始/停止/再始動、リモート・アプリ・ログの表示など、Docker と CloudFoundry の両方のワークフローで、エディターのコンテキストを離れることなく、`bx dev` コマンドのサブセットに素早くアクセスすることができます。
{:shortdesc}

![IBM Developer Tools の拡張機能ダウンロード画面の画面キャプチャー。](ibm-dev-tools-for-vscode.png "Visual Studio Code 内の拡張機能ダウンロード画面")

## 従属関係
{: #dependencies}

IBM Developer Tools の Visual Studio Code 用拡張機能を使用するには、さらに [Bluemix CLI](https://plugins.ng.bluemix.net/ui/home.html) および [IBM Developer CLI](/docs/cloudnative/dev_cli.html) プラグインがシステムにインストールされている必要があります。

## インストール
{: #installation}

IBM Developers Tools のこの拡張機能をインストールするための最も簡単な方法は、以下に示すように、Visual Studio Code の「quick open」コマンドを使用することです。

1. エディター内から以下のキーの組み合わせを使用して、「quick open」コマンド・パレットを開きます。

  * **Mac:** `cmd + p`
  * **Windows / Linux:** `ctrl + p`

2. `ext install ibm-developer` コマンドを入力し、Enter キーを押してこの IBM Developer Tools 拡張機能を Visual Studio Code エディター内にインストールします。

あるいは、以下に示すように、「拡張機能」管理パネルを介してこの IBM Developer Tools 拡張機能をインストールすることもできます。

1. Visual Studio Code エディターの**「拡張機能」**サイドバーを開き、次に、ストリング `publisher:IBM Developer` を使用して検索します。IBM Developer Tools 拡張機能が検索結果に表示されます。  
2. **「インストール」**ボタンをクリックしてインストールを開始します。

また、[Visual Studio Code Marketplace 内から直接、IBM Developer Tools 拡張機能](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer)にアクセスすることもできます。


## 使用量
{: #usage}

Visual Studio Code のコマンド・パレットを使用して extension のコマンドを呼び出します。

最初に、以下のキーの組み合わせを使用してコマンド・パレットを開きます。

* **Mac:** `cmd + shift + p`
* **Windows / Linux:** `ctrl + shift + p`

次に、呼び出すコマンドを入力または選択します。コマンド・パレット内に「bx」と入力すると、すべての使用可能コマンドのリストを表示できます。 

### Docker ワークフロー (Docker コンテナー) での IBM Developer Extension の使用
{: #usage-docker}

以下に示すように、ほんの数ステップで bx dev ワークフローを開始することができます。
* 以下の 2 つの方法のいずれかを使用してプロジェクトを作成します。
  * [Bluemix Web コンソール](https://console.ng.bluemix.net/developer/getting-started/)を使用し、生成されたコードをダウンロードします
  * [Bluemix Developer CLI](/docs/cloudnative/dev_cli.html) を使用し、`bx dev create` コマンドを使用してプロジェクトを生成します
* プロジェクトのフォルダーを Visual Studio Code エディターでローカルに開きます
* `bx dev build` コマンドを使用して、アプリをビルドして Docker イメージを作成します
* `bx dev debug` コマンドを使用して、開発用のローカル Docker でアプリを実行します
> 注: ローカル Docker コンテナー内で実行されている Node.js アプリケーションをデバッグするには、[ローカル・コンテナー用のデバッグ構成を追加](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container)する必要があります。

* `bx dev run` コマンドを使用して、アプリをローカル Docker 内でリリース・モードで実行します
* `bx dev deploy` コマンドを使用して、アプリケーションを Bluemix 上の Cloud Foundry ランタイムにデプロイします *(IBM Container サポートは間もなく利用可能になります)。*

### Cloud Foundry ワークフローでの IBM Developer Extension の使用
{: #usage-cloud-foundry}

現在、IBM Bluemix 上の Cloud Foundry ランタイムにアプリをデプロイしているユーザーのために、`cf` 操作セットのサポートも提供しています。

以下のに示すように、ほんの数ステップで CloudFoundry ワークフローを開始することができます。
* 新規 CloudFoundry アプリケーションを作成します。
  * [Web コンソール](https://console.ng.bluemix.net/dashboard/cf-apps) を使用し、スターター・コードをダウンロードします
  * 新しい CloudFoundry アプリケーションを手動で作成します
* Visual Studio Code エディターでローカル環境でプロジェクト・フォルダーを開きます
* `bx cf apps` を使用して、すべてのアプリケーションをリストします
* `bx cf push` を使用して、アプリケーションのビルドを Cloud Foundry ランタイムにプッシュします
* `bx cf <start/stop/restage/restart>` を使用して、アプリケーションの状況を変更します
* `bx cf logs` を使用して、アプリケーションの稼働中のログ・ストリームを表示します
  * `bx cf logs` を使用してログ・ストリームを停止します




