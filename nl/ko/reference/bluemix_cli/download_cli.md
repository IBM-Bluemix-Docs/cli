---



copyright:

  years: 2015, 2017
lastupdated: "2017-08-20"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# {{site.data.keyword.Bluemix_notm}} CLI 다운로드 및 설치
{: #download_install}

[설치 프로그램](#installers) 또는 [쉘](#shell_install)을 사용하여 {{site.data.keyword.Bluemix_notm}} CLI를 설치할 수 있습니다.

## 설치 프로그램 다운로드
{: #installers}

[모든 버전](all_versions.html){: new_window} 페이지로 이동하여 OS의 최신 설치 프로그램을 다운로드하십시오.

macOS 및 Windows의 경우 설치 프로그램을 실행하십시오.
Linux의 경우 설치 프로그램 패키지를 다운로드한 후 압축을 풀고 루트 권한을 사용하여 설치 스크립트를 실행하십시오.

  ```
  $ tar -xvf Bluemix_CLI.tar.gz
  $ cd Bluemix_CLI
  $ sudo ./install_bluemix_cli

  ```
## 쉘에서 설치
{: #shell_install}


### macOS  

다음 명령을 복사하여 mac OS의 터미널에 붙여넣고 실행하십시오.

```
curl -fsSL https://clis.ng.bluemix.net/install/osx | sh
```

### Linux

다음 명령을 복사하여 Linux OS의 터미널에 붙여넣고 실행하십시오.

```
curl -fsSL https://clis.ng.bluemix.net/install/linux | sh
```

### Windows PowerShell

다음 명령을 [Windows PowerShell](https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell){: new_window} 터미널 콘솔에 복사해서 붙여넣고 실행하십시오.

```
iex(New-Object Net.WebClient).DownloadString('https://clis.ng.bluemix.net/install/powershell')
```

