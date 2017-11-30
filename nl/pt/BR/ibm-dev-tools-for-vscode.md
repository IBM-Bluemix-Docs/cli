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

O IBM Developer Extension for Visual Studio Code é uma extensão do editor que fornece acesso a recursos da CLI do desenvolvedor da IBM diretamente na paleta de comandos do editor do Visual Studio Code.  Ele permite o acesso rápido a um subconjunto de comandos `bx dev` para os fluxos de trabalho Docker e CloudFoundry, incluindo implementação do app, início/parada/reinicialização de apps no Bluemix, visualização de logs de app remoto e mais – tudo sem a necessidade de sair do contexto do editor.
{:shortdesc}

![Captura de tela da tela de download da extensão IBM Developer Tools.](ibm-dev-tools-for-vscode.png "Tela de download da extensão dentro do Visual Studio Code")

## Dependências
{: #dependencies}

Para utilizar a extensão IBM Developer Tools para o Visual Studio Code, também serão necessários a [CLI do Bluemix](https://plugins.ng.bluemix.net/ui/home.html) e o plug-in [CLI do IBM Developer](/docs/cloudnative/dev_cli.html) instalados no sistema.

## Instalação
{: #installation}

A maneira mais simples de instalar a extensão IBM Developers Tools é usar o comando 'quick open' do Visual Studio Code:

1. Abra a paleta de comandos 'quick open' usando as combinações de teclas a seguir de dentro do editor:

  * **Mac:** `cmd + p`
  * **Windows/Linux:** `ctrl + p`

2. Insira o comando `ext install ibm-developer` e pressione Enter para instalar a extensão IBM Developer Tools dentro do editor do Visual Studio Code.

Como alternativa, é possível instalar a extensão IBM Developer Tools por meio do painel de gerenciamento "Extensões":

1. Abra a barra lateral **Extensões** dentro do editor do Visual Studio Code e, em seguida, procure usando a sequência `publisher:IBM Developer`.  A extensão IBM Developer Tools será exibida nos resultados da procura.  
2. Clique no botão **Instalar** para começar a instalação.

Também é possível acessar a [extensão IBM Developer Tools diretamente do Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer).


## Uso
{: #usage}

Você chama os comandos de extensão usando a paleta de comandos do Visual Studio Code.

Primeiramente, abra a paleta de comandos usando a combinação de teclas a seguir:

* **Mac:** `cmd + shift + p`
* **Windows/Linux:** `ctrl + shift + p`

Em seguida, insira ou selecione o comando que você deseja chamar. É possível digitar ‘bx’ na paleta de comandos para ver a lista de todos os comandos disponíveis. 

### Usando os fluxos de trabalho do IBM Developer Extension for Docker (contêineres do Docker)
{: #usage-docker}

É possível iniciar a utilização dos fluxos de trabalho bx dev em apenas algumas etapas:
* Crie um projeto usando um dos dois métodos abaixo:
  * Use o [Console da web do Bluemix](https://console.ng.bluemix.net/developer/getting-started/) e faça download do código gerado
  * Use a [CLI do Bluemix Developer](/docs/cloudnative/dev_cli.html) e gere um projeto usando o comando `bx dev create`
* Abra a pasta do projeto localmente no editor do Visual Studio Code
* Use o comando `bx dev build` para construir o app em uma imagem do Docker
* Use o comando `bx dev debug` para executar o app no Docker local para desenvolvimento
> Nota: para depurar um aplicativo Node.js em execução dentro do contêiner do Docker local, será necessário [incluir uma configuração de depuração para o contêiner local](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container).
* Use o comando `bx dev run` para executar o app no Docker local no modo de liberação
* Use o comando `bx dev deploy` para implementar o aplicativo em um tempo de execução do Cloud Foundry no Bluemix *(o Suporte do IBM Container virá em breve).*

### Usando os fluxos de trabalho do IBM Developer Extension for Cloud Foundry
{: #usage-cloud-foundry}

Para usuários que estão implementando atualmente apps nos tempos de execução do Cloud Foundry no IBM Bluemix, também estamos fornecendo suporte para o conjunto de operações `cf`.

É possível iniciar a utilização dos fluxos de trabalho do CloudFoundry em apenas algumas etapas:
* Crie um novo aplicativo CloudFoundry
  * Use o [console da web](https://console.ng.bluemix.net/dashboard/cf-apps) e faça download do código de início
  * Crie um novo aplicativo CloudFoundry manualmente
* Abra a pasta do projeto localmente no editor do Visual Studio Code
* Use `bx cf apps` para listar todos os seus aplicativos
* Use `bx cf push` para enviar por push uma construção de seu aplicativo para o tempo de execução do Cloud Foundry
* Use bx `cf <start/stop/restage/restart>` para mudar o status de seu aplicativo
* Use `bx cf logs` para visualizar o fluxo de logs em tempo real de seu aplicativo
  * Use `bx cf logs` para parar o fluxo de logs




