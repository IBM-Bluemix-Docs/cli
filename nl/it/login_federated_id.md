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

# Accesso con un ID federato
{: #federated_id}

Come utente federato, puoi accedere a {{site.data.keyword.Bluemix}} dalla CLI (command-line interface) utilizzando un passcode monouso o una chiave API. 
{: shortdesc}

## Utilizzo di un passcode monouso
{:onetime_passcode}

Se utilizzi l'opzione di passcode monouso per accedere con un ID federato, devi specificare il parametro SSO (single-sign on) per ottenere un passcode monouso da immettere durante la fase di accesso. 

Poiché un passcode monouso richiama il codice della console {{site.data.keyword.Bluemix_notm}}, l'utilizzo di un ID federato nello script di automazione provoca un errore. Evita il problema utilizzando l'opzione di chiave API con lo script automatizzato. 
{: tip}

### Dalla CLI {{site.data.keyword.Bluemix_notm}}
1. Specifica l'opzione `--sso` con il comando `bluemix login`.
2. Segui l'URL nel prompt per ottenere il passcode monouso.
3. Copia e incolla il valore del passcode nella CLI.
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  Codice monouso (Ottienine uno in  https://iam.ng.bluemix.net/oidc/passcode)> 
  Autenticazione in corso...
  OK
      
  ```
  
### Dalla CLI Cloud Foundry
1. Specifica l'opzione `--sso` con il comando `cf login`. 
2. Segui l'URL nel prompt per ottenere il passcode monouso. 
3. Copia e incolla il valore del passcode nella CLI. 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  Codice monouso (Ottienine uno in https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Autenticazione in corso...
  OK
      
  ```

## Utilizzo di una chiave API
{:api_key}

La chiave API richiesta è la chiave API {{site.data.keyword.Bluemix_notm}} utilizzata per l'autenticazione con la piattaforma {{site.data.keyword.Bluemix_notm}} e non la chiave API Softlayer o la chiave API del servizio {{site.data.keyword.Bluemix_notm}}.

1. Crea una chiave API con il [comando `bluemix iam api-key-create`](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create). Utilizza l'opzione `-f` per generare un file della chiave API invece di mostrare la chiave nella finestra di comando:

   ```
   bluemix iam api-key-create NOME [-d DESCRIZIONE] [-f, --file FILE]
  
   ```

2. Accedi con la chiave API. 

  Puoi utilizzare la chiave API con la CLI {{site.data.keyword.Bluemix_notm}} in uno dei seguenti modi:
    
    * Chiama direttamente la chiave API.
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * Chiama la chiave API con il file della chiave: 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * Imposta una variabile di ambiente. Puoi anche impostare una variabile di ambiente nel tuo sistema. Ad esempio, BLUEMIX_API_KEY=api_key_string, dove `api_key_string` è il valore personalizzato della chiave API. Una volta impostata la variabile di ambiente, puoi semplicemente specificare `bluemix login` dalla CLI. 
  
  Per accedere utilizzando la CLI Cloud Foundry, specifica `apikey` come nome utente e la stringa della chiave API come password:

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
Authenticating...
OK
  
    ```

