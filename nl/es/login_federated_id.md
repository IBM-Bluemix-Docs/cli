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

# Inicio de sesión con un ID federado
{: #federated_id}

Como usuario federado, puede iniciar una sesión en {{site.data.keyword.Bluemix}} desde la interfaz de línea de mandatos (CLI) mediante un código de acceso de una sola vez o una API clave. 
{: shortdesc}

## Utilización de un código de acceso de una sola vez
{:onetime_passcode}

Cuando utiliza la opción de código de acceso de una sola vez para iniciar sesión con un ID federado, debe especificar el parámetro de inicio de sesión único (SSO) para obtener un código de acceso de una sola vez, que especificará luego en el inicio de sesión. 

Dado que un código de acceso de una sola vez recupera código de la consola de {{site.data.keyword.Bluemix_notm}}, hace que falle el uso de un ID federado en su script de automatización. Evite problemas utilizando la opción de la clave de API con un script automatizado. 
{: tip}

### Desde la CLI de {{site.data.keyword.Bluemix_notm}}
1. Especifique la opción `--sso` con el mandato `bluemix login`.
2. Siga el URL en la solicitud para obtener un código de acceso de una sola vez.
3. Copie y pegue el valor del código de acceso en la CLI como su entrada.
    
  ``` 
  bluemix login --sso
  Punto final de la API: https://api.ng.bluemix.net
      
  Código de un solo uso (obtenga uno en https://iam.ng.bluemix.net/oidc/passcode)> 
  Autenticando...
  Correcto
      
  ```
  
### Desde la CLI de Cloud Foundry
1. Especifique la opción `--sso` con el mandato `cf login`. 
2. Siga el URL en la solicitud para obtener un código de acceso de una sola vez. 
3. Copie y pegue el valor del código de acceso en la CLI como su entrada. 
    
  ```
  cf login --sso
  Punto final de la API: https://api.ng.bluemix.net
      
  Código de un solo uso (obtenga uno en https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Autenticando...
  Correcto
      
  ```

## Utilización de la clave de API
{:api_key}

La clave de API necesaria es la clave de API de {{site.data.keyword.Bluemix_notm}} que ha utilizado para autenticarse con la plataforma de {{site.data.keyword.Bluemix_notm}}, no la clave de API de Softlayer ni la clave de API del servicio de {{site.data.keyword.Bluemix_notm}}.

1. Cree una clave de API con el mandato [`bluemix iam api-key-create`](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create). Utilice la opción `-f` para generar un archivo de claves de APIen lugar de mostrar la clave en la ventana de mandatos:

   ```
   bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
  
   ```

2. Inicie la sesión con su clave de API. 

  Puede utilizar la clave de API con la CLI de {{site.data.keyword.Bluemix_notm}} en cualquiera de las formas siguientes:
    
    * Llame a la clave de API directamente:
  
      ```
      bluemix login --apikey <api_key_string>
    
      ```
    
    * Llame a la clave de API con el archivo de claves: 
  
      ```
      bluemix login --apikey @key_file_name
    
      ```
    
    * Establece una variable de entorno. Además, también puede establecer una variable de entorno en el sistema. Por ejemplo, BLUEMIX_API_KEY=api_key_string, donde `api_key_string` es el valor personalizado de la clave de API. Después de establecer la variable de entorno, puede especificar `bluemix login` desde la CLI. 
  
  Para iniciar una sesión utilizando la CLI de Cloud Foundry, especifique `apikey` como el nombre de usuario y la serie de claves de API como la contraseña:

    ```
    cf login
    Punto final de la API: https://api.ng.bluemix.net
  
    Correo electrónico> apikey
  
    Contraseña>
    Autenticando...
    Correcto
  
    ```

