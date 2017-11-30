---



copyright:

  years: 2015，2017

lastupdated: "2017-07-12"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}

# 연합 ID로 로그인
{: #federated_id}

일회성 패스코드 또는 API 키를 사용하여 연합 사용자로 명령행 인터페이스(CLI)에서 {{site.data.keyword.Bluemix}}에 로그인할 수 있습니다.
{: shortdesc}

## 일회성 패스코드 사용
{:onetime_passcode}

연합 ID로 로그인하기 위해 일회성 패스코드 옵션을 사용할 때는 싱글 사인온(SSO) 매개변수를 지정하여 일회성 패스코드를 가져와서 로그인 시에 입력합니다.  

일회성 패스코드는 {{site.data.keyword.Bluemix_notm}} 콘솔에서 코드를 검색하기 때문에 자동화 스크립트에서 연합 ID의 사용에 실패하는 원인이 됩니다. 자동화된 스크립트로 API 키 옵션을 사용하여 문제를 피하십시오.
{: tip}

### {{site.data.keyword.Bluemix_notm}} CLI에서
1. `--sso` 옵션을 `bluemix login` 명령과 함께 지정하십시오.
2. 일회성 패스코드를 확보하려면 프롬프트에서 URL을 따르십시오 
3. CLI에서 패스코드 값을 입력으로 복사해서 붙여넣으십시오.
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### Cloud Foundry CLI에서
1. `--sso` 옵션을 `cf login` 명령과 함께 지정하십시오. 
2. 일회성 패스코드를 확보하려면 프롬프트에서 URL을 따르십시오  
3. CLI에서 패스코드 값을 입력으로 복사해서 붙여넣으십시오. 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## API 키 사용
{:api_key}

필요한 API 키는 Softlayer API 키 또는 {{site.data.keyword.Bluemix_notm}} 서비스 API 키가 아니라 {{site.data.keyword.Bluemix_notm}} 플랫폼으로 인증하는 데 사용된 {{site.data.keyword.Bluemix_notm}} API 키입니다. 

1. [`bluemix iam api-key-create` 명령](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create)으로 API 키를 작성하십시오. `-f` 옵션을 사용하여 명령 창에서 키를 표시하는 대신에 API 키 파일을 생성하십시오.

   ```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

2. API 키로 로그인하십시오. 

  다음과 같은 방법으로 {{site.data.keyword.Bluemix_notm}} CLI와 함께 API 키를 사용할 수 있습니다. 
    
    * API 키를 직접 호출합니다.
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * 키 파일과 함께 API 키를 호출합니다. 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * 환경 변수를 설정합니다. 사용자가 시스템에서 환경 변수를 설정할 수도 있습니다. 예를 들어, BLUEMIX_API_KEY=api_key_string에서 `api_key_string`은 API 키의 사용자 정의 값입니다. 환경 변수가 설정된 후에 CLI에서 간단하게 `bluemix login`을 지정할 수 있습니다. 
  
  Cloud Foundry CLI를 사용하여 로그인하려면 `apikey`를 사용자 이름으로, API 키 문자열을 비밀번호로 지정하십시오. 

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
    Authenticating...
    OK
  
    ```

