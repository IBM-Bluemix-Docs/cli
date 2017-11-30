---



copyright:

  years: 2017

lastupdated: "2017-10-26"


---

{:codeblock: .codeblock}
{:shortdesc: .shortdesc}
{:tip: .tip}
{:new_window: target="_blank"}

# {{site.data.keyword.registrylong_notm}} CLI {: #containerregcli}

{{site.data.keyword.registrylong}} CLI は、レジストリーと、{{site.data.keyword.Bluemix_notm}} アカウント用のリソースを管理するためのプラグインです。
{: shortdesc}

** の前提条件**
* レジストリー・コマンドを実行する前に、`bx login` コマンドを使用して {{site.data.keyword.Bluemix_notm}} にログインし、アクセス・トークンを生成して、セッションを認証します。

{{site.data.keyword.registrylong_notm}} CLI の使用方法については、[プライベート・イメージ・レジストリーのセットアップ (Setting up a private images registry)](../../../services/Registry/index.html) を参照してください。

<table summary="{{site.data.keyword.registrylong_notm}} の管理">
<caption>表 1. {{site.data.keyword.Bluemix_notm}} 上の {{site.data.keyword.registrylong_notm}} を管理するためのコマンド
</caption>
 <thead>
 <th colspan="5">レジストリーを管理するためのコマンド</th>
 </thead>
 <tbody>
 <tr>
 <td>[bx cr api](#bx_cr_api)</td>
 <td>[bx cr build](#bx_cr_build)</td>
 <td>[bx cr info](#bx_cr_info)</td>
 <td>[bx cr image-inspect](#bx_cr_image_inspect)</td>
 <td>[bx cr image-list (bx cr images)](#bx_cr_image_list)</td>
 </tr>
 <tr>
 <td>[bx cr image-rm](#bx_cr_image_rm)</td>
 <td>[bx cr login
](#bx_cr_login)</td>
 <td>[bx cr namespace-add](#bx_cr_namespace_add)</td>
 <td>[bx cr namespace-list (bx cr namespaces)](#bx_cr_namespace_list)</td>
 <td>[bx cr namespace-rm](#bx_cr_namespace_rm)</td>
 </tr>
 <tr>
 <td>[bx cr plan](#bx_cr_plan)</td>
 <td>[bx cr plan-upgrade](#bx_cr_plan_upgrade)</td>
 <td>[bx cr pricing](#bx_cr_pricing)</td>
 <td>[bx cr quota](#bx_cr_quota)</td>
 <td>[bx cr quota-set](#bx_cr_quota_set)</td>
 </tr>
 <tr>
 <td>[bx cr token-add](#bx_cr_token_add)</td>
 <td>[bx cr token-get](#bx_cr_token_get)</td>
 <td>[bx cr token-list (bx cr tokens)](#bx_cr_token_list)</td>
 <td>[bx cr token-rm](#bx_cr_token_rm)</td>
 <td>[bx cr vulnerability-assessment (bx cr va)](#bx_cr_va)</td>
 </tr>
 </tbody></table>



## bx cr api
{: #bx_cr_api}

コマンドの実行対象のレジストリー API エンドポイントに関する詳細を返します。

```
bx cr api
```
{: codeblock}


## bx cr build
{: #bx_cr_build}

{{site.data.keyword.registrylong_notm}} 内で Docker イメージをビルドします。

```
bx cr build [--no-cache] [--pull] [--quiet | -q] [--build-arg value ...] --tag value DIRECTORY
```
{: codeblock}

**パラメーター**
<dl>
<dt>DIRECTORY</dt>
<dd>Dockerfile と前提条件ファイルが含まれている、ビルド・コンテキストの場所。</dd>
<dt>--no-cache</dt>
<dd>(オプション)  指定されている場合、前のビルドからのキャッシュされたイメージ層はこのビルドで使用されません。</dd>
<dt>--pull</dt>
<dd>(オプション)  指定されている場合、一致するタグを持つイメージがビルド・ホスト上に既に存在していても、基本イメージがプルされます。</dd>
<dt>--quiet、-q</dt>
<dd>(オプション) 指定されている場合、エラーが発生しない限り、ビルド出力は抑止されます。</dd>
<dt> --build-arg value</dt>
<dd>(オプション) 「KEY=VALUE」のフォーマットで追加のビルド引数を指定します。このパラメーターを複数回含めることにより、複数のビルド引数を指定できます。Dockerfile 内のキーに一致する ARG 行を指定する時、ビルド引数の値は環境変数として使用できます。</dd>
<dt>--tag value, -t value</dt>
<dd>ビルドするイメージのフルネーム。これには、レジストリーの URL と名前空間が含まれます。</dd>
</dl>


## bx cr info
{: #bx_cr_info}

ログイン先のレジストリーの名前とアカウントを表示します。

```
bx cr info
```
{: codeblock}


## bx cr image-inspect
{: #bx_cr_image_inspect}

特定のイメージに関する詳細を表示します。

```
bx cr image-inspect [--format FORMAT] IMAGE [IMAGE...]
```
{: codeblock}

**パラメーター**

<dl>
<dt>--format FORMAT</dt>
<dd>(オプション) Go テンプレートを使用して、出力エレメントをフォーマットします。詳しくは、[イメージに関する情報の表示 (Viewing information about images)](../../../services/Registry/registry_cli_reference.html#registry_cli_listing) を参照してください。

</dd>
<dt>IMAGE</dt>
<dd>検査するイメージの絶対レジストリー・パス (フォーマットは `namespace/image:tag`)。イメージ・パスにタグが指定されていない場合、`latest` というタグが付いたイメージが検査されます。このコマンドでは、各パスの間をスペースで区切って、それぞれの専用レジストリー・パスをリストすることにより、複数のイメージを検査できます。</dd>
</dl>


## bx cr image-list (bx cr images)
{: #bx_cr_image_list}

{{site.data.keyword.Bluemix_notm}} アカウント内のすべてのイメージを表示します。

```
 bx cr image-list [--no-trunc] [-q, --quiet] [--include-ibm] [--format FORMAT]
```
{: codeblock}

**パラメーター**
<dl>
<dt>--no-trunc</dt>
<dd>(オプション) イメージ・ダイジェストを切り捨てません。</dd>
<dt>-q, --quiet</dt>
<dd>(オプション) 各イメージが、`repository:tag` というフォーマットでリストされます。</dd>
<dt>--include-ibm</dt>
<dd>(オプション) {{site.data.keyword.IBM_notm}} 提供のパブリック・イメージを出力に含めます。このオプションを指定しない場合、デフォルトではプライベート・イメージのみがリストされます。</dd>
<dt>--format FORMAT</dt>
<dd>(オプション) Go テンプレートを使用して、出力エレメントをフォーマットします。詳しくは、[イメージに関する情報の表示 (Viewing information about images)](../../../services/Registry/registry_cli_reference.html#registry_cli_listing) を参照してください。

</dd>
</dl>


## bx cr image-rm
{: #bx_cr_image_rm}

指定された 1 つ以上のイメージをレジストリーから削除します。

```
bx cr image-rm IMAGE [IMAGE...]
```
{: codeblock}

**パラメーター**
<dl>
<dt>IMAGE</dt>
<dd>削除するイメージの絶対レジストリー・パス (フォーマットは `namespace/image:tag`)。イメージのパスにタグが指定されていない場合、デフォルトで、`latest` というタグが付いたイメージが削除されます。このコマンドでは、各パスの間をスペースで区切って、それぞれの専用レジストリー・パスをリストすることにより、複数のイメージを削除できます。</dd>
</dl>


## bx cr login

{: #bx_cr_login}

このコマンドはレジストリーに対して `docker login` コマンドを実行します。`docker login` コマンドは、レジストリーに対して `docker push` または `docker pull` のコマンドを実行できるようにするために必要です。このコマンドは、その他の `bx cr` コマンドを実行するためには必要ではありません。Docker がインストールされていない場合、このコマンドはエラー・メッセージを返します。

```
bx cr login
```
{: codeblock}


## bx cr namespace-add
{: #bx_cr_namespace_add}

{{site.data.keyword.Bluemix_notm}} アカウントに名前空間を追加します。

```
bx cr namespace-add NAMESPACE
```
{: codeblock}

**パラメーター**
<dl>
<dt>NAMESPACE</dt>
<dd>追加する名前空間。名前空間は、同じ地域内のすべての {{site.data.keyword.Bluemix_notm}} アカウントにわたって固有でなければなりません。</dd>
</dl>


## bx cr namespace-list (bx cr namespaces)
{: #bx_cr_namespace_list}

{{site.data.keyword.Bluemix_notm}} アカウントが所有するすべての名前空間を表示します。

```
bx cr namespace-list
```
{: codeblock}


## bx cr namespace-rm
{: #bx_cr_namespace_rm}

{{site.data.keyword.Bluemix_notm}} アカウントから名前空間を削除します。名前空間を削除すると、この名前空間内のイメージが削除されます。

```
bx cr namespace-rm NAMESPACE
```
{: codeblock}

**パラメーター**
<dl>
<dt>NAMESPACE</dt>
<dd>削除する名前空間。</dd>
</dl>


## bx cr plan
{: #bx_cr_plan}

価格プランを表示します。

```
bx cr plan
```
{: codeblock}


## bx cr plan-upgrade
{: #bx_cr_plan_upgrade}

標準プランにアップグレードします。

プランについて詳しくは、[レジストリー・プラン (Registry plans)](../../../services/Registry/registry_overview.html#registry_plans) を参照してください。

```
bx cr plan-upgrade [PLAN]
```
{: codeblock}

**パラメーター**
<dl>
<dt>プラン</dt>
<dd>アップグレード先の価格プランの名前。PLAN を指定しない場合、デフォルトは `standard` です。</dd>
</dl>


## bx cr pricing
{: #bx_cr_pricing}

このコマンドは削除されました。料金カリキュレーターを使用して、推定コストを計算できます。[{{site.data.keyword.registrylong_notm}} のコストの見積もり](../../../services/Registry/registry_overview.html#registry_plan_billing)を参照してください。


## bx cr quota
{: #bx_cr_quota}

トラフィックおよびストレージの現在の割り当て量、およびそれらの割り当て量に対する使用量情報を表示します。

```
bx cr quota
```
{: codeblock}


## bx cr quota-set
{: #bx_cr_quota_set}

指定された割り当て量を変更します。

```
bx cr quota-set [--traffic VALUE] [--storage VALUE]
```
{: codeblock}

**パラメーター**
<dl>
<dt>--traffic VALUE</dt>
<dd>(オプション) トラフィック割り当て量を、指定された値 (M バイト単位) に変更します。トラフィックを設定する権限がない場合や現在の価格プランを超える値を設定した場合、操作は失敗します。</dd>
<dt>--storage VALUE</dt>
<dd>(オプション) ストレージ割り当て量を、指定された値 (M バイト単位) に変更します。ストレージ割り当て量を設定する権限がない場合や現在の価格プランを超える値を設定した場合、操作は失敗します。</dd>
</dl>


## bx cr token-add
{: #bx_cr_token_add}

レジストリーへのアクセスを制御するために使用できるトークンを追加します。

```
bx cr token-add [--description VALUE] [-q, --quiet] [--non-expiring] [--readwrite]
```

{: codeblock}


**パラメーター**
<dl>
<dt>--description VALUE</dt>
<dd>(オプション) トークンの説明としての値を指定します。これは、`bx cr token-list` を実行すると表示されます。トークンが {{site.data.keyword.containerlong_notm}} によって自動的に作成される場合、この説明は、Kubernetes クラスター名に設定されます。この場合、クラスターが除去されると、トークンは自動的に削除されます。</dd>
<dt>-q, --quiet</dt>
<dd>(オプション) 周囲のテキストを含めずに、トークンのみを表示します。</dd>
<dt>--non-expiring</dt>
<dd>(オプション) 有効期限が切れないアクセス権限を指定してトークンを作成します。このパラメーターを設定しないと、デフォルトでは、トークンからのアクセスは 24 時間後に期限切れになります。</dd>
<dt>--readwrite</dt>
<dd>(オプション) 読み取り権限および書き込み権限を付与するトークンを作成します。このオプションを指定しないと、デフォルトでは、アクセス権限は読み取り専用になります。</dd>
</dl>


## bx cr token-get
{: #bx_cr_token_get}

指定されたトークンをレジストリーから取得します。

```
bx cr token-get TOKEN
```

{: codeblock}

**パラメーター**
<dl>
<dt>TOKEN</dt>
<dd>(オプション) 取得するトークンの固有 ID。</dd>
</dl>


## bx cr token-list (bx cr tokens)
{: #bx_cr_token_list}

{{site.data.keyword.Bluemix_notm}} アカウント用に存在するすべてのトークンを表示します。

```
bx cr token-list --format FORMAT
```
{: codeblock}

**パラメーター**
<dl>
<dt>--format FORMAT</dt>
<dd>(オプション) Go テンプレートを使用して、出力エレメントをフォーマットします。詳しくは、[イメージに関する情報の表示 (Viewing information about images)](../../../services/Registry/registry_cli_reference.html#registry_cli_listing) を参照してください。

</dd>
</dl>

## bx cr token-rm
{: #bx_cr_token_rm}

指定された 1 つ以上のトークンを削除します。

```
bx cr token-rm TOKEN [TOKEN...]
```
{: codeblock}

**パラメーター**
<dl>
<dt>TOKEN</dt>
<dd>(オプション) TOKEN には、トークン自体またはトークンの固有 ID (`bx cr token-list` で表示される) のいずれかを指定できます。複数のトークンを、スペースで区切って指定できます。</dd>
</dl>


## bx cr vulnerability-assessment (bx cr va)
{: #bx_cr_va}

イメージの脆弱性評価レポートを表示します。

```
bx cr vulnerability-assessment IMAGE [IMAGE...]
```
{: codeblock}

**パラメーター**
<dl>
<dt>IMAGE</dt>
<dd>レポートを取得するイメージの絶対レジストリー・パス (フォーマットは `namespace/image:tag`)。このレポートは、イメージに、既知のパッケージ脆弱性があるかどうかを報告します。以下のオペレーティング・システムがサポートされています。

<ul>

<li>Alpine</li>
<li>CentOS</li>
<li>Debian</li>
<li>Red Hat Enterprise Linux (RHEL)</li>
<li>Ubuntu</li>
</ul>

詳しくは、[Managing image security with Vulnerability Advisor](../../../services/va/va_index.html) を参照してください。

</dd>

</dl>
