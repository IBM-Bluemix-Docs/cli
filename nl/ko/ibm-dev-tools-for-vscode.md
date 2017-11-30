---

copyright:

  years: 2017

lastupdated: "2017-06-29"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# Visual Studio Code용 IBM Developer Tools
{: #ibm-dev-tools-for-vscode}

Visual Studio Code용 IBM Developer Extension은 Visual Studio Code 편집기의 명령 팔레트 내의 IBM Developer CLI에서 직접 기능에 액세스를 제공하는 편집기용 확장입니다. 이는 편집기의 컨텍스트를 떠날 필요 없이 Docker 및 CloudFoundry 워크플로우 모두(앱 배치, Bluemix에서 앱 시작/중지/다시 시작하기, 원격 앱 로그 보기 등 포함)에 대해 `bx dev` 명령의 서브세트에 신속하게 액세스할 수 있도록 해줍니다.
{:shortdesc}

![IBM Developer Tools 확장 다운로드 화면의 화면 캡처.](ibm-dev-tools-for-vscode.png "Visual Studio Code 내의 확장 다운로드 화면")

## 종속 항목
{: #dependencies}

Visual Studio Code용 IBM Developer Tools 확장을 사용하려면 [Bluemix CLI](https://plugins.ng.bluemix.net/ui/home.html) 및 [IBM Developer CLI](/docs/cloudnative/dev_cli.html) 플러그인이 시스템에 설치되어 있어야 합니다. 

## 설치
{: #installation}

IBM Developers Tools 확장은 설치하는 가장 간단한 방법은 Visual Studio Code의 'quick open' 명령을 사용하는 것입니다. 

1. 편집기 내에서 다음과 같은 키 조합을 사용하여 'quick open' 명령 팔레트를 여십시오. 

  * **Mac:** `cmd + p`
  * **Windows / Linux:** `ctrl + p`

2. `ext install ibm-developer` 명령을 입력하고 Enter를 눌러서 Visual Studio Code 편집기 내부에서 IBM Developer Tools 확장을 설치하십시오. 

또는 "확장" 관리 패널을 통해 IBM Developer Tools 확장을 설치할 수 있습니다.

1. Visual Studio Code 편집기의 내부에서 **확장** 사이드바를 연 후에 `publisher:IBM Developer` 문자열을 사용하여 검색하십시오. IBM Developer Tools 확장이 검색 결과에 표시됩니다.  
2. **설치** 단추를 클릭하여 설치를 시작하십시오.

[IBM Developer Tools extension directly within the Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBM.ibm-developer)에 액세스할 수도 있습니다.


## 사용
{: #usage}

Visual Studio Code의 명령 팔레트를 사용하여 확장 명령을 호출합니다.

우선, 다음 키 조합을 사용하여 명령 팔레트를 여십시오.

* **Mac:** `cmd + shift + p`
* **Windows / Linux:** `ctrl + shift + p`

그 다음에는 호출하려는 명령을 입력하거나 선택하십시오. 명령 팔레트 내에서 ‘bx’를 입력하여 모든 사용 가능한 명령의 목록을 볼 수 있습니다.  

### Docker 워크플로우(Docker 컨테이너)용 IBM Developer Extension 사용
{: #usage-docker}

다음과 같은 몇 가지 단계로 bx dev 워크플로우를 시작할 수 있습니다.
* 아래 두 가지 방법 중 하나를 사용하여 프로젝트 작성: 
  * [Bluemix 웹 콘솔](https://console.ng.bluemix.net/developer/getting-started/) 사용 및 생성된 코드 다운로드
  * [Bluemix Developer CLI](/docs/cloudnative/dev_cli.html) 사용 및 `bx dev create` 명령을 사용하여 프로젝트 생성
* Visual Studio Code 편집기에서 프로젝트의 폴더를 로컬로 열기
* `bx dev build` 명령을 사용하여 앱을 Docker 이미지에 빌드
* `bx dev debug` 명령을 사용하여 개발을 위해 로컬 Docker에서 앱 실행
> 참고: 로컬 Docker 컨테이너 내부에서 실행 중인 Node.js 애플리케이션을 디버그하려면 [로컬 컨테이너에 대한 디버그 구성 추가](https://github.com/IBM-Bluemix/ibm-developer-extension-vscode#debugging-nodejs-apps-within-the-local-docker-container)를 해야 합니다.

* `bx dev run` 명령을 사용하여 릴리스 모드로 로컬 Docker에서 앱 실행
* `bx dev deploy` 명령을 사용하여 Bluemix에서 Cloud Foundry 런타임에 애플리케이션을 배치*(IBM 컨테이너 지원 예정).*

### Cloud Foundry 워크플로우용 IBM Developer Extension 사용
{: #usage-cloud-foundry}

IBM Bluemix에서 Cloud Foundry 런타임에 현재 앱을 배치하고 있는 사용자를 위해 `cf` 세트의 오퍼레이션에 대한 지원도 제공합니다.

다음과 같은 몇 가지 단계로 CloudFoundry 워크플로우를 시작할 수 있습니다.
* 새 CloudFoundry 애플리케이션 작성
  * [웹 콘솔](https://console.ng.bluemix.net/dashboard/cf-apps) 사용 및 스타터 코드 다운로드
  * 새 CloudFoundry 애플리케이션 수동으로 작성
* Visual Studio Code 편집기에서 프로젝트 폴더를 로컬로 열기
* `bx cf apps`를 사용하여 애플리케이션 모두 나열
* `bx cf push`를 사용하여 Cloud Foundry 런타임에 애플리케이션의 빌드 푸시
* `cf <start/stop/restage/restart>`를 사용하여 애플리케이션의 상태 변경
* `bx cf logs`를 사용하여 애플리케이션에 대한 라이브 로그 스트림 보기
  * `bx cf logs`를 사용하여 로그 스트림 중지




