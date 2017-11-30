---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 플러그인으로 {{site.data.keyword.Bluemix_notm}} CLI 확장
{: #plug-ins}

{{site.data.keyword.Bluemix_notm}} CLI는 해당 기능을 확장하도록 플러그인 프레임워크를 지원합니다. 저장소 또는 웹 URL에서 플러그인을 설치하거나 플러그인 2진을 로컬로 설치할 수 있습니다. 

[{{site.data.keyword.Bluemix_notm}} CLI 플러그인 저장소](http://clis.ng.bluemix.net/ui/repository.html#bluemix-plugins){: new_window}(![외부 링크 아이콘](../../../icons/launch-glyph.svg))는 플러그인을 호스팅하는 공식 저장소입니다.

## 저장소에서 플러그인 설치

* 플러그인 찾기

  'bluemix plugin repo-plugins -r REPO_NAME' 명령을 사용하여 저장소에서 플러그인을 찾으십시오.
  
  {{site.data.keyword.Bluemix_notm}} CLI에는 기본적으로 이름이 `Bluemix`인 공식 저장소가 구성되어 있습니다. 공식 `Bluemix` 저장소에서 다음과 같이 플러그인을 나열할 수 있습니다.

  ```
  $ bluemix plugin repo-plugins -r Bluemix
  Getting plug-ins from repository 'Bluemix'...

  Repository: Bluemix
  Name           Description                                    Versions
  auto-scaling   Bluemix CLI plugin for Auto-Scaling service    0.2.1, 0.2.2
  nsg            Bluemix Network Security Group plugin          0.1.1

  ```

* 플러그인 설치

  'bx plugin install PLUGIN_NAME -r REPO_NAME'을 사용하여 플러그인을 설치하십시오. 예를 들어, 다음과 같습니다.

  ```
  $ bluemix plugin install auto-scaling -r Bluemix
  Looking up 'auto-scaling' from repository 'Bluemix'...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload062468676/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ```

## 로컬로 플러그인 설치

  `bluemix plugin install LOCAL_FILE_NAME` 명령을 사용하여 로컬 머신에 플러그인 2진을 설치하십시오. 예를 들어, 다음과 같습니다.

  ```
  $ bluemix plugin install ./auto-scaling-darwin-amd64-0.2.2
  Installing pluign './auto-scaling-darwin-amd64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  $
  ```

## 웹 URL에서 설치

  `bluemix plugin install URL` 명령을 사용하여 웹 URL에서 직접 플러그인을 설치하십시오. 예를 들어, 다음과 같습니다.

  ```
  ~$ bluemix plugin install https://plugins.ng.bluemix.net/downloads/bluemix-plugins/auto-scaling/auto-scaling-darwin-amd64-0.2.2
  Attempting to download the binary file...
  9857792 bytes downloaded
  Installing plugin '/var/folder/v7/l3hnkz0x0b9b5mf1fyxh7yw00000gn/T/BluemixFileDownload274645142/auto-scaling-darwin-adm64-0.2.2'...
  OK
  Plugin 'auto-scaling 0.2.2' was successfully installed.
  ~$
  ```


플러그인 관리에 대한 자세한 명령을 보려면 `bluemix plugin`을 실행하여 도움말 메시지를 확인하십시오.
