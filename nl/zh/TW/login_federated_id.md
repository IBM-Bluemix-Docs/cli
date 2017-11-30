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

# 使用聯合 ID 登入
{: #federated_id}

身為聯合使用者，您可以使用一次性密碼或 API 金鑰從指令行介面 (CLI) 登入 {{site.data.keyword.Bluemix}}。
{: shortdesc}

## 使用一次性密碼
{:onetime_passcode}

當您使用一次性密碼選項以利用聯合 ID 登入時，會指定單一登入 (SSO) 參數來取得一次性密碼，您之後在登入時需要輸入它。 

因為一次性密碼會從 {{site.data.keyword.Bluemix_notm}} 主控台擷取密碼，所以在自動化 Script 中使用聯合 ID 會失敗。搭配使用 API 金鑰選項與自動化 Script，即可避免麻煩。
{: tip}

### 從 {{site.data.keyword.Bluemix_notm}} CLI
1. 指定 `bluemix login` 指令並使用 `--sso` 選項。
2. 遵循提示中的 URL，以取得一次性密碼。
3. 複製並貼上 CLI 中的密碼值作為您的輸入。
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### 從 Cloud Foundry CLI
1. 使用 `cf login` 指令指定 `--sso` 選項。 
2. 遵循提示中的 URL，以取得一次性密碼。 
3. 複製並貼上 CLI 中的密碼值作為您的輸入。 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## 使用 API 金鑰
{:api_key}

必要 API 金鑰是用來向 {{site.data.keyword.Bluemix_notm}} 平台進行鑑別的 {{site.data.keyword.Bluemix_notm}} API 金鑰，而不是 Softlayer API 金鑰或 {{site.data.keyword.Bluemix_notm}} 服務 API 金鑰。

1. 使用 [`bluemix iam api-key-create` 指令](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create)，建立 API 金鑰。在指令視窗中，使用 `-f` 選項以產生 API 金鑰檔，而不是顯示金鑰：

   ```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

2. 使用 API 金鑰登入。 

  您可以使用下列任何方式，以搭配使用 API 金鑰與 {{site.data.keyword.Bluemix_notm}} CLI：
    
    * 直接呼叫 API 金鑰：
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * 使用金鑰檔來呼叫 API 金鑰： 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * 設定環境變數。此外，您也可以在系統上設定環境變數。例如，BLUEMIX_API_KEY=api_key_string，其中 `api_key_string` 是 API 金鑰的自訂值。設定環境變數之後，只需要從 CLI 指定 `bluemix login` 即可。 
  
  若要使用 Cloud Foundry CLI 登入，請指定 `apikey` 作為使用者名稱，並指定 API 金鑰字串作為密碼：

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
Authenticating...
OK
```

