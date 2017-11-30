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

# フェデレーテッド ID を使用したログイン
{: #federated_id}

フェデレーテッド・ユーザーとして、ワンタイム・パスコードまたは API キーを使用してコマンド・ライン・インターフェース (CLI) から {{site.data.keyword.Bluemix}} にログインすることができます。
{: shortdesc}

## ワンタイム・パスコードの使用
{:onetime_passcode}

ワンタイム・パスコード・オプションを使用してフェデレーテッド ID でログインする場合、シングルサインオン (SSO) パラメーターを指定してワンタイム・パスコードを取得し、それをログイン時に入力します。 

ワンタイム・パスコードは {{site.data.keyword.Bluemix_notm}} コンソールからコードを取得するため、自動化スクリプトでのフェデレーテッド ID の使用は失敗します。自動化スクリプトでは API キー・オプションを使用して問題を回避します。
{: tip}

### {{site.data.keyword.Bluemix_notm}} CLIから
1. `bluemix login` コマンドに `--sso` オプションを指定します。
2. プロンプトの URL にアクセスしてワンタイム・パスコードを取得します。
3. 入力として CLI にパスコード値をコピー・アンド・ペーストします。
    
  ``` 
  bluemix login --sso
  API endpoint: https://api.ng.bluemix.net
      
  One Time Code (Get one at https://iam.ng.bluemix.net/oidc/passcode)> 
  Authenticating...
  OK
      
  ```
  
### Cloud Foundry CLI から
1. `cf login` コマンドに `--sso` オプションを指定します。 
2. プロンプトの URL にアクセスしてワンタイム・パスコードを取得します。 
3. 入力として CLI にパスコード値をコピー・アンド・ペーストします。 
    
  ```
  cf login --sso
  API endpoint: https://api.ng.bluemix.net

  One Time Code (Get one at https://login.ng.bluemix.net/UAALoginServerWAR/passcode)>
  Authenticating...
  OK
      
  ```

## API キーの使用
{:api_key}

必要な API キーは、{{site.data.keyword.Bluemix_notm}} プラットフォームでの認証に使用される {{site.data.keyword.Bluemix_notm}} の API キーです。Softlayer の API キーまたは {{site.data.keyword.Bluemix_notm}} サービスの API キーではありません。

1. [`bluemix iam api-key-create` コマンド](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_api_key_create)を使用して API キーを作成します。以下に示すように、コマンド・ウィンドウにキーを表示するのではなく API キー・ファイルを生成するには、`-f` オプションを使用します。

   ```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

2. API キーを使用してログインします。 

  API キーを {{site.data.keyword.Bluemix_notm}} CLI で使用するには、以下のいずれかの方法を使用できます。
    
    * 以下のように API キーを直接呼び出す。
  
      ```
      bluemix login --apikey <api_key_string>

      ```
    
    * 以下のようにキー・ファイルを使用して API キーを呼び出す。 
  
      ```
      bluemix login --apikey @key_file_name

      ```
    
    * 環境変数を設定します。さらに、ご使用のシステムにも環境変数を設定できます。例えば、BLUEMIX_API_KEY=api_key_string と指定します。ここで、`api_key_string` は、API キーのカスタム値です。環境変数が設定された後は、CLI から単純に `bluemix login` を指定できます。 
  
  Cloud Foundry CLI を使用してログインするには、以下のように、ユーザー名として `apikey` を指定し、パスワードとして API キー・ストリングを指定します。

    ```
    cf login
    API endpoint: https://api.ng.bluemix.net

    Email> apikey
  
    Password>
    Authenticating...
    OK

    ```

