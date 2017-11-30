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

# Efetuando login com um ID federado
{: #federated_id}

Como um usuário federado, é possível efetuar login no {{site.data.keyword.Bluemix}} por meio da interface da linha de comandos (CLI) usando uma senha única ou uma chave API. 
{: shortdesc}

## Usando uma senha única
{:onetime_passcode}

Ao usar a opção de senha única para efetuar login com um ID federado, você especifica o parâmetro single-sign on (SSO) para obter uma senha única, que será então inserida no login. 

Como uma senha única recupera código do console do {{site.data.keyword.Bluemix_notm}}, ela faz com que o uso de um ID federado em seu script de automação falhe. Evite problemas usando a opção de chave API com um script automatizado. 
{: tip}

### No {{site.data.keyword.Bluemix_notm}} CLI
1. Especifique a opção `--sso` com o comando `bluemix login`.
2. Siga a URL no prompt para obter a senha única.
3. Copie e cole o valor da senha na CLI como sua entrada.
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### Por meio da CLI do Cloud Foundry
1. Especifique a opção `--sso` com o comando `cf login`. 
2. Siga a URL no prompt para obter a senha única. 
3. Copie e cole o valor da senha na CLI como sua entrada. 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## Usando uma chave API
{:api_key}

A chave API necessária é a chave API do {{site.data.keyword.Bluemix_notm}} usada para se autenticar na plataforma do {{site.data.keyword.Bluemix_notm}}, não a chave API do Softlayer ou a chave API do serviço {{site.data.keyword.Bluemix_notm}}.

1. Crie uma chave API com o comando [`bluemix iam api-key-create`](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create). Use a opção `-f` para gerar um arquivo de chave API, em vez de mostrar a chave na janela de comando:

   ```
   bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
  
   ```

2. Efetue login com a chave API. 

  É possível usar a chave API com a CLI do {{site.data.keyword.Bluemix_notm}} em qualquer uma das maneiras a seguir:
    
    * Chamar a chave API diretamente:
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * Chamar a chave API com o arquivo-chave: 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * Configurar uma variável de ambiente. Além disso, também é possível configurar uma variável de ambiente em seu sistema. Por exemplo, BLUEMIX_API_KEY=api_key_string, em que `api_key_string` é o valor customizado da chave API. Após a configuração da variável de ambiente, basta especificar `bluemix login` por meio da CLI. 
  
  Para efetuar login usando a CLI do Cloud Foundry, especifique `apikey` como o nome do usuário e a keystring API como a senha:

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
Authenticating...
OK
  
    ```

