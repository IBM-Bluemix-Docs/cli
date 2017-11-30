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

# Mit eingebundener ID anmelden
{: #federated_id}

Als eingebundener Benutzer können Sie sich bei {{site.data.keyword.Bluemix}} über die Befehlszeilenschnittstelle (CLI) anmelden, indem Sie entweder einen einmaligen Kenncode oder einen API-Schlüssel verwenden. 
{: shortdesc}

## Einmaligen Kenncode verwenden
{:onetime_passcode}

Wenn Sie die Option für den einmaligen Kenncode verwenden, um sich mit einer eingebundenen ID anzumelden, geben Sie den Single-Sign-on-Parameter (SSO) an, um einen einmaligen Kenncode anzufordern, den Sie dann bei der Anmeldung eingeben. 

Ein einmaliger Kenncode ruft Code über die {{site.data.keyword.Bluemix_notm}}-Konsole ab. Dies hat zur Folge, dass die Verwendung einer eingebundenen ID in Ihrem Automationsscript fehlschlägt. Sie können dieses Problem vermeiden, indem Sie die API-Schlüssel-Option mit einem automatisierten Script verwenden. 
{: tip}

### Über die {{site.data.keyword.Bluemix_notm}}-Befehlszeilenschnittstelle
1. Geben sie die Option `--sso` mit dem Befehl `bluemix login` an.
2. Folgen Sie der URL in der Eingabeaufforderung, um den einmaligen Kenncode abzurufen.
3. Verwenden den Kenncodewert in der Befehlszeilenschnittstelle per Cut-and-paste als Ihre Eingabe.
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### Über die Cloud Foundry-Befehlszeilenschnittstelle
1. Geben sie die Option `--sso` mit dem Befehl `cf login` an. 
2. Folgen Sie der URL in der Eingabeaufforderung, um den einmaligen Kenncode abzurufen. 
3. Verwenden den Kenncodewert in der Befehlszeilenschnittstelle per Cut-and-paste als Ihre Eingabe. 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## API-Schlüssel verwenden
{:api_key}

Der erforderliche API-Schlüssel ist der {{site.data.keyword.Bluemix_notm}}-API-Schlüssel, der für die Authentifizierung bei der {{site.data.keyword.Bluemix_notm}}-Plattform verwendet wird, und nicht der Softlayer-API-Schlüssel oder der {{site.data.keyword.Bluemix_notm}}-Service-API-Schlüssel.

1. Erstellen Sie einen API-Schlüssel mit dem Befehl [`bluemix iam api-key-create`](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create). Verwenden Sie die Option `-f`, um eine API-Schlüsseldatei zu erstellen, anstatt den Schlüssel im Befehlsfenster anzuzeigen:

   ```
   bluemix iam api-key-create NAME [-d BESCHREIBUNG] [-f, --file DATEI]
  
   ```

2. Melden Sie sich mit dem API-Schlüssel an. 

  Sie können den API-Schlüssel mit der {{site.data.keyword.Bluemix_notm}}-Befehlszeilenschnittstelle auf folgende Art und Weise verwenden:
    
    * API-Schlüssel direkt aufrufen
  
      ```
      bluemix login --apikey <api-schlüsselzeichenfolge>
    
      ```
    
    * API-Schlüssel mit der Schlüsseldatei aufrufen: 
  
      ```
      bluemix login --apikey @schlüsseldateiname
    
      ```
    
    * Legen Sie eine Umgebungsvariable fest. Darüber hinaus können Sie auf Ihrem System auch eine Umgebungsvariable definieren. Beispiel: BLUEMIX_API_KEY=api-schlüsselzeichenfolge, wobei `api-schlüsselzeichenfolge` der angepasste Wert des API-Schlüssels ist. Wenn die Umgebungsvariable definiert wurde, können Sie einfach `bluemix login` in der Befehlszeilenschnittstelle angeben. 
  
  Um sich über die Cloud Foundry-Befehlszeilenschnittstelle anzumelden, geben Sie `apikey` als Benutzernamen und die API-Schlüsselzeichenfolge als Kennwort an:

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
    Authenticating...
    OK
  
    ```

