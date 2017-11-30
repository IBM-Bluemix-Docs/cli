---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.Bluemix_notm}} (bx) コマンド
{: #bluemix_cli}

バージョン: 0.6.1

{{site.data.keyword.Bluemix_notm}} コマンド・ライン・インターフェース (CLI) では、ユーザーが {{site.data.keyword.Bluemix_notm}} と対話できるように、名前空間別にグループ化したコマンドのセットが提供されています。 

バージョン 0.5.0 以降、{{site.data.keyword.Bluemix_notm}} コマンド・ライン・クライアントは、Cloud Foundry コマンド・ライン・クライアントをインストール済み環境にバンドルしています。独自の cf cli がインストールされている場合は、{{site.data.keyword.Bluemix_notm}} CLI コマンド `bx [command]` と、独自のインストール済み環境の Cloud Foundry CLI コマンド `cf [command]` の両方を同じコンテキストで使用しないでください。cf cli を使用して {{site.data.keyword.Bluemix_notm}} CLI コンテキストで Cloud Foundry リソースを管理したい場合は、代わりに `bluemix cf [command]` を使用してください。さらに、`bluemix cf api/login/logout/target` は許可されていません。代わりに `bluemix api/login/logout/target` を使用してください。

名前、引数、オプション、前提条件、説明、および例を含め、{{site.data.keyword.Bluemix_notm}} CLI でサポートされている詳細なコマンド使用法を以下にリストします。
{:shortdesc}

**注:** *前提条件*には、コマンドを使用する前に必要なアクションがリストされています。前提条件となるアクションのないコマンドでは、**なし**とリストされています。それ以外の場合、前提条件には以下のアクションのうちの 1 つ以上が含まれます。

<dl>
<dt>エンドポイント</dt>
<dd>このコマンドを使用する前に、<code>bluemix api</code> を介して API エンドポイントを設定する必要があります。</dd>
<dt>ログイン</dt>
<dd>このコマンドを使用する前に、<code>bluemix login</code> コマンドを使用してログインする必要があります。フェデレーテッド ID でログインする場合は、「--sso」オプションを使用してワンタイム・パスコードで認証するか、「--apikey」を使用して API キーで認証します。{{site.data.keyword.Bluemix_notm}} コンソールで**「管理」** &gt; **「セキュリティー」** &gt; **「Bluemix API キー」**に移動して、API キーを作成します。
</dd>
<dt>ターゲット</dt>
<dd>このコマンドを使用する前に、<code>bluemix target</code> コマンドを使用して組織およびスペースを設定する必要があります。</dd>
<dt>Docker</dt>
<dd>このコマンドを実行するためには、Docker CLI (docker) がインストールされている必要があります。</dd>
</dl>

**注:** 短形式の Bluemix コマンドを使用できます。例えば、`bx api` は `bluemix api` の短形式です。

以下の表の索引を使用して、使用頻度の高い bluemix コマンドを
参照してください。

## 汎用 Bluemix コマンド 
{: #bx_commands_index}

<table summary="汎用 Bluemix コマンド。">
 <caption>表 1. 汎用 bluemix コマンド</caption>
 <thead>
 <th colspan="5">汎用 Bluemix コマンド</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix help](bx_cli.html#bluemix_help)</td>
 <td>[bluemix api](bx_cli.html#bluemix_api)</td>
 <td>[bluemix config](bx_cli.html#bluemix_config)</td>
 <td>[bluemix info
](bx_cli.html#bluemix_info)</td>
 <td>[bluemix cf](bx_cli.html#bluemix_cf)</td>
 </tr>
 <tr>
 <td>[bluemix login](bx_cli.html#bluemix_login) </td>
 <td>[bluemix logout](bx_cli.html#bluemix_logout) </td>
 <td>[bluemix regions](bx_cli.html#bluemix_regions)</td>
 <td>[bluemix target](bx_cli.html#bluemix_target)</td>
 <td>[bluemix update](bx_cli.html#bluemix_update)</td>
 </tr>
 </tbody>
 </table>
 
 ## {{site.data.keyword.BluSoftlayer_notm}} サービスを管理および構成するためのコマンド
  {: #bx_commands_softlayer}
  
{{site.data.keyword.BluSoftlayer_notm}} を管理するためのコマンドは Bluemix CLI にマージされました。Bluemix CLI を使用した {{site.data.keyword.BluSoftlayer_notm}} サービスの構成および管理について詳しくは、[Bluemix CLI {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) コマンド](/docs/cli/reference/softlayer/index.md#softlayer_cli)を参照してください。
 
 ## アカウント、組織、および役割を管理するためのコマンド
 {: #bx_commands_account}

<table summary="アカウント、組織、スペース、および役割を管理するために使用できる bluemix コマンド。">
<caption>表 2. アカウント、組織、スペース、および役割を管理するためのコマンド</caption>
 <thead>
 <th colspan="5">アカウント、組織、スペース、および役割を管理するためのコマンド</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix account orgs](bx_cli.html#bluemix_account_orgs)</td>
 <td>[bluemix account org](bx_cli.html#bluemix_account_org)</td>
 <td>[bluemix account org-create](bx_cli.html#bluemix_account_org_create)</td>
 <td>[bluemix account org-replicate](bx_cli.html#bluemix_account_org_replicate)</td>
 <td>[bluemix account org-rename](bx_cli.html#bluemix_account_org_rename)</td>
 </tr>
 <tr>
 <td>[bluemix account spaces](bx_cli.html#bluemix_account_spaces)</td>
 <td>[bluemix account space](bx_cli.html#bluemix_account_space)</td>
 <td>[bluemix account space-create](bx_cli.html#bluemix_account_space_create)</td>
 <td>[bluemix account space-rename](bx_cli.html#bluemix_account_space_rename)</td>
 <td>[bluemix account space-delete](bx_cli.html#bluemix_account_space_delete)</td>
 </tr>
 <tr>
 <td>[bluemix account org-users](bx_cli.html#bluemix_account_org_users)</td>
 <td>[bluemix account org-user-add](bx_cli.html#bluemix_account_org_user_add)</td>
 <td>[bluemix account org-user-remove](bx_cli.html#bluemix_account_org_user_remove)</td>
 <td>[bluemix account org-roles](bx_cli.html#bluemix_account_org_roles)</td>
 <td>[bluemix account org-role-set](bx_cli.html#bluemix_account_org_role_set)</td>
 </tr>
 <tr>
 <td>[bluemix account org-role-unset](bx_cli.html#bluemix_account_org_role_unset)</td>
 <td>[bluemix account space-users](bx_cli.html#bluemix_account_space_users)</td>
 <td>[bluemix account space-roles](bx_cli.html#bluemix_account_space_roles)</td>
 <td>[bluemix account space-role-set](bx_cli.html#bluemix_account_space_role_set)</td>
 <td>[bluemix account space-role-unset](bx_cli.html#bluemix_account_space_role_unset)</td>
</tr>
 <td>[bluemix account list](bx_cli.html#bluemix_account_list)</td>
 <td>[bluemix account org-account](bx_cli.html#bluemix_account_org_account)</td>
 <td>[bluemix account users](bx_cli.html#bluemix_account_users)</td>
 <td>[bluemix account users-delete](bx_cli.html#bluemix_account_users_delete)</td>
 <td>[bluemix account user-invite](bx_cli.html#bluemix_account_user_invite)</td>
 </tr>
 <tr>
  <td>[bluemix account user-reinvite](bx_cli.html#bluemix_account_user_reinvite)</td>
 </tr>
 </tbody>
 </table>


 ## リソース・グループとリソースを管理するためのコマンド
{: #bx_commands_resource}

<table summary="リソース・グループとリソースを管理するために使用できる bluemix コマンド。">
  <caption>表 3. リソース・グループとリソースを管理するためのコマンド</caption>
  <thead>
    <th colspan="5">リソース・グループとリソースを管理するためのコマンド</th>
  </thead>
  <tbody>
    <tr>
      <td>[bluemix resource groups](bx_cli.html#bluemix_resource_groups)</td>
      <td>[bluemix resource group](bx_cli.html#bluemix_resource_group)</td>
      <td>[bluemix resource group-update](bx_cli.html#bluemix_resource_group_update)</td>
      <td>[bluemix resource quotas](bx_cli.html#bluemix_resource_quotas)</td>
      <td>[bluemix resource quota](bx_cli.html#bluemix_resource_quota)</td>
    </tr>
    <tr>
      <td>[bluemix resource instances](bx_cli.html#bluemix_resource_instances)</td>
      <td>[bluemix resource instance](bx_cli.html#bluemix_resource_instance)</td>
      <td>[bluemix resource instance-create](bx_cli.html#bluemix_resource_instance-create)</td>
      <td>[bluemix resource instance-update](bx_cli.html#bluemix_resource_instance-update)</td>
      <td>[bluemix resource instance-delete](bx_cli.html#bluemix_resource_instance-delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource bindings](bx_cli.html#bluemix_resource_bindings)</td>
      <td>[bluemix resource binding](bx_cli.html#bluemix_resource_binding)</td>
      <td>[bluemix resource binding-create](bx_cli.html#bluemix_resource_binding-create)</td>
      <td>[bluemix resource binding-delete](bx_cli.html#bluemix_resource_binding-delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource keys](bx_cli.html#bluemix_resource_keys)</td>
      <td>[bluemix resource key](bx_cli.html#bluemix_resource_key)</td>
      <td>[bluemix resource key-create](bx_cli.html#bluemix_resource_key-create)</td>
      <td>[bluemix resource key-delete](bx_cli.html#bluemix_resource_key-delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource aliases](bx_cli.html#bluemix_resource_aliases)</td>
      <td>[bluemix resource alias](bx_cli.html#bluemix_resource_alias)</td>
      <td>[bluemix resource alias-create](bx_cli.html#bluemix_resource_alias-create)</td>
      <td>[bluemix resource alias-update](bx_cli.html#bluemix_resource_alias-update)</td>
      <td>[bluemix resource alias-delete](bx_cli.html#bluemix_resource_alias-delete)</td>
    </tr>
  </tbody>
</table>

 
 ## API キーとポリシーを管理するためのコマンド
 {: #bx_commands_iam}
 <table summary="API キーとポリシーを管理するために使用できる bluemix コマンド。">
 <caption>表 3. API キーとポリシーを管理するためのコマンド</caption>
  <thead>
  <th colspan="5">API キーとポリシーを管理するためのコマンド</th>
  </thead>
  <tbody>
  <tr>
   <td>[bluemix iam service-id](bx_cli.html#bluemix_iam_service_id)</td>
   <td>[bluemix iam service-id-create](bx_cli.html#bluemix_iam_service_id_create)</td>
   <td>[bluemix iam service-id-update](bx_cli.html#bluemix_iam_service_id_update)</td>
   <td>[bluemix iam service-id-delete](bx_cli.html#bluemix_iam_service_id_delete)</td>
   <td>[bluemix iam service-ids](bx_cli.html#bluemix_iam_service_ids)</td>
  </tr>
  <tr>
   <td>[bluemix iam api-keys](bx_cli.html#bluemix_iam_api_keys)</td>
   <td>[bluemix iam api-key-create](bx_cli.html#bluemix_iam_api_key_create)</td>
   <td>[bluemix iam api-key-delete](bx_cli.html#bluemix_iam_api_key_delete)</td>
   <td>[bluemix iam api-key-update](bx_cli.html#bluemix_iam_api_key_update)</td>
   <td>[bluemix iam service-api-keys](bx_cli.html#bluemix_iam_service_api_keys)</td>
  </tr>
  <tr>
   <td>[bluemix iam service-api-key](bx_cli.html#bluemix_iam_service_api_key)</td>
   <td>[bluemix iam service-api-key-create](bx_cli.html#bluemix_iam_service_api_key_create)</td>
   <td>[bluemix iam service-api-key-update](bx_cli.html#bluemix_iam_service_api_key_update)</td>
   <td>[bluemix iam service-api-key-delete](bx_cli.html#bluemix_iam_service_api_key_delete)</td>
   <td>[bluemix iam service-policies](bx_cli.html#bluemix_iam_service_policies)</td>
  </tr>
  <tr>
    <td>[bluemix iam service-policy](bx_cli.html#bluemix_iam_service_policy)</td>
    <td>[bluemix iam service-policy-create](bx_cli.html#bluemix_iam_service_policy_create)</td>
    <td>[bluemix iam service-policy-update](bx_cli.html#bluemix_iam_service_policy_update)</td>
    <td>[bluemix iam service-policy-delete](bx_cli.html#bluemix_iam_service_policy_delete)</td>
    <td>[bluemix iam user-policies](bx_cli.html#bluemix_iam_user_policies)</td>
  </tr>
  <tr>
   <td>[bluemix iam user-policy](bx_cli.html#bluemix_iam_user_policy)</td>
   <td>[bluemix iam user-policy-create](bx_cli.html#bluemix_iam_user_policy_create)</td>
   <td>[bluemix iam user-policy-update](bx_cli.html#bluemix_iam_user_policy_update)</td>
   <td>[bluemix iam user-policy-delete](bx_cli.html#bluemix_iam_user_policy_delete)</td>
  </tr>
  </tbody>
  </table>
 
 ## CF アプリとアプリ関連ドメイン、経路、および証明書を管理するためのコマンド
 {: #bx_commands_apps}

<table summary="CF アプリとアプリ関連ドメイン、経路、および証明書を管理するために使用できる bluemix コマンド。">
<caption>表 4. CF アプリとアプリ関連ドメイン、経路、および証明書を管理するためのコマンド</caption>
 <thead>
 <th colspan="5">CF アプリとアプリ関連ドメイン、経路、および証明書を管理するためのコマンド</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix app push](bx_cli.html#bluemix_app_push)</td>
 <td>[bluemix app list](bx_cli.html#bluemix_app_list)</td>
 <td>[bluemix app show](bx_cli.html#bluemix_app_show)</td>
 <td>[bluemix app delete](bx_cli.html#bluemix_app_delete)</td>
 <td>[bluemix app rename](bx_cli.html#bluemix_app_rename)</td>
 </tr>
 <tr>
 <td>[bluemix app start](bx_cli.html#bluemix_app_start)</td>
 <td>[bluemix app stop](bx_cli.html#bluemix_app_stop)</td>
 <td>[bluemix app restart](bx_cli.html#bluemix_app_restart)</td>
 <td>[bluemix app restage](bx_cli.html#bluemix_app_restage)</td>
 <td>[bluemix app instance-restart](bx_cli.html#bluemix_app_instance_restart)</td>
 </tr>
 <tr>
 <td>[bluemix app events](bx_cli.html#bluemix_app_events)</td>
 <td>[bluemix app files](bx_cli.html#bluemix_app_files)</td>
 <td>[bluemix app logs](bx_cli.html#bluemix_app_logs)</td>
 <td>[bluemix app env](bx_cli.html#bluemix_app_env)</td>
 <td>[bluemix app env-set](bx_cli.html#bluemix_app_env_set)</td>
 </tr>
 <tr>
 <td>[bluemix app env-unset](bx_cli.html#bluemix_app_env_unset)</td>
 <td>[bluemix app stacks](bx_cli.html#bluemix_app_stacks)</td>
 <td>[bluemix app stack-show](bx_cli.html#bluemix_app_stack_show)</td>
 <td>[bluemix app manifest-create](bx_cli.html#bluemix_app_manifest_create)</td>
 <td>[bluemix app domain-cert](bx_cli.html#bluemix_app_domain_cert)</td>
 </tr>
 <tr>
  <td>[bluemix app domain-cert-add](bx_cli.html#bluemix_app_domain_cert_add)</td>
  <td>[bluemix app domain-cert-remove](bx_cli.html#bluemix_app_domain_cert_remove)</td>
  <td>[bluemix app domains](bx_cli.html#bluemix_app_domains)</td>
  <td>[bluemix app domain-create](bx_cli.html#bluemix_app_domain_create)</td>
  <td>[bluemix app domain-delete](bx_cli.html#bluemix_app_domain_delete)</td>
 </tr>
 <tr>
  <td>[bluemix app shared-domain-create](bx_cli.html#bluemix_app_shared_domain_create)</td>
  <td>[bluemix app shared-domain-delete](bx_cli.html#bluemix_app_shared_domain_delete)</td>
  <td>[bluemix app routes](bx_cli.html#bluemix_app_routes)</td>
  <td>[bluemix app route-check](bx_cli.html#bluemix_app_route_check)</td>
  <td>[bluemix app route-map](bx_cli.html#bluemix_app_route_map)</td>
 </tr>
 <tr>
  <td>[bluemix app route-unmap](bx_cli.html#bluemix_app_route_unmap)</td>
  <td>[bluemix app route-create](bx_cli.html#bluemix_app_route_create)</td>
  <td>[bluemix app route-delete](bx_cli.html#bluemix_app_route_delete)</td>
  <td>[bluemix app orphaned-routes-delete](bx_cli.html#bluemix_app_orphaned_routes_delete)</td>
  <td></td>
 </tr>
  </tbody>
 </table>
 
 ## Bluemix サービスを管理するためのコマンド
 {: #bx_commands_services}

<table summary="Bluemix サービスの管理に使用することができる Bluemix コマンド。">
 <caption>表 5. Bluemix サービスを管理するためのコマンド</caption>
 <thead>
 <th colspan="5">Bluemix サービスを管理するためのコマンド</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix service offerings](bx_cli.html#bluemix_service_offerings)</td>
 <td>[bluemix service list](bx_cli.html#bluemix_service_list)</td>
 <td>[bluemix service show](bx_cli.html#bluemix_service_show)</td>
 <td>[bluemix service create](bx_cli.html#bluemix_service_create)</td>
 <td>[bluemix service update](bx_cli.html#bluemix_service_update)</td>
 </tr>
 <tr>
 <td>[bluemix service delete](bx_cli.html#bluemix_service_delete)</td>
 <td>[bluemix service rename](bx_cli.html#bluemix_service_rename)</td>
 <td>[bluemix service bind](bx_cli.html#bluemix_service_bind)</td>
 <td>[bluemix service unbind](bx_cli.html#bluemix_service_unbind)</td>
 <td>[bluemix service key-create](bx_cli.html#bluemix_service_key_create)</td>
 </tr>
 <tr>
 <td>[bluemix service key-delete](bx_cli.html#bluemix_service_key_delete)</td>
 <td>[bluemix service keys](bx_cli.html#bluemix_service_keys)</td>
 <td>[bluemix service key-show](bx_cli.html#bluemix_service_key_show)</td>
 <td>[bluemix service user-provided-create](bx_cli.html#bluemix_service_user_provided_create)</td>
 <td>[bluemix service user-provided-update](bx_cli.html#bluemix_service_user_provided_update)</td>
 </tr>
  </tbody>
 </table>

 
 ## カタログ、プラグイン、および請求処理の設定を管理するためのコマンド
 {: #bx_commands_settings}

<table summary="Bluemix カタログ、プラグイン、請求、およびセキュリティー設定の管理に使用できる Bluemix コマンド。">
 <caption>表 6. Bluemix カタログ、プラグイン、請求、およびセキュリティー設定を管理するためのコマンド</caption>
 <thead>
 <th colspan="5">Bluemix カタログ、プラグイン、請求、およびセキュリティー設定を管理するためのコマンド</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix catalog search](bx_cli.html#bluemix_catalog_search)</td>
  <td>[bluemix catalog entry](bx_cli.html#bluemix_catalog_entry)</td>
  <td>[bluemix catalog entry-create](bx_cli.html#bluemix_catalog_entry-create)</td>
  <td>[bluemix catalog entry-update](bx_cli.html#bluemix_catalog_entry-update)</td>
  <td>[bluemix catalog entry-visibility](bx_cli.html#bluemix_catalog_entry-visibility)</td>
 </tr>
 <tr>
  <td>[bluemix catalog service-marketplace](bx_cli.html#bluemix_catalog_service-marketplace)</td>
  <td>[bluemix catalog entry-visibility-set](bx_cli.html#bluemix_catalog_entry-visibility-set)</td>
  <td>[bluemix catalog templates](bx_cli.html#bluemix_catalog_templates)</td>
  <td>[bluemix catalog template](bx_cli.html#bluemix_catalog_template)</td>
  <td>[bluemix catalog template-run](bx_cli.html#bluemix_catalog_template_run)</td>
 </tr>
 <tr>
  <td>[bluemix plugin repos](bx_cli.html#bluemix_plugin_repos)</td>
  <td>[bluemix plugin repo-add](bx_cli.html#bluemix_plugin_repo_add)</td>
  <td>[bluemix plugin repo-remove](bx_cli.html#bluemix_plugin_repo_remove)</td>
  <td>[bluemix plugin repo-plugins](bx_cli.html#bluemix_plugin_repo_plugins)</td>
  <td>[bluemix plugin repo-plugin](bx_cli.html#bluemix_plugin_repo_plugin)</td>
 </tr>
 <tr>
  <td>[bluemix plugin list](bx_cli.html#bluemix_plugin_list)</td>
  <td>[bluemix plugin install](bx_cli.html#bluemix_plugin_install)</td>
  <td>[bluemix plugin uninstall](bx_cli.html#bluemix_plugin_uninstall)</td>
  <td>[bluemix plugin update](bx_cli.html#bluemix_plugin_update)</td>
  <td>[bluemix billing account-usage](bx_cli.html#bluemix_billing_account_usage)</td>
 </tr>
 <tr>
  <td>[bluemix billing org-usage](bx_cli.html#bluemix_billing_org_usage)</td>
  <td>[bluemix billing orgs-usage-summary](bx_cli.html#bluemix_billing_orgs_usage_summary)</td>
 </tr>
 </tbody>
 </table>
 
## bluemix help
{: #bluemix_help}
{{site.data.keyword.Bluemix_notm}} CLI の第 1 レベルの組み込みコマンドおよびサポートされる名前空間に関する一般ヘルプを表示するか、または、特定の組み込みコマンドまたは名前空間に関するヘルプを表示します。

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>COMMAND|NAMESPACE (オプション)</dt>
   <dd>ヘルプを表示する対象のコマンドまたは名前空間。指定されない場合、{{site.data.keyword.Bluemix_notm}} CLI の一般ヘルプが表示されます。</dd>
   </dl>



<strong>例</strong>:

{{site.data.keyword.Bluemix_notm}} CLI の一般ヘルプを表示します。

```
bluemix help
```

`info` コマンドのヘルプを表示します。

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
{{site.data.keyword.Bluemix_notm}} API エンドポイントを設定または表示します。

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>API_ENDPOINT (オプション)</dt>
   <dd>ターゲットの API エンドポイント (例えば `https://api.chinabluemix.net`)。 *API_ENDPOINT* オプションと `--unset` オプションのどちらも指定されない場合、現行 API エンドポイントが表示されます。</dd>
   <dt>--unset (オプション)</dt>
   <dd>API エンドポイント設定を削除します。</dd>
   <dt>--skip-ssl-validation (オプション)</dt>
   <dd>HTTP 要求の SSL 検証をバイパスします。 </dd>
   </dl>
<strong>例</strong>:

API エンドポイントを api.chinabluemix.net に設定します。

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

現行 API エンドポイントを表示します。

```
bluemix api
```

API エンドポイントを設定解除します。

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


構成ファイルにデフォルト値を書き込みます。

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>HTTP 要求のタイムアウト値。デフォルト値は 60 秒です。</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>端末または指定されたファイルへの HTTP 要求をトレースします。</dd>
   <dt>--color true|false</dt>
   <dd>カラー出力を使用可能または使用不可にします。カラー出力はデフォルトで使用可能に設定されています。</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>デフォルト・ロケールを設定します。LOCALE  が <i>CLEAR</i> の場合は、前のロケールが削除されます。</dd>
   <dt>--check-version true|false</dt>
   <dd>CLI バージョン・チェックを使用可能または使用不可にします。</dd>
   </dl>

一度に指定できるのは、これらのオプションの 1 つだけです。

<strong>例</strong>:

次のように、HTTP 要求タイムアウトを 30 秒に設定します。

```
bluemix config --http-timeout 30
```

次のように、HTTP 要求のトレース出力を使用可能にします。

```
bluemix config --trace true
```

次のように、指定されたファイル */home/usera/my_trace* への HTTP 要求をトレースします。

```
bluemix config --trace /home/usera/my_trace
```

次のように、カラー出力を使用不可にします。

```
bluemix config --color false
```

次のように、ロケールを zh_Hans に設定します。

```
bluemix config --locale zh_Hans
```

次のように、ロケール設定をクリアします。

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

基本的な {{site.data.keyword.Bluemix_notm}} 情報を表示します。これには、現行領域、クラウド・コントローラーのバージョン、および、いくつかの有用なエンドポイント (例えば、ログイン用のエンドポイントや、アクセス・トークン交換用のエンドポイントなど) が含まれます。

```
bluemix info
```

<strong>前提条件</strong>: エンドポイント


## bluemix cf
{: #bluemix_cf}

組み込み CF CLI を呼び出します

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-q, --quiet</dt>
  <dd>「cf コマンドの呼び出し中...」というメッセージをオフにします</dd>
</dl>

<strong>例</strong>:

cf アプリをリストします

```
bluemix cf apps
```

「cf コマンドの呼び出し中...」というメッセージを表示せずに cf サービスをリストします

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

ユーザーをログインします。 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>前提条件</strong>: なし

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>コマンド・オプション</strong>:
<dl>
  <dt> -a <i>API_ENDPOINT</i> (オプション)</dt>
  <dd> API エンドポイント (例: api.ng.bluemix.net)</dd>
  <dt> --apikey <i>API_KEY または @API_KEY_FILE_PATH</i>
  <dd> API キーの内容、または @ で示された API キー・ファイルのパス</dd>
  <dt> --sso (オプション) </dt>
  <dd> ワンタイム・パスコードを使用してログインします</dd>
  <dt> -u <i>USERNAME</i> (オプション)</dt>
  <dd> ユーザー名</dd>
  <dt> -p <i>PASSWORD</i> (オプション)</dt>
  <dd> パスワード</dd>
  <dt> -c <i>ACCOUNT_ID</i> (オプション) </dt>
  <dd> ターゲット・アカウントの ID</dd>
  <dt> -o <i>ORG_NAME</i> (オプション)</dt>
  <dd> ターゲット組織の名前 </dd>
  <dt> -s <i>SPACE_NAME</i> (オプション)</dt>
  <dd> ターゲット・スペースの名前</dd>
  <dt> --skip-ssl-validation (オプション) </dt>
  <dd> HTTP 要求の SSL 検証をバイパスします。このオプションは推奨されません。</dd>
</dl>

<strong>例</strong>:

#### 対話式ログイン

```
bluemix login```

以下のように、ユーザー名とパスワードを使用してログインし、ターゲットのアカウント、組織、およびスペースを設定します。

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

ワンタイム・パスコードを使用してログインし、ターゲット・アカウント、組織、およびスペースを設定します

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

API キーを使用してログインし、ターゲットを設定します。

#### API キーにアカウントが関連付けられている

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### API キーにアカウントが関連付けられていない

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>注:</strong> API キーに、関連付けられたアカウントがある場合、別のアカウントへの切り替えは許可されません。

#### ワンタイム・パスコードを使用する

```
bluemix login -u UserID --sso
```

すると、CLI は以下のように URL リンクを提供し、パスコードの入力を要求します。
```
One Time Code (Get one at https://URL_Link_To_Obtain_Passcode):
```

ブラウザーでこのリンクを開くと、パスコードを取得するための案内が表示されます。提供されたパスコードをコンソールに入力するとログインできます。

## bluemix logout
{: #bluemix_logout}

ユーザーをログアウトします。

```
bluemix logout
```

<strong>前提条件</strong>: なし

## bluemix regions
{: #bluemix_regions}

{{site.data.keyword.Bluemix_notm}} のすべての地域の情報を表示します。

```
bluemix regions
```

<strong>前提条件</strong>: エンドポイント


## bluemix target
{: #bluemix_target}


ターゲット・アカウント、地域、組織、またはスペースを設定するか表示します。

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>-r <i>REGION_NAME</i> (オプション)</dt>
   <dd>切り替え先の地域の名前。例えば、「us-south」または「eu-gb」など。</dd>
   <dt>-c <i>ACCOUNT_ID</i> (オプション)</dt>
   <dd>ターゲットとなるアカウントの ID。</dd>
   <dt>--cf</dt>
   <dd>ターゲットの組織およびスペースを対話式に選択します</dd>
   <dt>-o <i>ORG_NAME</i> (オプション)</dt>
   <dd>ターゲットとなる組織の名前。</dd>
   <dt>-s <i>SPACE_NAME</i> (オプション)</dt>
   <dd>ターゲットとなるスペースの名前。</dd>
   </dl>
どのオプションも指定されていない場合、現行のアカウント、地域、組織、およびスペースが表示されます。

<strong>例</strong>:

現行のアカウント、組織、およびスペースを設定します。

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

新しい地域に切り替えます。

```
bluemix target -r eu-gb
```

現行のアカウント、地域、組織、およびスペースを表示します。

```
bluemix target
```

### bluemix update
{: #bluemix_update}

CLI を最新バージョンに更新します。

```
bluemix update
```

<strong>前提条件</strong>: なし

### bluemix account orgs
{: #bluemix_account_orgs}

すべての組織をリストします。

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>-r <i>REGION</i> (オプション)</dt>
   <dd>どの地域の組織情報を表示するかを指定します。'all' に設定された場合は、すべての地域のすべての組織がリストされます。</dd>
   <dt>--guid (オプション)</dt>
   <dd>組織の GUID を表示します。</dd>
   </dl>

<strong>例</strong>:

地域 `us-south` 内のすべての組織を、GUID の
出力と共にリストします。

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

指定された組織の情報を表示します。

```
bluemix account org ORG_NAME [--guid]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>ORG_NAME (必須)</dt>
   <dd>組織の名前。</dd>
   <dt>--guid (オプション)</dt>
   <dd>組織の GUID を表示します。</dd>
   </dl>

<strong>例</strong>:

組織 `IBM`
の情報を、GUID の出力と共に表示します

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

新しい組織を作成します。この操作は、アカウントの所有者のみが実行できます。  

```
bluemix account org-create ORG_NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>ORG_NAME (必須)</dt>
   <dd>作成される組織の名前。</dd>
   </dl>

<strong>例</strong>:

名前が `IBM` という組織を作成します。

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

現在の地域から別の地域に組織を複製します。

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>ORG_NAME (必須)</dt>
   <dd>複製する既存の組織の名前。</dd>
   <dt>REGION_NAME (必須)</dt>
   <dd>複製された組織をホストする地域の名前。</dd>
   </dl>

<strong>例</strong>:

組織 `myorg` を地域 `eu-gb` に複製します。

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

組織の名前を変更します。この操作は、組織の管理者のみが実行できます。

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>OLD_ORG_NAME (必須)</dt>
   <dd>名前を変更する組織の古い名前。</dd>
   <dt>NEW_ORG_NAME (必須)</dt>
   <dd>名前を変更する組織の新しい名前。</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

このコマンドの機能とオプションは `cf spaces` コマンドと同じです。


## bluemix account space
{: #bluemix_account_space}

このコマンドの機能とオプションは `cf space` コマンドと同じです。


## bluemix account space-create
{: #bluemix_account_space_create}

このコマンドの機能とオプションは `cf create-space` コマンドと同じです。


## bluemix account space-rename
{: #bluemix_account_space_rename}


このコマンドの機能とオプションは `cf rename-space` コマンドと同じです。


## bluemix account space-delete
{: #bluemix_account_space_delete}


このコマンドの機能とオプションは `cf delete-space` コマンドと同じです。

## bluemix account org-users
{: #bluemix_account_org_users}

指定された組織内のユーザーを役割別に表示します

```
bluemix account org-users ORG_NAME [-a]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>ORG_NAME (必須)</dt>
<dd>組織の名前。</dd>
<dt>-a (オプション)</dt>
<dd>指定された組織内のすべてのユーザーを、役割別にグループ化せずにリストします。</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

組織にユーザーを追加します (組織管理者が必要)。

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

組織からユーザーを削除します (組織管理者またはユーザー本人のみ)

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>コマンド・オプション</strong>:
<dl>
<dt>--force, -f</dt>
<dd>確認なしで削除を強制します。</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

現行ユーザーのすべての組織の役割を取得します

```
bluemix account org-roles```

<strong>前提条件</strong>: エンドポイント、ログイン

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

組織の役割をユーザーに割り当てます。この操作は、組織の管理者のみが実行できます。  

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
  <dl>
   <dt>USER_NAME (必須)</dt>
   <dd>割り当てられるユーザーの名前。</dd>
   <dt>ORG_NAME (必須)</dt>
   <dd>このユーザーの割り当て先の組織の名前。</dd>
   <dt>ORG_ROLE (必須)</dt>
   <dd>このユーザーの割り当て先の組織内での役割の名前。以下に例を示します。
<ul>
   <li>OrgManager: この役割は、ユーザーの招待と管理、プランの選択と変更、支払上限の設定を行います。</li>
   <li>BillingManager: この役割は、請求アカウントと支払い情報の作成および管理を行えます。</li>
   <li>OrgAuditor: この役割は、組織の情報とレポートに読み取りアクセスだけが可能です。</li>
   </ul>
   </dd>
  </dl>

<strong>例</strong>:

ユーザー `Mary` を組織 `IBM` に役割 `OrgManager` として割り当てるには、次のように指定します。

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**注**: 組織/スペースの役割は CLI を使用して設定できますが、その他の許可を設定したい場合は、UI を使用する必要があります。詳細については、[ユーザー・アクセスの割り当て](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)を参照してください。<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

組織の役割をユーザーから削除します。この操作は、組織の管理者のみが実行できます。  

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>USER_NAME (必須)</dt>
   <dd>削除されるユーザーの名前。</dd>
   <dt>ORG_NAME (必須)</dt>
   <dd>このユーザーの削除元の組織の名前。</dd>
   <dt>ORG_ROLE (必須)</dt>
   <dd>このユーザーの削除元の組織内での役割の名前。以下に例を示します。
<ul>
   <li>OrgManager: この役割は、ユーザーの招待と管理、プランの選択と変更、支払上限の設定を行います。</li>
   <li>BillingManager: この役割は、請求アカウントと支払い情報の作成および管理を行えます。</li>
   <li>OrgAuditor: この役割は、組織の情報とレポートに読み取りアクセスだけが可能です。</li>
   </ul>
   </dd>
    </dl>

<strong>例</strong>:

ユーザー `Mary` を組織 `IBM` の役割 `OrgManager` から削除するには、次のように指定します。

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

指定されたスペース内のユーザーを役割別に表示します

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>ORG_NAME (必須)</dt>
   <dd>組織の名前。</dd>
   <dt>SPACE_NAME (必須)</dt>
   <dd>スペースの名前。</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

スペースの役割をユーザーに割り当てます。この操作は、スペースの管理者のみが実行できます。  

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>USER_NAME (必須)</dt>
   <dd>割り当てられるユーザーの名前。</dd>
   <dt>ORG_NAME (必須)</dt>
   <dd>このユーザーの割り当て先の組織の名前。</dd>
   <dt>SPACE_NAME (必須)</dt>
   <dd>このユーザーの割り当て先のスペースの名前。</dd>
   <dt>SPACE_ROLE (必須)</dt>
   <dd>このユーザーの割り当て先のスペース内での役割の名前。以下に例を示します。
<ul>
   <li>SpaceManager: この役割は、ユーザーの招待と管理を行い、特定のスペースに対してフィーチャーを有効にします。</li>
   <li>SpaceDeveloper: この役割は、アプリとサービスを作成して管理し、ログとレポートを表示します。</li>
   <li>SpaceAuditor: この役割は、ログ、レポート、スペースの設定を表示できます。 </li>
   </ul></dd>
    </dl>

<strong>例</strong>:

ユーザー `Mary` を組織 `IBM` およびスペース `Cloud` に役割 `SpaceManager` として割り当てるには、次のように指定します。

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

スペースの役割をユーザーから削除します。この操作は、スペースの管理者のみが実行できます。  

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>USER_NAME (必須)</dt>
   <dd>削除されるユーザーの名前。</dd>
   <dt>ORG_NAME (必須)</dt>
   <dd>このユーザーの削除元の組織の名前。</dd>
   <dt>SPACE_NAME (必須)</dt>
   <dd>このユーザーの削除元のスペースの名前。</dd>
   <dt>SPACE_ROLE (必須)</dt>
   <dd>このユーザーの削除元のスペース内での役割の名前。以下に例を示します。
<ul>
   <li>SpaceManager: この役割は、ユーザーの招待と管理を行い、特定のスペースに対してフィーチャーを有効にします。</li>
   <li>SpaceDeveloper: この役割は、アプリとサービスを作成して管理し、ログとレポートを表示します。</li>
   <li>SpaceAuditor: この役割は、ログ、レポート、スペースの設定を表示できます。 </li>
   </ul></dd>
    </dl>


<strong>例</strong>:

ユーザー `Mary` を組織 `IBM` と、役割 `SpaceManager` としてのスペース `Cloud` から削除するには、次のように指定します。

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

現行ユーザーのすべてのアカウントをリストします

```
bluemix account list```

<strong>前提条件</strong>: エンドポイント、ログイン


## bluemix account org-account
{: #bluemix_account_org_account}

指定された組織のアカウントを表示します (組織のユーザーが必要)。

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
  <dt>--guid (オプション)</dt>
  <dd>アカウント ID のみを表示します</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

アカウントに関連付けられているユーザーを表示します。この操作は、アカウントの所有者のみが実行できます。

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

現行アカウントからユーザーを削除します (アカウント所有者のみ)

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>USERNAME (必須)</dt>
<dd>ユーザー名</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>アカウント ID。指定しない場合、現行アカウントがデフォルトで使用されます。</dd>
<dt>--force、-f (オプション)</dt>
<dd>確認なしで削除を強制します。</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

組織とスペースの役割が既に設定されているアカウントにユーザーを招待します。この操作は、アカウントの所有者のみが実行できます。

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
   <dt>USER_NAME (必須)</dt>
   <dd>招待されるユーザーの名前。</dd>
   <dt>ORG_NAME (必須)</dt>
   <dd>このユーザーの招待先の組織の名前。</dd>
   <dt>ORG_ROLE (必須)</dt>
   <dd>このユーザーの招待先の組織内での役割の名前。以下に例を示します。
<ul>
  <li>OrgManager: この役割は、ユーザーの招待と管理、プランの選択と変更、支払上限の設定を行います。</li>
  <li>BillingManager: この役割は、請求アカウントと支払い情報の作成および管理を行えます。</li>
  <li>OrgAuditor: この役割は、組織の情報とレポートに読み取りアクセスだけが可能です。</li>
  </ul> </dd>
   <dt>SPACE_NAME (必須)</dt>
   <dd>このユーザーの招待先のスペースの名前。</dd>
   <dt>SPACE_ROLE (必須)</dt>
   <dd>このユーザーの招待先のスペースの名前。このユーザーの招待先のスペース内での役割の名前。以下に例を示します。
<ul>
<li>SpaceManager: この役割は、ユーザーの招待と管理を行い、特定のスペースに対してフィーチャーを有効にします。</li>
<li>SpaceDeveloper: この役割は、アプリとサービスを作成して管理し、ログとレポートを表示します。</li>
<li>SpaceAuditor: この役割は、ログ、レポート、スペースの設定を表示できます。 </li>
</ul>
</dd>
</dl>

<strong>例</strong>:

ユーザー `Mary` を組織 `IBM` に役割 `OrgManager` として招待し、スペース `Cloud` に役割 `SpaceAuditor` として招待するには、次のように指定します。

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**注**: 組織/スペースの役割は、CLI を使用して招待中に設定できますが、その他の許可を設定したい場合は、UI を使用する必要があります。詳細については、[ユーザー・アクセスの割り当て](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)を参照してください。<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

ユーザーに招待を再送信します (組織管理者かアカウント所有者が必要)

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

すべてのサービス ID をリストします

```
bluemix iam service-ids --uuid
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>サービス ID の UUID のみを表示します</dd>
</dl>

<strong>例</strong>:
現行アカウントに含まれているすべてのサービス ID の UUID をリストします

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

サービス ID の詳細を表示します

```
bluemix iam service-id NAME [--uuid]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>サービスの名前</dd>
  <dt>-uuid</dt>
  <dd>サービス ID の UUID を表示します</dd>
</dl>

<strong>例</strong>:

サービス ID `sample-test` の詳細を表示します

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

サービス ID を作成します

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>サービスの名前</dd>
  <dt>-d, --description</dt>
  <dd>サービス ID の説明</dd>
</dl>

<strong>例</strong>:

サービス名 `sample-test` と説明 `hello, world!` でサービス ID を作成します

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
サービス ID を更新します

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>サービスの名前</dd>
  <dt>-n, --name</dt>
  <dd>サービスの新しい名前</dd>
  <dt>-d, --description</dt>
  <dd>サービスの新しい説明</dd>
  <dt>-v, --version</dt>
  <dd>サービス ID のバージョン</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに更新します</dd>
</dl>

<strong>例</strong>:

確認を求めずにサービス ID `sample-test` を `sample-test-2` に名前変更します

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

サービス `sample-test` バージョン `1-0jn39fbefew` の説明を更新します

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

サービス ID を削除します

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>サービスの名前</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに削除します</dd>
</dl>

<strong>例</strong>:

確認を求めずにサービス ID `sample-teset` を削除します

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

すべての Bluemix プラットフォーム API キーをリストします

```
bluemix iam api-keys```

<strong>前提条件</strong>: エンドポイント、ログイン

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

新しい Bluemix プラットフォーム API キーを作成します

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>NAME (必須)</dt>
<dd>作成する API キーの名前。</dd>
<dt>-d <i>DESCRIPTION</i> (オプション)</dt>
<dd>API キーの説明</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>指定されたファイルに API キー情報を保存します。設定されていない場合、JSON コンテンツが表示されます。</dd>
</dl>

<strong>例</strong>:

API キーを作成し、ファイルに保存します

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Bluemix プラットフォーム API キーを更新します

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>NAME (必須)</dt>
<dd>更新する API キーの古い名前。</dd>
<dt>-n <i>NAME</i> (オプション)</dt>
<dd>API キーの新しい名前</dd>
<dt>-d <i>DESCRIPTION</i> (オプション)</dt>
<dd>API キーの新しい説明</dd>
</dl>

<strong>例</strong>:

API キーの説明を更新します。

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Bluemix プラットフォーム API キーを削除します

```
bluemix iam api-key-delete NAME [-f]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>NAME (必須)</dt>
<dd>削除する API キーの名前。</dd>
<dt>-f (オプション)</dt>
<dd>確認なしで削除を強制します。</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

すべてのサービス API キーをリストします

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
</dl>

<strong>例</strong>:

サービス CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` にバインドされたサービス API キーをリストします。

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

サービス API キーの詳細をリストします

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>サービス API キーの UUID を表示します</dd>
</dl>

<strong>例</strong>:

サービス CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` にバインドされたサービス API キー `sample-key` の詳細を表示します。

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

サービス API キーを作成します

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-d, --description</dt>
  <dd>API キーの説明</dd>
  <dt>-f, --file</dt>
  <dd>指定されたファイルに API キー情報を保存します。設定されていない場合、JSON コンテンツが表示されます。</dd>
</dl>

<strong>例</strong>:

サービス CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` にバインドされたサービス API キー `sample-key` を作成します。

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

サービス API キーを更新します

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-n, --name</dt>
  <dd>サービスAPI キーの新しい名前</dd>
  <dt>-d, --description</dt>
  <dd>サービス API キーの新しい説明</dd>
  <dt>-v, --version</dt>
  <dd>サービス API キーのバージョン</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに更新します</dd>
</dl>

<strong>例</strong>:

サービス API キー `sample-key` を `new-sample-key` に名前変更します

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

サービス API キーを削除します

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>確認を求めずに削除します</dd>
</dl>

<strong>例</strong>:

サービス API キー `sample-key` を削除します

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

ユーザー `name@example.com` のポリシーをリストします

```
bluemix iam user-policies name@example.com
```

<strong>前提条件</strong>:  エンドポイント、ログイン、ターゲットのアカウント

<strong>コマンド・オプション</strong>:
<dl>
<dt>USER_NAME (必須)</dt>
<dd>ポリシーが属するユーザー名</dd>
</dl>

<strong>例</strong>:

ユーザー `name@example.com` のポリシーをリストします

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

ユーザー・ポリシーの詳細を表示します

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>前提条件</strong>:  エンドポイント、ログイン、ターゲットのアカウント

<strong>コマンド・オプション</strong>:
<dl>
<dt>USER_NAME (必須)</dt>
<dd>ポリシーが属するユーザー名</dd>
<dt>POLICY_ID (必須)</dt>
<dd>ポリシーの ID</dd>
</dl>

<strong>例</strong>:

ユーザー `name@example.com` のポリシー `0bb730daa` をリストします

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

ユーザー・ポリシーを作成します

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>前提条件</strong>:  エンドポイント、ログイン、ターゲットのアカウント

<strong>コマンド・オプション</strong>:
<dl>
<dt>USER_NAME (必須)</dt>
<dd>ポリシーが属するユーザー名</dd>
<dt>-f, --file <i>FILE</i> (オプション)</dt>
<dd>ポリシー定義の JSON ファイル</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (オプション)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (オプション)</dt>
<dd>ポリシー定義のサービス名。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (オプション)</dt>
<dd>ポリシー定義のサービス・インスタンス。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--region <i>REGION</i> (オプション)</dt>
<dd>ポリシー定義の地域。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (オプション)</dt>
<dd>ポリシー定義のリソース・タイプ。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource <i>RESOURCE</i> (オプション)</dt>
<dd>ポリシー定義のリソース。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (オプション)</dt>
<dd>リソース・グループの名前。これは、「-f, --file」、「--resource」、および「--resource-group-id」の各フラグと同時に指定することはできません。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (オプション)</dt>
<dd>リソース・グループの ID。これは、「-f, --file」、「--resource」、および「--resource-group-id」の各フラグと同時に指定することはできません。</dd>
  <dd>ポリシー定義の役割名。 特定のサービスの、サポートされる役割については、「bluemix iam roles --service SERVICE_NAME」を実行してください。このオプションは、「-f, --file」と同時に指定することはできません。</dd>
</dl>

<strong>例</strong>:

ポリシー JSON ファイル `policy.json` から、ユーザー `name@example.com` のユーザー・ポリシーを作成します。

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

`name@example.com` に、すべての `sample-service` リソースの `Administrator` 役割を与えます。

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

`name@example.com` に、`us-south` 地域のサンプル・サービス・インスタンス `ServiceId-ade78e9f` のリソース `key123` の `Editor` 役割を与えます。

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

`name@example.com` に、リソース・グループ ID `dda27e49d2a1efca58083a01dfde18f6` の `Operator` 役割を与えます。

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

`name@example.com` に、 リソース・グループ `sample-resource-group` のメンバーの `Viewer` 役割を与えます。

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

`name@example.com` に、ID `dda27e49d2a1efca58083a01dfde18f6` を持つリソース・グループのメンバーの `Viewer` 役割を与えます。

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

ユーザー・ポリシーを更新します

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>前提条件</strong>:  エンドポイント、ログイン、ターゲットのアカウント

<strong>コマンド・オプション</strong>:
<dt>USER_NAME (必須)</dt>
<dd>ポリシーが属するユーザー名</dd>
<dt>POLICY_ID (必須)</dt>
<dd>更新するポリシーの ID</dd>
<dt>-v, --version <i>VERSION</i> (オプション)</dt>
<dd>既存のポリシーのバージョン</dd>
<dt>-f, --file <i>FILE</i> (オプション)</dt>
<dd>ポリシー定義の JSON ファイル</dd>
<dt>-f, --file <i>FILE</i> (オプション)</dt>
<dd>ポリシー定義の JSON ファイル</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (オプション)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (オプション)</dt>
<dd>ポリシー定義のサービス名。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (オプション)</dt>
<dd>ポリシー定義のサービス・インスタンス。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--region <i>REGION</i> (オプション)</dt>
<dd>ポリシー定義の地域。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (オプション)</dt>
<dd>ポリシー定義のリソース・タイプ。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource <i>RESOURCE</i> (オプション)</dt>
<dd>ポリシー定義のリソース。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (オプション)</dt>
<dd>リソース・グループの名前。これは、「-f, --file」、「--resource」、および「--resource-group-id」の各フラグと同時に指定することはできません。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (オプション)</dt>
<dd>リソース・グループの ID。これは、「-f, --file」、「--resource」、および「--resource-group-id」の各フラグと同時に指定することはできません。</dd>
  <dd>ポリシー定義の役割名。特定のサービスの、サポートされる役割については、「bluemix iam roles --service SERVICE_NAME」を実行してください。このオプションは、「-f, --file」と同時に指定することはできません。</dd>
</dl>

<strong>例</strong>:

JSON ファイル内のポリシーによってユーザー・ポリシーを更新します

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

`name@example.com` に、すべての `sample-service` リソースの `Administrator` 役割を与えるようにユーザー・ポリシーを更新します

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 `name@example.com` に、`us-south` 地域のサンプル・サービス・インスタンス `ServiceId-ade78e9f` のリソース `key123` の `Editor` 役割を与えるようにユーザー・ポリシーを更新します

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

`name@example.com` に、リソース・グループ ID `dda27e49d2a1efca58083a01dfde18f6` の `Operator` 役割を与えるようにユーザー・ポリシーを更新します

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

`name@example.com` に、 リソース・グループ `sample-resource-group` のメンバーの `Viewer` 役割を与えるようにユーザー・ポリシーを更新します

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

`name@example.com` に、ID `dda27e49d2a1efca58083a01dfde18f6` を持つリソース・グループのメンバーの `Viewer` 役割を与えるようにユーザー・ポリシーを更新します

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

指定したサービスのすべてのサービス・ポリシーをリストします

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>SERVICE_ID_NAME (必須)</dt>
  <dd>サービス ID の名前</dd>
  <dt>-json</dt>
  <dd>JSON フォーマットでポリシーを表示します</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずにサービス・ポリシーを表示します</dd>
</dl>

<strong>例</strong>:

サービス `test` のポリシーをリストします

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

サービス・ポリシーの詳細を表示します

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>SERVICE_ID_NAME (必須)</dt>
  <dd>サービス ID の名前</dd>
  <dt>POLICY_ID (必須)</dt>
  <dd>サービス・ポリシーの ID<dd>
  <dt>-json</dt>
  <dd>JSON フォーマットでポリシーを表示します</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずにサービス・ポリシーを表示します</dd>
</dl>

<strong>例</strong>:

サービス `test` のポリシー `140798e2-8ea7db3` を表示します

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

サービス・ポリシーを作成します

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>SERVICE_ID_NAME (必須)</dt>
  <dd>サービス ID の名前</dd>
  <dt>-f, --file</dt>
  <dd>ポリシー定義の JSON ファイル。 これは、「-r, --roles」、「--service-name」、「--service-instance」、「--region」、「--resource-type」、および「--resource」の各フラグと同時に指定することはできません。</dd>
  <dt>-r, --roles</dt>
  <dd>ポリシー定義の役割名。特定のサービスの、サポートされる役割については、「bluemix iam roles --service SERVICE_NAME」を実行してください。このオプションは、「-f, --file」と同時に指定することはできません。</dd>
  <dt>-service-name</dt>
  <dd>ポリシー定義のサービス名。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-service-instance</dt>
  <dd>ポリシー定義のサービス・インスタンス。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-region</dt>
  <dd>ポリシー定義の地域。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-resource-type</dt>
  <dd>ポリシー定義のリソース・タイプ。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-resource</dt>
  <dd>ポリシー定義のリソース。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-F, --force</dt>
  <dd>確認を求めずにサービス・ポリシーを作成します</dd>
</dl>

<strong>例</strong>:

サービス `test` のサービス・ポリシーを JSON ファイルから作成します

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

サービス・ポリシーを更新します

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>SERVICE_ID_NAME (必須)</dt>
  <dd>サービス ID の名前</dd>
  <dt>POLICY_ID (必須)</dt>
  <dd>サービス・ポリシーの ID<dd>
  <dt>-v, --version</dt>
  <dd>サービス・ポリシーのバージョン</dd>
  <dt>-f, --file</dt>
  <dd>ポリシー定義の JSON ファイル。これは、「-r, --roles」、「--service-name」、「--service-instance」、「--region」、「--resource-type」、および「--resource」の各フラグと同時に指定することはできません。</dd>
  <dt>-r, --roles</dt>
  <dd>ポリシー定義の役割名。特定のサービスの、サポートされる役割については、「bluemix iam roles --service SERVICE_NAME」を実行してください。このオプションは、「-f, --file」と同時に指定することはできません。</dd>
  <dt>-service-name</dt>
  <dd>ポリシー定義のサービス名。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-service-instance</dt>
  <dd>ポリシー定義のサービス・インスタンス。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-region</dt>
  <dd>ポリシー定義の地域。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-resource-type</dt>
  <dd>ポリシー定義のリソース・タイプ。 これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-resource</dt>
  <dd>ポリシー定義のリソース。これは、「-f, --file」フラグと同時に指定することはできません。</dd>
  <dt>-F, --force</dt>
  <dd>確認を求めずにサービス・ポリシーを更新します</dd>
</dl>

<strong>例</strong>:

サービス `test` のサービス・ポリシー `140798e2-8ea7db3` を JSON ファイルから更新します

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

サービス・ポリシーを削除します

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>SERVICE_ID_NAME (必須)</dt>
  <dd>サービス ID の名前</dd>
  <dt>POLICY_ID (必須)</dt>
  <dd>サービス・ポリシーの ID<dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに削除します</dd>
</dl>

<strong>例</strong>:

サービス `test` のポリシー `140798e2-8ea7db3` を削除します

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

リソース・グループをリストします

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>--default</dt>
  <dd>現行アカウントのデフォルト・グループを取得します</dd>
  <dt>-r, --resource</dt>
  <dd>従属リソースの ID</dd>
  <dt>-o, --resource-origin</dt>
  <dd>従属リソースの起点。 指定できる値: 「CF_ORG」、「IMS_ACCOUNT」。</dd>
</dl>

<strong>例</strong>:

現在のターゲット・アカウントのすべてのリソース・グループをリストします

```
bluemix resource groups
```

現在のターゲット・アカウントのデフォルト・グループをリストします

```
bluemix resource groups --default
```

CloudFoundry 組織のマッピングであるリソース・グループをリストします

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

リソース・グループの詳細を表示します

```
bluemix resource group NAME [--id]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>リソース・グループの名前</dd>
  <dt>--id</dt>
  <dd>ID のみを表示します</dd>
</dl>

<strong>例</strong>:

リソース・グループ `example-group` を表示します

```
bluemix resource group example-group
```

リソース・グループ `example-group` の ID のみを表示します

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

既存のリソース・グループを更新します

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>ターゲット・リソース・グループの名前</dd>
  <dt>-n, --name</dt>
  <dd>リソース・グループの新しい名前</dd>
  <dt>-q, --quota</dt>
  <dd>新規割り当て量定義の名前</dd>
  <dt>-f</dt>
  <dd>確認を求めずに更新を強制します</dd>
</dl>

<strong>例</strong>:

リソース・グループ `example-group` を `trial-group` に名前変更します

```
bluemix resource group-update example-group -n trial-group
```

リソース・グループ `example-group` の割り当て量を `free` に変更します

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

すべての割り当て量定義をリストします

```
bluemix resource quotas```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
</dl>

<strong>例</strong>:

すべての割り当て量定義をリストします

```
bluemix resource quotas```

## bluemix resource quota
{: #bluemix_resource_quota}

割り当て量定義の詳細を表示します

```
bluemix resource quota NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>割り当て量の名前</dd>
</dl>

<strong>例</strong>:
割り当て量 `free` の詳細を表示します

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

このコマンドの機能とオプションは `cf push` コマンドと同じです。


## bluemix app list
{: #bluemix_app_list}

このコマンドの機能とオプションは `cf apps` コマンドと同じです。


## bluemix app show
{: #bluemix_app_show}

このコマンドの機能とオプションは `cf app` コマンドと同じです。


## bluemix app delete
{: #bluemix_app_delete}

このコマンドの機能とオプションは `cf delete` コマンドと同じです。


## bluemix app rename
{: #bluemix_app_rename}

このコマンドの機能とオプションは `cf rename` コマンドと同じです。


## bluemix app start
{: #bluemix_app_start}

このコマンドの機能とオプションは `cf start` コマンドと同じです。


## bluemix app stop
{: #bluemix_app_stop}

このコマンドの機能とオプションは `cf stop` コマンドと同じです。


## bluemix app restart
{: #bluemix_app_restart}

このコマンドの機能とオプションは `cf restart` コマンドと同じです。


## bluemix app restage
{: #bluemix_app_restage}


このコマンドの機能とオプションは `cf restage` コマンドと同じです。


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


このコマンドの機能とオプションは `cf restart-app-instance` コマンドと同じです。


## bluemix app events
{: #bluemix_app_events}

このコマンドの機能とオプションは `cf events` コマンドと同じです。


## bluemix app files
{: #bluemix_app_files}

このコマンドの機能とオプションは `cf files` コマンドと同じです。


## bluemix app logs
{: #bluemix_app_logs}

このコマンドの機能とオプションは `cf logs` コマンドと同じです。


## bluemix app env
{: #bluemix_app_env}

このコマンドの機能とオプションは `cf env` コマンドと同じです。


## bluemix app env-set
{: #bluemix_app_env_set}

このコマンドの機能とオプションは `cf set-env` コマンドと同じです。


## bluemix app env-unset
{: #bluemix_app_env_unset}

このコマンドの機能とオプションは `cf unset-env` コマンドと同じです。


## bluemix app stacks
{: #bluemix_app_stacks}

このコマンドの機能とオプションは `cf stacks` コマンドと同じです。


## bluemix app stack-show
{: #bluemix_app_stack_show}

このコマンドの機能とオプションは `cf stack` コマンドと同じです。


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

このコマンドの機能とオプションは `cf create-app-manifest` コマンドと同じです。

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

ドメインの証明書情報をリストします。

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
<dl>
<dt>DOMAIN_NAME (必須)</dt>
<dd>証明書をホストするドメイン。</dd>
</dl>


<strong>例</strong>:

ドメイン `ibmcxo-eventconnect.com` の証明書情報を表示するには、次のように指定します。

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

現在の組織内の、指定したドメインに証明書を追加します。

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>DOMAIN (必須)</dt>
   <dd>証明書を追加するドメイン。</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i> (必須)</dt>
   <dd>秘密鍵ファイル・パス。</dd>
   <dt>-c <i>CERT_FILE</i> (必須)</dt>
   <dd>証明書ファイル・パス。</dd>
   <dt>-p <i>PASSWORD</i> (オプション)</dt>
   <dd>証明書のパスワード。</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i> (オプション)</dt>
   <dd>中間証明書ファイル・パス。</dd>
   <dt>-t <i>TRUST_STORE_FILE</i> (オプション)</dt>
   <dd>トラストストア・ファイル。</dd>
   </dl>


<strong>例</strong>:

ドメイン `ibmcxo-eventconnect.com` に証明書を追加するには、以下のように指定します。

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

現在の組織内の、指定したドメインから証明書を削除します。

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>DOMAIN (必須)</dt>
   <dd>証明書を削除するドメイン。</dd>
   <dt>-f (オプション)</dt>
   <dd>確認なしで削除を強制します。</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

このコマンドの機能とオプションは `cf domains` コマンドと同じです。


## bluemix app domain-create
{: #bluemix_app_domain_create}

このコマンドの機能とオプションは `cf create-domain` コマンドと同じです。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

このコマンドの機能とオプションは `cf delete-domain` コマンドと同じです。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

このコマンドの機能とオプションは `cf create-shared-domain` コマンドと同じです。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

このコマンドの機能とオプションは `cf delete-shared-domain` コマンドと同じです。

## bluemix app routes
{: #bluemix_app_routes}

このコマンドの機能とオプションは `cf routes` コマンドと同じです。


## bluemix app route-check
{: #bluemix_app_route_check}

このコマンドの機能とオプションは `cf check-route` コマンドと同じです。


## bluemix app route-map
{: #bluemix_app_route_map}

指定されたドメインおよびホスト名を持つ経路を既存 cf アプリケーションまたはコンテナー・グループにマップします。

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (必須)</dt>
   <dd>経路によってマップされる cf アプリケーションまたはコンテナー・
グループの名前。</dd>
   <dt>DOMAIN (必須)</dt>
   <dd>経路のドメイン。例えば、mychinabluemix.net または chinabluemix.net などです。</dd>
   <dt>-n <i>HOST_NAME</i> (オプション)</dt>
   <dd>経路のホスト名。指定されない場合、ホスト名は、デフォルトで、アプリケーション名またはコンテナー・グループ名に設定されます。</dd>
   </dl>

<strong>例</strong>:

指定されたドメインで `my-app` に経路をマップします。

```
bluemix app route-map my-app mychinabluemix.net
```

指定されたドメインとホスト名で「my-container-group」に経路をマップします。

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

指定された経路を既存 cf アプリケーションまたはコンテナー・グループからマップ解除します。

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (必須)</dt>
   <dd>cf アプリケーションまたはコンテナー・グループの名前。</dd>
   <dt>DOMAIN (必須)</dt>
   <dd>経路のドメイン (例えば、mychinabluemix.net または chinabluemix.net)。</dd>
   <dt>-n <i>HOST_NAME</i> (オプション)</dt>
   <dd>経路のホスト名。指定されない場合、ホスト名は、デフォルトで、アプリケーション名またはコンテナー・グループ名に設定されます。</dd>
   </dl>

<strong>例</strong>:

`my-app.mychinabluemix.net` を `my-app` からマップ解除するには、以下のように指定します。

```
bluemix app route-unmap my-app mychianbluemix.net
```

`abc.chinabluexmix.net` を `my-container-group` からマップ解除するには、以下のように指定します。

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

このコマンドの機能とオプションは `cf create-route` コマンドと同じです。


## bluemix app route-delete
{: #bluemix_app_route_delete}

このコマンドの機能とオプションは `cf delete-route` コマンドと同じです。


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

このコマンドの機能とオプションは `cf delete-orphaned-routes` コマンドと同じです。


## bluemix app domains
{: #bluemix_app_domains}

このコマンドの機能とオプションは `cf domains` コマンドと同じです。


## bluemix app domain-create
{: #bluemix_app_domain_create}

このコマンドの機能とオプションは `cf create-domain` コマンドと同じです。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

このコマンドの機能とオプションは `cf delete-domain` コマンドと同じです。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

このコマンドの機能とオプションは `cf create-shared-domain` コマンドと同じです。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

このコマンドの機能とオプションは `cf delete-shared-domain` コマンドと同じです。


## bluemix service offerings
{: #bluemix_service_offerings}


このコマンドの機能とオプションは `cf marketplace` コマンドと同じです。


## bluemix service list
{: #bluemix_service_list}

このコマンドの機能とオプションは `cf services` コマンドと同じです。


## bluemix service show
{: #bluemix_service_show}

このコマンドの機能とオプションは `cf service` コマンドと同じです。


## bluemix service create
{: #bluemix_service_create}

このコマンドの機能とオプションは `cf create-service` コマンドと同じです。


## bluemix service update
{: #bluemix_service_update}

このコマンドの機能とオプションは `cf update-service` コマンドと同じです。


## bluemix service delete
{: #bluemix_service_delete}

このコマンドの機能とオプションは `cf delete-service` コマンドと同じです。


## bluemix service rename
{: #bluemix_service_rename}

このコマンドの機能とオプションは `cf rename-service` コマンドと同じです。


## bluemix service bind
{: #bluemix_service_bind}

このコマンドの機能とオプションは `cf bind-service` コマンドと同じです。


## bluemix service unbind
{: #bluemix_service_unbind}

このコマンドの機能とオプションは `cf unbind-service` コマンドと同じです。


## bluemix service key-create
{: #bluemix_service_key_create}

このコマンドの機能とオプションは `cf create-service-key` コマンドと同じです。


## bluemix service key-delete
{: #bluemix_service_key_delete}

このコマンドの機能とオプションは `cf delete-service-key` コマンドと同じです。


## bluemix service keys
{: #bluemix_service_keys}

このコマンドの機能とオプションは `cf service-keys` コマンドと同じです。


## bluemix service key-show
{: #bluemix_service_key_show}

このコマンドの機能とオプションは `cf service-key` コマンドと同じです。


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

このコマンドの機能とオプションは `cf create-user-provided-service` コマンドと同じです。


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

このコマンドの機能とオプションは `cf update-user-provided-service` コマンドと同じです。


## bluemix resource instances
{: #bluemix_resource_instances}

リソース・インスタンスをリストします

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>--resource-name</dt>
  <dd>従属リソースの名前</dd>
  <dt>-r, --region</dt>
  <dd>地域 ID を基準にフィルター操作します。未指定の場合、デフォルトは現行地域です。「-r, --region all」はすべての地域のリソース・インスタンスを表示します</dd>
  <dt>--long</dt>
  <dd>出力に追加フィールドを表示します</dd>
</dl>

<strong>例</strong>:

リソース `test-resource` のリソース・インスタンスをリストします。

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

リソース・インスタンスの詳細を表示します

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>リソース・インスタンスの名前</dd>
  <dt>-r, --region</dt>
  <dd>地域 ID を基準にフィルター操作します。未指定の場合、デフォルトは現行地域です。「-r, --region all」はすべての地域のリソース・インスタンスを表示します</dd>
  <dt>--id</dt>
  <dd>リソース・インスタンスの ID を表示します</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` の詳細を表示します

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

リソース・インスタンスを作成します

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME (必須)</dt>
  <dd>リソース・インスタンスの名前</dd>
  <dt>RESOURCE_NAME または RESOURCE_ID (必須)</dt>
  <dd>リソースの名前または ID</dd>
  <dt>RESOURCE_PLAN_NAME または RESOURCE_PLAN_ID (必須)</dt>
  <dd>リソース・プランの名前または ID</dd>
  <dt>-r, --region</dt>
  <dd>リソース・インスタンスを作成する地域。未指定の場合、デフォルトは現行地域です。</dd>
  <dt>-t, --tags</dt>
  <dd>タグ</dd>
  <dt>-p, --parameters</dt>
  <dd>リソース・インスタンスを作成するパラメーターの JSON ファイルまたは JSON 文字列</dd>
</dl>

<strong>例</strong>:
リソース `test-resource` のリソース・プラン `test-resource-plan` を使用して、`my-resource-instance` という名前のリソース・インスタンスを作成します

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

リソース・インスタンスを更新します

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>RESOURCE_INSTANCE_NAME (必須)</dt>
  <dd>リソース・インスタンスの名前</dd>
  <dt>-n, --name</dt>
  <dd>新規リソース・インスタンス名</dd>
  <dt>-t, --tags</dt>
  <dd>新規タグ</dd>
  <dt>--resource-plan-id</dt>
  <dd>新規リソース・プラン ID</dd>
  <dt>--update-time</dt>
  <dd>有料の記録が有効になってからの時間 (秒)</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに更新を強制します</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` を更新し、その名前を `new-resource-instance` に変更します

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

リソース・インスタンスを削除します

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>確認なしで削除を強制します</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` を削除します

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

リソース別名へのバインディングを表示します

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>RESOURCE_ALIAS (必須)</dt>
  <dd>リソース別名</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` へのリソース・バインディングを表示します

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

リソース・バインディングの詳細を表示します

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>ALIAS_NAME (必須)</dt>
  <dd>リソース別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry アプリケーション名</dd>
  <dt>--id</dt>
  <dd>ID のみを表示します。このリソース・バインディングの他の出力はすべて抑制されます。</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` とアプリ `my-app` の間のリソース・バインディングの詳細を表示します

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

リソース・バインディングを作成します

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (必須)</dt>
  <dd>リソース別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry アプリケーション名</dd>
  <dt>ROLE_NAME</dt>
  <dd>ユーザー役割の名前</dd>
  <dt>--service-id-name</dt>
  <dd>役割が属しているサービス ID の名前</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに作成を強制します</dd>
</dl>

<strong>例</strong>:
`Administrator` の役割によってリソース別名 `my-resource-alias` とアプリ `my-app` の間のリソース・バインディングを作成します

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

リソース・バインディングを削除します

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (必須)</dt>
  <dd>リソース別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry アプリケーション名</dd>
  <dt>-f, --force</dt>
  <dd>確認なしで削除を強制します</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` とアプリ `my-app` の間のリソース・バインディングを削除します

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

リソース・インスタンスまたはリソース別名のリソース・キーをリストします

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>リソース・インスタンス ID</dd>
  <dt>--instance-name</dt>
  <dd>リソース・インスタンス名</dd>
  <dt>--alias-id</dt>
  <dd>リソース別名 ID</dd>
  <dt>--alias-name</dt>
  <dd>リソース別名</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` のリソース・キーをリストします

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

リソース・キーの詳細を表示します

```
bluemix resource key KEY_NAME [--id]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>キーの名前</dd>
  <dt>--id</dt>
  <dd>リソース・キーの ID を表示します</dd>
</dl>

<strong>例</strong>:
リソース・キー `my-resource-key` の詳細を表示します

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

リソース・キーを作成します

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>NAME</dt>
  <dd>キーの名前</dd>
  <dt>ROLE_NAME</dt>
  <dd>ユーザー役割の名前</dd>
  <dt>--instance-id</dt>
  <dd>リソース・インスタンス ID</dd>
  <dt>--instance-name</dt>
  <dd>リソース・インスタンス名</dd>
  <dt>--alias-id</dt>
  <dd>リソース別名 ID</dd>
  <dt>--alias-name</dt>
  <dd>リソース別名</dd>
  <dt>-service-id-name</dt>
  <dd>役割が属しているサービス ID の名前</dd>
  <dt>-f, --force</dt>
  <dd>確認を求めずに作成を強制します</dd>
</dl>

<strong>例</strong>:
役割 `Administrator` を使用して、リソース・インスタンス `my-resource-instance` に対して `my-resource-key` という名前のリソース・キーを作成します。

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

リソース・キーを削除します

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>キーの名前</dd>
  <dt>-f, --force</dt>
  <dd>確認なしで削除を強制します</dd>
</dl>

<strong>例</strong>:
リソース・キー `my-resource-key` を削除します

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

リソース・インスタンスの別名をリストします

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>従属リソース・インスタンスの ID</dd>
  <dt>--instance-name</dt>
  <dd>従属リソース・インスタンスの名前</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` のリソース別名をリストします
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

リソース別名の詳細を表示します

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>ALIAS_NAME (必須)</dt>
  <dd>リソース別名の名前</dd>
  <dt>--id</dt>
  <dd>指定されたリソース別名の ID のみを表示してください。 この別名の他の出力はすべて抑制されます。</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` の詳細を表示します
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

リソース・インスタンスの別名を作成します

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>ALIAS_NAME (必須)</dt>
  <dd>リソース別名の名前</dd>
  <dt>--instance-id</dt>
  <dd>従属リソース・インスタンスの ID</dd>
  <dt>--instance-name</dt>
  <dd>従属リソース・インスタンスの名前</dd>
  <dt>-s</dt>
  <dd>別名が作成されるスペースの名前。 デフォルトは現行のスペースです。</dd>
  <dt>-t, --tags</dt>
  <dd>タグのリスト。</dd>
  <dt>-p, --parameters</dt>
  <dd>パラメーター JSON ファイルまたは JSON 文字列。</dd>
</dl>

<strong>例</strong>:
リソース・インスタンス `my-resource-instance` の、`my-resource-alias` という名前のリソース別名を作成します
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

リソース別名を更新します

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>ALIAS_NAME (必須)</dt>
  <dd>リソース別名の名前</dd>
  <dt>-n, --name</dt>
  <dd>リソース別名の新しい名前。</dd>
  <dt>-t, --tags</dt>
  <dd>タグのリスト。</dd>
  <dt>-p, --parameters</dt>
  <dd>パラメーター JSON ファイルまたは JSON 文字列。</dd>
  <dt>-f, --force</dt>
  <dd>ユーザーの確認を求めずに更新を強制します。</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` を更新し、その名前を `new-resource-alias` に変更します

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

リソースの別名を削除します

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>ALIAS_NAME (必須)</dt>
  <dd>リソース別名の名前</dd>
  <dt>-f, --force</dt>
  <dd>確認なしで削除を強制します</dd>
</dl>

<strong>例</strong>:
リソース別名 `my-resource-alias` を削除します

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

カタログ項目を検索します

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-q, --query</dt>
  <dd>キーワードを検索します</dd>
  <dt>-r, --region</dt>
  <dd>検索範囲の地理的地域を指定します。現在は、「us-south」と「united-kingdom」のみがサポートされています。</dd>
  <dt>-k, --kind</dt>
  <dd>リソースの種類を基準にしてフィルター操作します。現在は、「service-cf」、「iaas」、「runtime」、「template」、および「dashboard」のみがサポートされています。</dd>
  <dt>-p, --price</dt>
  <dd>価格を基準にしてフィルター操作します。現在は、「free」、「paygo」、「bluemix-subscription」のみがサポートされています。</dd>
  <dt>-t, --tag</dt>
  <dd>タグを基準にしてフィルター操作します。</dd>
  <dt>-sort-by</dt>
  <dd>ソート基準のプロパティー</dd>
  <dt>-reverse</dt>
  <dd>ソート順序を反転するかどうか</dd>
  <dt>-json</dt>
  <dd>元の JSON 応答を出力します</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

サービス `Automation test` を検索します

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

カタログ項目を取得します

```
bluemix catalog entry [-i ID] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>カタログ項目の ID。</dd>
  <dt>-children</dt>
  <dd>カタログ項目のすべての子を取得します</dd>
  <dt>-json</dt>
  <dd>元の JSON 応答を出力します</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

ID `a0ef1-d3b4j0` の項目を取得します

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
新しいカタログ項目を作成します (アカウントのカタログ管理者のみ)

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-p, --parent</dt>
  <dd>オブジェクトの親 ID</dd>
  <dt>-c</dt>
  <dd>インラインまたはファイルのいずれかで提供される、カタログ固有の構成パラメーターを含む有効な JSON オブジェクト。サポートされている構成パラメーターのリストについては、特定のカタログ項目用の資料を参照してください。</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

親 ID `a0ef1-d3b4j0` を持つ JSON ファイルからリソースを作成します

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
既存のカタログ項目を更新します (アカウントのカタログ管理者またはエディターのみ)

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>更新するカタログ項目の ID。</dd>
  <dt>-c</dt>
  <dd>インラインまたはファイルのいずれかで提供される、カタログ固有の構成パラメーターを含む有効な JSON オブジェクト。サポートされている構成パラメーターのリストについては、特定のカタログ項目用の資料を参照してください。</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

JSON ファイルからリソース `j402-dnf1i` を更新します

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
カタログ項目の可視性を取得します (アカウントのカタログ管理者のみ)

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>カタログ項目の ID。</dd>
  <dt>-json</dt>
  <dd>元の JSON 応答を出力します</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

グローバル・スコープでリソース `j402-dnf1i` の可視性を取得します

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
既存のカタログ項目の可視性を更新します (アカウントのカタログ管理者のみ)

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>更新するカタログ項目の ID。</dd>
  <dt>-c</dt>
  <dd>インラインまたはファイルのいずれかで提供される、カタログ固有の構成パラメーターを含む有効な JSON オブジェクト。サポートされている構成パラメーターのリストについては、特定のカタログ項目用の資料を参照してください。</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

JSON ファイルからリソース `j402-dnf1i` の可視性を設定します

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
マーケットプレイス内のサービス・オファリングをリストします

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
<dl>
  <dt>-cf</dt>
  <dd>Cloud Foundry サービスのみを表示します</dd>
  <dt>-rc</dt>
  <dd>RC と互換性のあるサービスのみを表示します</dd>
  <dt>-global</dt>
  <dd>グローバル・スコープで操作します</dd>
</dl>

<strong>例</strong>:

グローバル・スコープでのサービス・オファリングを表示します

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

Bluemix のボイラープレート・テンプレートを表示します。

```
bluemix catalog templates [-d]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>-d (オプション)</dt>
   <dd><i>-d</i> オプションが指定されている場合、各テンプレートの説明
も表示されます。それ以外の場合、各テンプレートの ID および名前のみが表示されます。</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

指定されたボイラープレート・テンプレートの詳細情報を表示します。

```
bluemix catalog template TEMPLATE_ID
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>TEMPLATE_ID (必須)</dt>
   <dd>ボイラープレート・テンプレートの ID。すべてのテンプレートの ID を表示するには、
<i>bluemix templates</i> を使用します。</dd>
   </dl>


<strong>例</strong>:

テンプレート `mobileBackendStarter` の詳細を表示します。

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

指定されたテンプレートをベースにした、指定された URL と説明を持つ cf アプリケーションを作成します。デフォルトでは、この新規アプリケーションは自動的に開始されます。

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>前提条件</strong>: エンドポイント、ログイン、ターゲット

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>TEMPLATE_ID (必須)</dt>
   <dd>アプリケーションの作成時にそのアプリケーションの基盤とするテンプレート。すべてのテンプレートの ID を表示するには、<i>bluemix templates</i> を使用します。</dd>
   <dt>CF_APP_NAME (必須)</dt>
   <dd>作成される cf アプリケーションの名前。</dd>
   <dt>-u <i>URL</i> (オプション)</dt>
   <dd>アプリケーションの経路。指定しない場合、経路はアプリ名とデフォルト・ドメインに基づき、Bluemix が自動的に設定します。</dd>
   <dt>-d <i>DESCRIPTION</i> (オプション)</dt>
   <dd>アプリケーションの説明。</dd>
   <dt>--no-start (オプション)</dt>
   <dd>作成後のアプリケーションを自動的に開始しません。
指定されない場合、アプリケーションは作成された後で自動的に開始されます。</dd>
   </dl>


<strong>例</strong>:

`javaHelloWorld` テンプレートをベースにして cf アプリケーション `my-app` を作成します。

```
bluemix catalog template-run javaHelloWorld my-app
```

`rubyHelloWorld` テンプレートに基づき、経路 `myrubyapp.chinabluemix.net` と説明 `My first ruby app on {{site.data.keyword.Bluemix_notm}}.` を使用してアプリケーション `my-ruby-app` を作成するには、以下のように指定します。

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

`pythonHelloWorld` テンプレートをベースにして、自動開始なしでアプリケーション `my-python-app` を作成します。

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

アカウントの月次使用量とコストを表示します。

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

<dl>
  <dt>-d MONTH_DATE (オプション)</dt>
  <dd>YYYY-MM 形式を使用して指定する日付のデータを表示します。指定されていない場合、今月の使用量が表示されます。</dd>
  <dt>--json (オプション)</dt>
  <dd>使用量の結果を JSON 形式で表示します。</dd>
</dl>

<strong>例</strong>:

2016 年 6 月のマイ・アカウントの使用量とコストのレポートを表示します。

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

組織の月次使用量の詳細を表示します。この操作は、組織の請求管理者のみ実行できます。

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

<dl>
  <dt>ORG_NAME (必須)</dt>
  <dd>組織の名前。</dd>
  <dt>-d MONTH_DATE (オプション)</dt>
  <dd>YYYY-MM 形式を使用して指定された日付のデータを表示します。指定されていない場合、今月の使用量が表示されます。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>組織をホストする地域の名前。「all」に設定されている場合、すべての地域の組織の使用量が表示されます。</dd>
  <dt>--json (オプション)</dt>
  <dd>使用量の結果を JSON 形式で表示します。</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

マイ・アカウント内の組織の月次使用量サマリーを表示します。

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>前提条件</strong>: エンドポイント、ログイン

<strong>コマンド・オプション</strong>:

<dl>
  <dt>-d MONTH_DATE (オプション)</dt>
  <dd>YYYY-MM 形式を使用して指定された日付のデータを表示します。指定されていない場合、今月の使用量が表示されます。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>組織をホストする地域の名前。「all」に設定されている場合、すべての地域の組織の使用量サマリーが表示されます。</dd>
  <dt>--json (オプション)</dt>
  <dd>使用量の結果を JSON 形式で表示します。</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

{{site.data.keyword.Bluemix_notm}} CLI に登録されているすべてのプラグイン・リポジトリーをリストします。

```
bluemix plugin repos
```

<strong>前提条件</strong>: なし


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

新規プラグイン・リポジトリーを {{site.data.keyword.Bluemix_notm}} CLI に追加します。

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>REPO_NAME (必須)</dt>
   <dd>追加するリポジトリーの名前。各リポジトリーに対して任意の名前を定義できます。</dd>
   <dt>REPO_URL (必須)</dt>
   <dd>追加するリポジトリーの URL。リポジトリー URL にはプロトコルが含まれている必要があります (例えば、plugins.ng.bluemix.net ではなく、http://plugins.ng.bluemix.net)。http://plugins.ng.bluemix.net は、Bluemix CLI の公式プラグイン・リポジトリーです。</dd>
    </dl>


<strong>例</strong>:

Bluemix CLI の公式プラグイン・リポジトリーを `bluemix-repo` として追加します。

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

{{site.data.keyword.Bluemix_notm}} CLI からプラグイン・リポジトリーを削除します。

```
bluemix plugin repo-remove REPO_NAME
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
   <dl>
   <dt>REPO_NAME (必須)</dt>
   <dd>削除するリポジトリーの名前。</dd>
   </dl>

<strong>例</strong>:

{{site.data.keyword.Bluemix_notm}} CLI から `bluemix-repo` リポジトリーを削除します。

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

追加されたすべてのリポジトリーまたは特定のリポジトリー内にある使用可能なプラグインをすべてリストします。

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (オプション)</dt>
   <dd>指定されたリポジトリー内のプラグインのみをリストします。</dd>
   </dl>

<strong>例</strong>:

追加されたすべてのリポジトリー内のすべてのプラグインをリストします。

```
bluemix plugin repo-plugins
```

`bluemix-repo` リポジトリー内のすべてのプラグインをリストします。

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

リポジトリー内のプラグインの詳細を表示します。

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (オプション)</dt>
   <dd>リポジトリーの名前。リポジトリーが指定されない場合、コマンドは、デフォルトのプラグイン・リポジトリーを使用します</dd>
   </dl>

<strong>例</strong>:

リポジトリー「sample-repo」内のプラグイン「IBM-Containers」の詳細をリストします

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

デフォルト・リポジトリー内のプラグイン「IBM-Containers」の詳細をリストします

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

{{site.data.keyword.Bluemix_notm}} CLI 内のインストールされたプラグインをすべてリストします。

```
bluemix plugin list
```

<strong>前提条件</strong>: なし

## bluemix plugin show
{: #bluemix_plugin_show}

インストールされたプラグインの詳細を表示します

```
bluemix plugin show PLUGIN-NAME
```

<strong>前提条件</strong>: なし


## bluemix plugin install
{: #bluemix_plugin_install}

指定したパスまたはリポジトリーから、特定のバージョンのプラグインを {{site.data.keyword.Bluemix_notm}} CLI にインストールします。

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME (必須)</dt>
   <dd>「-r <i>REPO_NAME</i>」が指定されない場合、指定されたローカル
・パスまたはリモート URL からプラグインがインストールされます。</dd>
   <dt>-r <i>REPO_NAME</i> (オプション)</dt>
   <dd>プラグインのバイナリーが配置されているリポジトリーの名前。リポジトリーが指定されない場合、コマンドは、デフォルトのプラグイン・リポジトリーを使用します。</dd>
   <dt>-v <i>VERSION</i> (オプション)</dt>
   <dd>インストールするプラグインのバージョン。指定されていない場合は、最新バージョンのプラグインがインストールされます。このオプションは、リポジトリーからプラグインをインストールする場合にのみ有効です。</dd>
    </dl>

<strong>例</strong>:

ローカル・ファイルからプラグインをインストールします。

```
bluemix plugin install /downloads/new_plugin
```

リモート URL からプラグインをインストールします。

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

最新バージョンの `IBM-Containers` プラグインを `bluemix-repo` リポジトリーからインストールするには、以下のように指定します。

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
バージョン `0.5.800` の `IBM-Containers` プラグインを `bluemix-repo` リポジトリーからインストールするには、以下のように指定します。

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

リポジトリーからプラグインをアップグレードします

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>更新するプラグインの名前。指定されない場合、コマンドは、インストールされているすべてのプラグインのアップグレードを確認します。</dd>
 <dt>-r REPO_NAME</dt>
 <dd>プラグインのバイナリーが配置されているリポジトリーの名前。指定されない場合、コマンドは、デフォルトのプラグイン・リポジトリーを使用します。</dd>
 <dt>-v <i>VERSION</i> (オプション)</dt>
 <dd>更新するプラグインのバージョン。表示されない場合、プラグインを入手可能な最新バージョンに更新してください。</dd>
 <dt>--all</dt>
 <dd>利用可能なすべてのプラグインを更新します</dd>
</dl>

<strong>例</strong>:

プラグイン・リポジトリー「My-Repo」で使用可能なすべてのアップグレードを確認します。

```
bluemix plugin update -r My-Repo
```

リポジトリー「My-Repo」内のプラグイン「plugin-echo」を最新にアップグレードします。

```
bluemix plugin update -r My-Repo plugin-echo
```

リポジトリー「My-Repo」内のプラグイン「plugin-echo」をバージョン「1.0.1」に更新します。

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

指定されたプラグインを {{site.data.keyword.Bluemix_notm}} CLI からアンインストールします。

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>前提条件</strong>: なし

<strong>コマンド・オプション</strong>:

   <dl>
   <dt>PLUGIN_NAME (必須)</dt>
   <dd>アンインストールされるプラグインの名前。</dd>
    </dl>

<strong>例</strong>:

前にインストールされた `IBM-Containers` プラグインをアンインストールします。

```
bluemix plugin uninstall IBM-Containers
```

