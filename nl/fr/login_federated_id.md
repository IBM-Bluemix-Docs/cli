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

# Connexion à l'aide d'un ID fédéré
{: #federated_id}

En tant qu'utilisateur fédéré, vous pouvez vous connecter à {{site.data.keyword.Bluemix}} à partir de l'interface de ligne de commande en utilisant un code d'accès à utilisation unique ou une clé d'API. 
{: shortdesc}

## Utilisation d'un code d'accès à utilisation unique
{:onetime_passcode}

Lorsque vous choisissez d'utiliser un code d'accès à utilisation unique pour vous connecter à l'aide d'un ID fédéré, vous spécifiez le paramètre de connexion unique (SSO) afin d'obtenir le code d'accès à utilisation unique, puis vous tapez celui-ci pour vous connecter. 

Etant donné qu'un code d'accès à utilisation unique extrait du code de la console {{site.data.keyword.Bluemix_notm}}, l'utilisation d'un ID fédéré dans votre script d'automatisation échoue. Pour éviter tout incident, choisissez d'utiliser une clé d'API avec un script d'automatisation. 
{: tip}

### Depuis l'interface de ligne de commande de {{site.data.keyword.Bluemix_notm}}
1. Spécifiez l'option `--sso` à l'aide de la commande `bluemix login`.
2. Suivez l'URL dans l'invite afin d'obtenir le code d'accès à utilisation unique.
3. Copiez et collez la valeur de code d'accès dans l'interface de ligne de commande comme valeur d'entrée.
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### Depuis l'interface de ligne de commande de Cloud Foundry
1. Spécifiez l'option `--sso` à l'aide de la commande `cf login`. 
2. Suivez l'URL dans l'invite afin d'obtenir le code d'accès à utilisation unique. 
3. Copiez et collez la valeur de code d'accès dans l'interface de ligne de commande comme valeur d'entrée. 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## Utilisation d'une clé d'API
{:api_key}

La clé d'API requise est la clé d'API {{site.data.keyword.Bluemix_notm}} qui est utilisée pour l'authentification auprès de la plateforme {{site.data.keyword.Bluemix_notm}} et non la clé d'API Softlayer ni la clé d'API de service {{site.data.keyword.Bluemix_notm}}.

1. Créez une clé d'API à l'aide de la [commandes `bluemix iam api-key-create`](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create). Utilisez l'option `-f` pour générer un fichier de clés d'API au lieu d'afficher la clé dans la fenêtre de commande :

   ```
   bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
  
   ```

2. Connectez-vous à l'aide de la clé d'API. 

  Vous pouvez utiliser la clé d'API à l'aide de l'interface de ligne de commande de {{site.data.keyword.Bluemix_notm}} en procédant de l'une des façons suivantes :
    
    * Appelez la clé d'API directement :
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * Appelez la clé d'API à l'aide du fichier de clés : 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * Configurez une variable d'environnement. Vous pouvez également définir une variable d'environnement sur votre système. Par exemple, BLUEMIX_API_KEY=api_key_string, où `api_key_string` est la valeur personnalisée de la clé d'API. Une fois la variable d'environnement définie, il vous suffit de spécifier `bluemix login` à partir de l'interface de ligne de commande. 
  
  Pour vous connecter à l'aide de l'interface de ligne de commande de Cloud Foundry, spécifiez `apikey` comme nom d'utilisateur et la chaîne de clé d'API comme mot de passe :

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net
  
    Email> apikey
  
    Password>
    Authenticating...
    OK
  
    ```

