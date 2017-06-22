---



copyright:

  years: 2015，2017

lastupdated: "2017-06-30"


---

{:shortdesc: .shortdesc}

# Login Bluemix with Federated ID using Command Line Interface
{: #federated_id}

Logging into Bluemix with federated ID and password from command line interface will be rejected, you will need to use one time passcode or Bluemix API key instead. One time passcode will need to retrieve the code from Bluemix Console, so if you are using federated ID in your automation script, Bluemix API key is the only way.

Please note the API key is Bluemix API key for authentication with Bluemix platform, not the Softlayer API key or Bluemix service API key.

## Login with one time asscode
{:onetime_passcode}


If you are using Bluemix CLI, login with `--sso` option as the example below. Follow the url in the prompt to get the one time passcode, then copy and paste it as your input.

```
bluemix login --sso
API endpoint: https://api.ng.bluemix.net

One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
Authenticating...
OK

```


If you are using CF CLI, use the same way to login with `--sso` option.

```
cf login --sso
API endpoint: https://api.ng.bluemix.net

One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)> 
Authenticating...
OK

```


## Login with Bluemix API key
{:api_key}

### Create Bluemix API key

You can create Bluemix platform API key from [bluemix Console](https://console.bluemix.net), select "Manage" -> "Security" -> "Bluemix API key" after you log into the console.

Bluemix CLI also provides the command line to create API key. `-f` option will generate an API key file instead of showing the key in the command window. 

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

### login with API key using Bluemix CLI

Once you have the API key, there are a few you could use with Bluemix CLI.

```
bluemix login --apikey <api_key_string>
```

or with the key file generated with `-f` option when you create the API key

```
bluemix login --apikey @key_file_name
```

You can also set the environment variable BLUEMIX_API_KEY=<api_key_string>, then simply `bluemix login`


### login with API key using CF CLI

If you want to login with CF CLI instead of Bluemix CLI, just use “apikey” as username and the API key string as password.

```
cf login     
API endpoint: https://api.ng.bluemix.net

Email> apikey    

Password>
Authenticating...
OK
```