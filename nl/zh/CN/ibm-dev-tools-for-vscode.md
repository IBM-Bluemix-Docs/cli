---

copyright:

  years: 2017

lastupdated: "2017-06-29"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# IBM Developer Tools for Visual Studio Code
{: #ibm-dev-tools-for-vscode}

IBM Developer Extension for Visual Studio Code 是一个编辑器扩展，可用于直接在 Visual Studio Code 编辑器的命令选用板内访问 IBM 开发者 CLI 中的功能。它支持快速访问适用于 Docker 和 CloudFoundry 工作流的 `bx dev` 命令子集，包括应用程序部署、在 Bluemix 上启动/停止/重新启动应用程序、查看远程应用程序日志等等，这一切操作都无需退出编辑器的上下文。
{:shortdesc}

![IBM Developer Tools 扩展下载屏幕的截屏。](ibm-dev-tools-for-vscode.png "Visual Studio Code 中的扩展下载屏幕")

## 依赖项
{: #dependencies}

要利用 IBM Developer Tools 用于 Visual Studio Code 的扩展，您还需要在系统上安装 [Bluemix CLI](https://plugins.ng.bluemix.net/ui/home.html) 和 [IBM Developer CLI](/docs/cloudnative/dev_cli.html) 插件。

## 安装
{: #installation}

最简单的 IBM Developers Tools 扩展安装方法是使用 Visual Studio Code 的“快速打开”命令：

1. 在编辑器中使用以下组合键打开“快速打开”命令选用板：

  * **Mac：**`cmd + p`
  * **Windows / Linux：**`ctrl + p`

2. 输入 `ext install ibm-developer` 命令，然后按 Enter 键以在 Visual Studio Code 编辑器中安装 IBM Developer Tools 扩展。

或者，可以通过“扩展”管理面板来安装 IBM Developer Tools 扩展：

1. 打开 Visual Studio Code 编辑器内部的**扩展**侧边栏，然后使用字符串 `publisher:IBM Developer` 进行搜索。IBM Developer Tools 扩展将显示在搜索结果中。  
2. 单击**安装**按钮以开始安装。

您还可以[直接在 Visual Studio Code 的 Marketplace 中访问 IBM Developer Tools 扩展](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer)。


## 用法
{: #usage}

可以使用 Visual Studio Code 的命令选用板来调用扩展命令。

首先，使用以下组合键打开命令选用板：

* **Mac：**`cmd + shift + p`
* **Windows / Linux：**`ctrl + shift + p`

接下来，输入或选择要调用的命令。可以在命令选用板中输入“bx”来查看所有可用命令的列表。 

### 使用 IBM Developer Extension for Docker 工作流（Docker 容器）
{: #usage-docker}

只需几个步骤即可开始使用 bx dev 工作流：
* 使用以下两种方法中的一种来创建项目：
  * 使用 [Bluemix Web 控制台](https://console.ng.bluemix.net/developer/getting-started/)并下载生成的代码
  * 使用 [Bluemix Developer CLI](/docs/cloudnative/dev_cli.html) 并使用 `bx dev create` 命令生成项目
* 在 Visual Studio Code 编辑器本地打开项目的文件夹
* 使用 `bx dev build` 命令将应用程序构建到 Docker 映像中
* 使用 `bx dev debug` 命令在本地 Docker 中运行应用程序以进行开发
> 注：要调试在本地 Docker 容器内运行的 Node.js 应用程序，需要[为本地容器添加调试配置](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container)。

* 使用 `bx dev run` 命令在本地 Docker 中以发布方式运行应用程序
* 使用 `bx dev deploy` 命令将应用程序部署到 Bluemix 上的 Cloud Foundry 运行时*（IBM Container 支持即将推出）*。

### 使用 IBM Developer Extension for Cloud Foundry 工作流
{: #usage-cloud-foundry}

对于当前正在将应用程序部署到 IBM Bluemix 上的 Cloud Foundry 运行时的用户，我们还提供了对 `cf` 操作集的支持。

只需几个步骤即可开始使用 CloudFoundry 工作流：
* 创建新的 CloudFoundry 应用程序
  * 使用 [Web 控制台](https://console.ng.bluemix.net/dashboard/cf-apps)并下载入门模板代码
  * 手动创建新的 CloudFoundry 应用程序
* 在 Visual Studio Code 编辑器本地打开项目文件夹
* 使用 `bx cf apps` 列出所有应用程序
* 使用 `bx cf push` 将应用程序的构建推送到 Cloud Foundry 运行时
* 使用 `bx cf<start/stop/restage/restart>` 更改应用程序的状态
* 使用 `bx cf logs` 查看应用程序的实时日志流
  * 使用 `bx cf logs` 停止日志流




