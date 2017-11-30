---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.Bluemix_notm}} (bx) 指令
{: #bluemix_cli}

版本：0.6.1

{{site.data.keyword.Bluemix_notm}} 指令行介面 (CLI) 提供一組依名稱空間分組的指令，讓使用者與 {{site.data.keyword.Bluemix_notm}} 互動。 

從 0.5.0 版開始，{{site.data.keyword.Bluemix_notm}} 指令行用戶端已將 Cloud Foundry 指令行用戶端搭載在其安裝中。如果您已安裝自己的 cf cli，請不要在相同環境定義中使用自己的安裝的 {{site.data.keyword.Bluemix_notm}} CLI 指令 `bx [command]` 及 Cloud Foundry CLI 指令 `cf [command]`。如果您要使用 cf cli 來管理 {{site.data.keyword.Bluemix_notm}} CLI 環境定義中的 Cloud Foundry 資源，請改為使用 `bluemix cf [command]`。此外，不容許 `bluemix cf api/login/logout/target`，請改為使用 `bluemix api/login/logout/target`。

以下列出 {{site.data.keyword.Bluemix_notm}} CLI 所支援的詳細指令用法，包括其名稱、引數、選項、必要條件、說明及範例。
{:shortdesc}

**附註：***必要條件* 列出使用指令之前需要哪些動作。沒有必要動作的指令會列為**無**。否則，必要條件可能包括下列一個以上的動作：

<dl>
<dt>端點</dt>
<dd>必須透過 <code>bluemix api</code> 設定 API 端點後，才能使用這個指令。</dd>
<dt>登入</dt>
<dd>需要使用 <code>bluemix login</code> 指令進行登入後，才能使用這個指令。如果是使用聯合 ID 登入，請使用 '--sso' 選項以一次性密碼進行鑑別，或使用 '--apikey' 以 API 金鑰進行鑑別。移至 {{site.data.keyword.Bluemix_notm}} 主控台**管理** &gt; **安全** &gt; **Bluemix API 金鑰**，以建立 API 金鑰。
</dd>
<dt>目標</dt>
<dd>必須使用 <code>bluemix target</code> 指令來設定組織及空間後，才能使用這個指令。</dd>
<dt>Docker</dt>
<dd>必須先安裝 Docker CLI (docker)，才能執行這個指令。</dd>
</dl>

**附註：**您可以使用短格式的 bluemix 指令；例如，`bx api` 為 `bluemix api` 的短格式。

請使用下表中的索引來參照常用的 bluemix 指令。

## 一般 bluemix 指令 
{: #bx_commands_index}

<table summary="一般 bluemix 指令。">
 <caption>表 1. 一般 bluemix 指令</caption>
 <thead>
 <th colspan="5">一般 bluemix 指令</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix help](bx_cli.html#bluemix_help)</td>
 <td>[bluemix api](bx_cli.html#bluemix_api)</td>
 <td>[bluemix config](bx_cli.html#bluemix_config)</td>
 <td>[bluemix info](bx_cli.html#bluemix_info)</td>
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
 
 ## 用來管理及配置 {{site.data.keyword.BluSoftlayer_notm}} 服務的指令
  {: #bx_commands_softlayer}
  
用來管理 {{site.data.keyword.BluSoftlayer_notm}} 的指令已合併至 Bluemix CLI。如需使用 Bluemix CLI 配置及管理 {{site.data.keyword.BluSoftlayer_notm}} 服務的相關資訊，請參閱：[Bluemix CLI {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) 指令](/docs/cli/reference/softlayer/index.md#softlayer_cli)。
 
 ## 用來管理帳戶、組織及角色的指令
 {: #bx_commands_account}

<table summary="您可以用來管理帳戶、組織、空間及角色的 bluemix 指令。">
<caption>表 2. 用來管理帳戶、組織、空間及角色的指令</caption>
 <thead>
 <th colspan="5">用來管理帳戶、組織、空間及角色的指令</th>
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


 ## 用來管理資源群組及資源的指令
{: #bx_commands_resource}

<table summary="您可以用來管理資源群組及資源的 bluemix 指令。">
  <caption>表 3. 用來管理資源群組及資源的指令</caption>
  <thead>
    <th colspan="5">用來管理資源群組及資源的指令</th>
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

 
 ## 用來管理 API 金鑰及原則的指令
 {: #bx_commands_iam}
 <table summary="您可以用來管理 API 金鑰及原則的 bluemix 指令。">
 <caption>表 3. 用來管理 API 金鑰及原則的指令</caption>
  <thead>
  <th colspan="5">用來管理 API 金鑰及原則的指令</th>
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
 
 ## 用來管理 cf 應用程式及應用程式相關網域、路徑和憑證的指令
 {: #bx_commands_apps}

<table summary="您可以用來管理 cf 應用程式及應用程式相關網域、路徑和憑證的 bluemix 指令。">
<caption>表 4. 用來管理 cf 應用程式及應用程式相關網域、路徑和憑證的指令</caption>
 <thead>
 <th colspan="5">用來管理 cf 應用程式及應用程式相關網域、路徑和憑證的指令</th>
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
 
 ## 用來管理 Bluemix 服務的指令
 {: #bx_commands_services}

<table summary="您可以用來管理 Bluemix 服務的 bluemix 指令。">
 <caption>表 5. 用來管理 Bluemix 服務的指令</caption>
 <thead>
 <th colspan="5">用來管理 Bluemix 服務的指令</th>
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

 
 ## 用來管理型錄、外掛程式及帳單設定的指令
 {: #bx_commands_settings}

<table summary="您可以用來管理 Bluemix 型錄、外掛程式、帳單和安全設定的 bluemix 指令。">
 <caption>表 6. 用來管理 Bluemix 型錄、外掛程式、帳單和安全設定的指令</caption>
 <thead>
 <th colspan="5">用來管理 Bluemix 型錄、外掛程式、帳單和安全設定的指令</th>
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
顯示 {{site.data.keyword.Bluemix_notm}} CLI 之第一層內建指令及所支援名稱空間的一般說明，或特定內建指令或名稱空間的說明。

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>COMMAND|NAMESPACE（選用）</dt>
   <dd>顯示其說明的指令或名稱空間。如果未指定，則會顯示 {{site.data.keyword.Bluemix_notm}} CLI 的一般說明。</dd>
   </dl>



<strong>範例</strong>：

顯示 {{site.data.keyword.Bluemix_notm}} CLI 的一般說明：

```
bluemix help
```

顯示 `info` 指令的說明：

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
設定或檢視 {{site.data.keyword.Bluemix_notm}} API 端點。

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
   <dl>
   <dt>API_ENDPOINT（選用）</dt>
   <dd>設為目標的 API 端點，例如 `https://api.chinabluemix.net`。 如果未同時指定 *API_ENDPOINT* 及 `--unset` 選項，則會顯示現行 API 端點。</dd>
   <dt>--unset（選用）</dt>
   <dd>移除 API 端點設定。</dd>
   <dt>--skip-ssl-validation（選用）</dt>
   <dd>略過 HTTP 要求的 SSL 驗證。</dd>
   </dl>
<strong>範例</strong>：將 API 端點設為 api.chinabluemix.net：

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

檢視現行 API 端點：

```
bluemix api
```

取消設定 API 端點：

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


將預設值寫入配置檔。

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>用於 HTTP 要求的逾時值。預設值為 60 秒。</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>追蹤對終端機或指定檔案的 HTTP 要求。</dd>
   <dt>--color true|false</dt>
   <dd>啟用或停用彩色輸出。依預設，會啟用彩色輸出。</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>設定預設語言環境。如果 LOCALE 為 <i>CLEAR</i>，則會刪除先前的語言環境。</dd>
   <dt>--check-version true|false</dt>
   <dd>啟用或停用 CLI 版本檢查。</dd>
   </dl>

一次只能指定其中一個選項。

<strong>範例</strong>：

將 HTTP 要求逾時值設為 30 秒：

```
bluemix config --http-timeout 30
```

啟用 HTTP 要求的追蹤輸出：

```
bluemix config --trace true
```

追蹤對指定檔案 */home/usera/my_trace* 的 HTTP 要求：

```
bluemix config --trace /home/usera/my_trace
```

停用彩色輸出：

```
bluemix config --color false
```

將語言環境設為 zh_Hans：

```
bluemix config --locale zh_Hans
```

清除語言環境設定：

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

檢視基本 {{site.data.keyword.Bluemix_notm}} 資訊，包括現行地區、雲端控制器版本以及部分有用端點（例如用於登入及交換存取記號的端點）。

```
bluemix info
```

<strong>必要條件</strong>：端點


## bluemix cf
{: #bluemix_cf}

呼叫內嵌的 CF CLI

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
<dl>
  <dt>-q, --quiet</dt>
  <dd>關閉「呼叫 cf 指令...」訊息</dd>
</dl>

<strong>範例</strong>：

列出 cf 應用程式：

```
bluemix cf apps
```

列出 cf 服務，但沒有「呼叫 cf 指令...」訊息：

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

登入使用者。 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>必要條件</strong>：無

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>指令選項</strong>：
<dl>
  <dt> -a <i>API_ENDPOINT</i>（選用）</dt>
  <dd> API 端點（例如：api.ng.bluemix.net）</dd>
  <dt> --apikey <i>API_KEY 或 @API_KEY_FILE_PATH</i>
  <dd> API 金鑰內容，或透過 @ 指出的 API 金鑰檔案的路徑</dd>
  <dt> --sso（選用）</dt>
  <dd> 使用一次性密碼進行登入</dd>
  <dt> -u <i>USERNAME</i>（選用）</dt>
  <dd> 使用者名稱</dd>
  <dt> -p <i>PASSWORD</i>（選用）</dt>
  <dd> 密碼</dd>
  <dt> -c <i>ACCOUNT_ID</i>（選用）</dt>
  <dd> 目標帳戶的 ID</dd>
  <dt> -o <i>ORG_NAME</i>（選用）</dt>
  <dd> 目標組織的名稱</dd>
  <dt> -s <i>SPACE_NAME</i>（選用）</dt>
  <dd> 目標空間的名稱</dd>
  <dt> --skip-ssl-validation（選用）</dt>
  <dd> 略過 HTTP 要求的 SSL 驗證。不建議使用這個選項。</dd>
</dl>

<strong>範例</strong>：

#### 互動式登入

```
bluemix login
```

以使用者名稱及密碼登入，並設定目標帳戶、組織及空間：

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

以一次性密碼登入，並設定目標帳戶、組織及空間：

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

以 API 金鑰登入，並設定目標：

#### API 金鑰具有關聯的帳戶

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### API 金鑰沒有關聯的帳戶

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>附註：</strong>如果 API 金鑰具有關聯的帳戶，則不容許切換至另一個帳戶。

#### 使用一次性密碼

```
bluemix login -u UserID --sso
```

CLI 接著會提供 URL 鏈結，並要求密碼：
```
一次性密碼（從 https://URL_Link_To_Obtain_Passcode 取得）：
```

在瀏覽器中開啟鏈結，這會引導您取得密碼。在主控台中鍵入給定的密碼，您應該就可以登入。

## bluemix logout
{: #bluemix_logout}

登出使用者。

```
bluemix logout
```

<strong>必要條件</strong>：無

## bluemix regions
{: #bluemix_regions}

檢視 {{site.data.keyword.Bluemix_notm}} 上所有地區的資訊。

```
bluemix regions
```

<strong>必要條件</strong>：端點


## bluemix target
{: #bluemix_target}


設定或檢視目標帳戶、地區、組織或空間。

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>-r <i>REGION_NAME</i>（選用）</dt>
   <dd>要切換至的地區名稱，例如 'us-south' 或 'eu-gb'。</dd>
   <dt>-c <i>ACCOUNT_ID</i>（選用）</dt>
   <dd>要設為目標的帳戶 ID。</dd>
   <dt>--cf</dt>
   <dd>以互動方式選取目標組織及空間</dd>
   <dt>-o <i>ORG_NAME</i>（選用）</dt>
   <dd>要設為目標的組織名稱。</dd>
   <dt>-s <i>SPACE_NAME</i>（選用）</dt>
   <dd>要設為目標的空間名稱。</dd>
   </dl>
如果未指定選項，則會顯示現行帳戶、地區、組織及空間。

<strong>範例</strong>：

設定現行帳戶、組織及空間：

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

切換至新的地區：

```
bluemix target -r eu-gb
```

檢視現行帳戶、地區、組織及空間：

```
bluemix target
```

### bluemix update
{: #bluemix_update}

將 CLI 更新為最新版本。

```
bluemix update
```

<strong>必要條件</strong>：無

### bluemix account orgs
{: #bluemix_account_orgs}

列出所有組織

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>-r <i>REGION</i>（選用）</dt>
   <dd>顯示其組織資訊的地區。如果設為 'all'，則會列出所有地區中的所有組織。</dd>
   <dt>--guid（選用）</dt>
   <dd>顯示組織的 GUID。</dd>
   </dl>

<strong>範例</strong>：

列出 `us-south` 地區中的所有組織，並顯示 GUID

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

顯示所指定組織的資訊。

```
bluemix account org ORG_NAME [--guid]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>ORG_NAME（必要）</dt>
   <dd>組織的名稱。</dd>
   <dt>--guid（選用）</dt>
   <dd>顯示組織的 GUID。</dd>
   </dl>

<strong>範例</strong>：

顯示 `IBM` 組織的資訊，並顯示 GUID

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

建立新的組織。只有帳戶擁有者才能執行此作業。

```
bluemix account org-create ORG_NAME
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>ORG_NAME（必要）</dt>
   <dd>所要建立之組織的名稱。</dd>
   </dl>

<strong>範例</strong>：

建立名稱為 `IBM` 的組織。

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

將組織從現行地區抄寫到另一個地區。

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>ORG_NAME（必要）</dt>
   <dd>要抄寫之現有組織的名稱。</dd>
   <dt>REGION_NAME（必要）</dt>
   <dd>管理所抄寫組織的地區名稱。</dd>
   </dl>

<strong>範例</strong>：

將組織 `myorg` 抄寫到地區 `eu-gb`：

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

重新命名組織。只有組織管理員才能執行此作業。

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>OLD_ORG_NAME（必要）</dt>
   <dd>要重新命名之組織的舊名稱。</dd>
   <dt>NEW_ORG_NAME（必要）</dt>
   <dd>組織重新命名後的新名稱。</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

這個指令的功能及選項與 `cf spaces` 指令相同。


## bluemix account space
{: #bluemix_account_space}

這個指令的功能及選項與 `cf space` 指令相同。


## bluemix account space-create
{: #bluemix_account_space_create}

這個指令的功能及選項與 `cf create-space` 指令相同。


## bluemix account space-rename
{: #bluemix_account_space_rename}


這個指令的功能及選項與 `cf rename-space` 指令相同。


## bluemix account space-delete
{: #bluemix_account_space_delete}


這個指令的功能及選項與 `cf delete-space` 指令相同。

## bluemix account org-users
{: #bluemix_account_org_users}

依角色顯示指定組織中的使用者。

```
bluemix account org-users ORG_NAME [-a]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>ORG_NAME（必要）</dt>
<dd>組織的名稱。</dd>
<dt>-a（選用）</dt>
<dd>列出指定組織中的所有使用者，而不依角色分組。</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

將使用者新增至組織（需要組織管理員）。

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

從組織移除使用者（僅限組織管理員或使用者自己）

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>指令選項</strong>：
<dl>
<dt>--force, -f</dt>
<dd>強制刪除，而不確認。</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

取得現行使用者的所有組織角色

```
bluemix account org-roles
```

<strong>必要條件</strong>：端點、登入

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

將組織角色指派給使用者。只有組織管理員才能執行此作業。

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
  <dl>
   <dt>USER_NAME（必要）</dt>
   <dd>所指派之使用者的名稱。</dd>
   <dt>ORG_NAME（必要）</dt>
   <dd>獲指派此使用者之組織的名稱。</dd>
   <dt>ORG_ROLE（必要）</dt>
   <dd>獲指派此使用者之組織角色的名稱。例如：
   <ul>
   <li>OrgManager：此角色可以邀請和管理使用者、選取和變更方案，以及設定消費限制。</li>
   <li>BillingManager：此角色可以建立和管理計費帳戶及付款資訊。</li>
   <li>OrgAuditor：此角色具有組織資訊和報告的唯讀權。</li>
   </ul>
   </dd>
  </dl>

<strong>範例</strong>：

以 `OrgManager` 角色，將使用者 `Mary` 指派給組織 `IBM`：

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**附註**：您可以使用 CLI 設定組織/空間角色，但如果您要設定其他許可權，則必須利用使用者介面。如需進一步詳細資料，請參閱[指派使用者存取權](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)。<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

移除使用者的組織角色。只有組織管理員才能執行此作業。

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>USER_NAME（必要）</dt>
   <dd>所要移除之使用者的名稱。</dd>
   <dt>ORG_NAME（必要）</dt>
   <dd>從中移除此使用者之組織的名稱。</dd>
   <dt>ORG_ROLE（必要）</dt>
   <dd>從中移除此使用者之組織角色的名稱。例如：
   <ul>
   <li>OrgManager：此角色可以邀請和管理使用者、選取和變更方案，以及設定消費限制。</li>
   <li>BillingManager：此角色可以建立和管理計費帳戶及付款資訊。</li>
   <li>OrgAuditor：此角色具有組織資訊和報告的唯讀權。</li>
   </ul>
   </dd>
    </dl>

<strong>範例</strong>：

以 `OrgManager` 角色，從組織 `IBM` 移除使用者 `Mary`：

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

依角色顯示指定空間中的使用者。

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>ORG_NAME（必要）</dt>
   <dd>組織的名稱。</dd>
   <dt>SPACE_NAME（必要）</dt>
   <dd>空間的名稱。</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

將空間角色指派給使用者。只有空間管理員才能執行此作業。

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

   <dl>
   <dt>USER_NAME（必要）</dt>
   <dd>所指派之使用者的名稱。</dd>
   <dt>ORG_NAME（必要）</dt>
   <dd>獲指派此使用者之組織的名稱。</dd>
   <dt>SPACE_NAME（必要）</dt>
   <dd>獲指派此使用者之空間的名稱。</dd>
   <dt>SPACE_ROLE（必要）</dt>
   <dd>獲指派此使用者之空間角色的名稱。例如：
   <ul>
   <li>SpaceManager：此角色可以邀請和管理使用者，以及啟用給定空間的特性。</li>
   <li>SpaceDeveloper：此角色可以建立和管理應用程式及服務，以及查看日誌和報告。</li>
   <li>SpaceAuditor：此角色可以檢視空間的日誌、報告和設定。</li>
   </ul></dd>
    </dl>

<strong>範例</strong>：

以 `SpaceManager` 角色，將使用者 `Mary` 指派給組織 `IBM` 及空間 `Cloud`：

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

移除使用者的空間角色。只有空間管理員才能執行此作業。

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

   <dl>
   <dt>USER_NAME（必要）</dt>
   <dd>所要移除之使用者的名稱。</dd>
   <dt>ORG_NAME（必要）</dt>
   <dd>從中移除此使用者之組織的名稱。</dd>
   <dt>SPACE_NAME（必要）</dt>
   <dd>從中移除此使用者之空間的名稱。</dd>
   <dt>SPACE_ROLE（必要）</dt>
   <dd>從中移除此使用者之空間角色的名稱。例如：
   <ul>
   <li>SpaceManager：此角色可以邀請和管理使用者，以及啟用給定空間的特性。</li>
   <li>SpaceDeveloper：此角色可以建立和管理應用程式及服務，以及查看日誌和報告。</li>
   <li>SpaceAuditor：此角色可以檢視空間的日誌、報告和設定。</li>
   </ul></dd>
    </dl>


<strong>範例</strong>：

以 `SpaceManager` 角色，從組織 `IBM` 及空間 `Cloud` 移除使用者 `Mary`：

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

列出現行使用者的所有帳戶

```
bluemix account list
```

<strong>必要條件</strong>：端點、登入


## bluemix account org-account
{: #bluemix_account_org_account}

顯示所指定組織的帳戶（需要組織使用者）

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
  <dt>--guid（選用）</dt>
  <dd>僅顯示帳戶 ID</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

顯示與帳戶相關聯的使用者。只有帳戶擁有者才能執行此作業。

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

從現行帳戶刪除使用者（僅限帳戶擁有者）

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>USERNAME（必要）</dt>
<dd>使用者名稱</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>帳戶 ID。如果未指定，則預設為現行帳戶。</dd>
<dt>--force, -f（選用）</dt>
<dd>強制刪除，而不確認。</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

邀請使用者加入已設定組織和空間角色的帳戶。只有帳戶擁有者才能執行此作業。

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
   <dt>USER_NAME（必要）</dt>
   <dd>所邀請之使用者的名稱。</dd>
   <dt>ORG_NAME（必要）</dt>
   <dd>邀請此使用者加入之組織的名稱。</dd>
   <dt>ORG_ROLE（必要）</dt>
   <dd>邀請此使用者加入之組織角色的名稱。例如：
   <ul>
  <li>OrgManager：此角色可以邀請和管理使用者、選取和變更方案，以及設定消費限制。</li>
  <li>BillingManager：此角色可以建立和管理計費帳戶及付款資訊。</li>
  <li>OrgAuditor：此角色具有組織資訊和報告的唯讀權。</li>
  </ul> </dd>
   <dt>SPACE_NAME（必要）</dt>
   <dd>邀請此使用者加入之空間的名稱。</dd>
   <dt>SPACE_ROLE（必要）</dt>
   <dd>邀請此使用者加入之空間的名稱。邀請此使用者加入之空間角色的名稱。例如：
   <ul>
<li>SpaceManager：此角色可以邀請和管理使用者，以及啟用給定空間的特性。</li>
<li>SpaceDeveloper：此角色可以建立和管理應用程式及服務，以及查看日誌和報告。</li>
<li>SpaceAuditor：此角色可以檢視空間的日誌、報告和設定。</li>
</ul>
</dd>
</dl>

<strong>範例</strong>：

以 `OrgManager` 角色，邀請使用者 `Mary` 加入組織 `IBM`，以及以 `SpaceAuditor` 角色加入空間 `Cloud`：

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**附註**：您可以使用 CLI 在邀請期間設定組織/空間角色，但如果您要設定其他許可權，則必須利用使用者介面。如需進一步詳細資料，請參閱[指派使用者存取權](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)。<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

將邀請重新傳送給使用者（需要組織管理員或帳戶擁有者）

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

列出所有服務 ID

```
bluemix iam service-ids --uuid
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-uuid</dt>
  <dd>僅顯示服務 ID 的 UUID</dd>
</dl>

<strong>範例</strong>：列出現行帳戶下所有服務 ID 的 UUID：

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

顯示服務 ID 的詳細資料

```
bluemix iam service-id NAME [--uuid]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>服務的名稱</dd>
  <dt>-uuid</dt>
  <dd>顯示服務 ID 的 UUID</dd>
</dl>

<strong>範例</strong>：

顯示服務 ID `sample-test` 的詳細資料

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

建立服務 ID

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>服務的名稱</dd>
  <dt>-d, --description</dt>
  <dd>服務 ID 的說明</dd>
</dl>

<strong>範例</strong>：

建立服務名稱為 `sample-test` 且說明為 `hello, world!` 的服務 ID

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
更新服務 ID

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>服務的名稱</dd>
  <dt>-n, --name</dt>
  <dd>服務的新名稱</dd>
  <dt>-d, --description</dt>
  <dd>服務的新說明</dd>
  <dt>-v, --version</dt>
  <dd>服務 ID 的版本</dd>
  <dt>-f, --force</dt>
  <dd>更新而不進行確認</dd>
</dl>

<strong>範例</strong>：

將服務 ID `sample-test` 重新命名為 `sample-test-2`，而不進行確認

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

更新服務 `sample-test` 版本 `1-0jn39fbefew` 的說明

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

刪除服務 ID

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>服務的名稱</dd>
  <dt>-f, --force</dt>
  <dd>刪除而不進行確認</dd>
</dl>

<strong>範例</strong>：

刪除服務 ID `sample-teset`，而不進行確認

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

列出所有 Bluemix 平台 API 金鑰

```
bluemix iam api-keys
```

<strong>必要條件</strong>：端點、登入

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

建立新的 Bluemix 平台 API 金鑰

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>NAME（必要）</dt>
<dd>要建立之 API 金鑰的名稱。</dd>
<dt>-d <i>DESCRIPTION</i>（選用）</dt>
<dd>API 金鑰的說明</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>將 API 金鑰資訊儲存至指定的檔案。如果未設定，則會顯示 JSON 內容。</dd>
</dl>

<strong>範例</strong>：

建立 API 金鑰，並儲存至檔案

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

更新 Bluemix 平台 API 金鑰

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>NAME（必要）</dt>
<dd>要更新之 API 金鑰的舊名稱。</dd>
<dt>-n <i>NAME</i>（選用）</dt>
<dd>API 金鑰的新名稱</dd>
<dt>-d <i>DESCRIPTION</i>（選用）</dt>
<dd>API 金鑰的新說明</dd>
</dl>

<strong>範例</strong>：

更新 API 金鑰的說明：

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

刪除 Bluemix 平台 API 金鑰

```
bluemix iam api-key-delete NAME [-f]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>NAME（必要）</dt>
<dd>要刪除之 API 金鑰的名稱。</dd>
<dt>-f（選用）</dt>
<dd>強制刪除，而不確認。</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

列出所有服務 API 金鑰

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
</dl>

<strong>範例</strong>：

列出連結至服務 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 的服務 API 金鑰：

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

列出服務 API 金鑰的詳細資料

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-uuid</dt>
  <dd>顯示服務 API 金鑰的 UUID</dd>
</dl>

<strong>範例</strong>：

顯示連結至服務 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 之服務 API 金鑰 `sample-key` 的詳細資料：

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

建立服務 API 金鑰

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-d, --description</dt>
  <dd>API 金鑰的說明</dd>
  <dt>-f, --file</dt>
  <dd>將 API 金鑰資訊儲存至指定的檔案。如果未設定，則會顯示 JSON 內容。</dd>
</dl>

<strong>範例</strong>：

建立連結至服務 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 的服務 API 金鑰 `sample-key`：

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

更新服務 API 金鑰

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-n, --name</dt>
  <dd>服務 API 金鑰的新名稱</dd>
  <dt>-d, --description</dt>
  <dd>服務 API 金鑰的新說明</dd>
  <dt>-v, --version</dt>
  <dd>服務 API 金鑰的版本</dd>
  <dt>-f, --force</dt>
  <dd>更新而不進行確認</dd>
</dl>

<strong>範例</strong>：

將服務 API 金鑰 `sample-key` 重新命名為 `new-sample-key`：

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

刪除服務 API 金鑰

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-f, --force</dt>
  <dd>刪除而不進行確認</dd>
</dl>

<strong>範例</strong>：

刪除服務 API 金鑰 `sample-key`：

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

列出使用者 `name@example.com` 的原則：

```
bluemix iam user-policies name@example.com
```

<strong>必要條件</strong>：端點、登入、設為目標的帳戶

<strong>指令選項</strong>：
<dl>
<dt>USER_NAME（必要）</dt>
<dd>原則所屬的使用者名稱</dd>
</dl>

<strong>範例</strong>：

列出使用者 `name@example.com` 的原則：

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

顯示使用者原則的詳細資料

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>必要條件</strong>：端點、登入、設為目標的帳戶

<strong>指令選項</strong>：
<dl>
<dt>USER_NAME（必要）</dt>
<dd>原則所屬的使用者名稱</dd>
<dt>POLICY_ID（必要）</dt>
<dd>原則的 ID</dd>
</dl>

<strong>範例</strong>：

列出使用者 `name@example.com` 的原則 `0bb730daa`：

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

建立使用者原則

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>必要條件</strong>：端點、登入、設為目標的帳戶

<strong>指令選項</strong>：
<dl>
<dt>USER_NAME（必要）</dt>
<dd>原則所屬的使用者名稱</dd>
<dt>-f, --file <i>FILE</i>（選用）</dt>
<dd>原則定義的 JSON 檔案</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i>（選用）</dt>
<dt>--service-name <i>SERVICE_NAME</i>（選用）</dt>
<dd>原則定義的服務名稱。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i>（選用）</dt>
<dd>原則定義的服務實例。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--region <i>REGION</i>（選用）</dt>
<dd>原則定義的地區。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i>（選用）</dt>
<dd>原則定義的資源類型。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource <i>RESOURCE</i>（選用）</dt>
<dd>原則定義的資源。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i>（選用）</dt>
<dd>資源群組的名稱。這與 '-f, --file'、'--resource' 及 '--resource-group-id' 旗標不能同時使用。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i>（選用）</dt>
<dd>資源群組的 ID。這與 '-f, --file'、'--resource' 及 '--resource-group-name' 旗標不能同時使用。</dd>
  <dd>原則定義的角色名稱。針對特定服務所支援的角色，執行 'bluemix iam roles --service SERVICE_NAME'。此選項與 '-f, --file' 不能同時使用。</dd>
</dl>

<strong>範例</strong>：

從原則 JSON 檔案 `policy.json`，建立使用者 `name@example.com` 的使用者原則：

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

針對所有 `sample-service` 資源，將 `Administrator` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

針對 `us-south` 地區中範例服務實例 `ServiceId-ade78e9f` 的資源 `key123`，將 `Editor` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

針對 ID 為 `dda27e49d2a1efca58083a01dfde18f6` 的資源群組，將 `Operator` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

針對資源群組 `sample-resource-group` 的成員，將 `Viewer` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

針對 ID 為 `dda27e49d2a1efca58083a01dfde18f6` 之資源群組的成員，將 `Viewer` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

更新使用者原則

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>必要條件</strong>：端點、登入、設為目標的帳戶

<strong>指令選項</strong>：
<dt>USER_NAME（必要）</dt>
<dd>原則所屬的使用者名稱</dd>
<dt>POLICY_ID（必要）</dt>
<dd>要更新之原則的 ID</dd>
<dt>-v, --version <i>VERSION</i>（選用）</dt>
<dd>現有原則的版本</dd>
<dt>-f, --file <i>FILE</i>（選用）</dt>
<dd>原則定義的 JSON 檔案</dd>
<dt>-f, --file <i>FILE</i>（選用）</dt>
<dd>原則定義的 JSON 檔案</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i>（選用）</dt>
<dt>--service-name <i>SERVICE_NAME</i>（選用）</dt>
<dd>原則定義的服務名稱。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i>（選用）</dt>
<dd>原則定義的服務實例。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--region <i>REGION</i>（選用）</dt>
<dd>原則定義的地區。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i>（選用）</dt>
<dd>原則定義的資源類型。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource <i>RESOURCE</i>（選用）</dt>
<dd>原則定義的資源。這與 '-f, --file' 旗標不能同時使用。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i>（選用）</dt>
<dd>資源群組的名稱。這與 '-f, --file'、'--resource' 及 '--resource-group-id' 旗標不能同時使用。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i>（選用）</dt>
<dd>資源群組的 ID。這與 '-f, --file'、'--resource' 及 '--resource-group-name' 旗標不能同時使用。</dd>
  <dd>原則定義的角色名稱。針對特定服務所支援的角色，執行 'bluemix iam roles --service SERVICE_NAME'。此選項與 '-f, --file' 不能同時使用。</dd>
</dl>

<strong>範例</strong>：

將使用者原則更新為 JSON 檔案中的使用者原則：

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

更新使用者原則，以針對所有 `sample-service` 資源，將 `Administrator` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 更新使用者原則，以針對 `us-south` 地區中範例服務實例 `ServiceId-ade78e9f` 的資源 `key123`，將 `Editor` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

更新使用者原則，以針對 ID 為 `dda27e49d2a1efca58083a01dfde18f6` 的資源群組，將 `Operator` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

更新使用者原則，以針對資源群組 `sample-resource-group` 的成員，將 `Viewer` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

更新使用者原則，以針對 ID 為 `dda27e49d2a1efca58083a01dfde18f6` 之資源群組的成員，將 `Viewer` 角色授與給 `name@example.com`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

列出指定服務的所有服務原則

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必要）</dt>
  <dd>服務 ID 的名稱</dd>
  <dt>-json</dt>
  <dd>以 JSON 格式顯示原則</dd>
  <dt>-f, --force</dt>
  <dd>顯示服務原則而不進行確認</dd>
</dl>

<strong>範例</strong>：

列出服務 `test` 的原則：

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

顯示服務原則的詳細資料

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必要）</dt>
  <dd>服務 ID 的名稱</dd>
  <dt>POLICY_ID（必要）</dt>
  <dd>服務原則的 ID<dd>
  <dt>-json</dt>
  <dd>以 JSON 格式顯示原則</dd>
  <dt>-f, --force</dt>
  <dd>顯示服務原則而不進行確認</dd>
</dl>

<strong>範例</strong>：

顯示服務 `test` 的原則 `140798e2-8ea7db3`：

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

建立服務原則

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必要）</dt>
  <dd>服務 ID 的名稱</dd>
  <dt>-f, --file</dt>
  <dd>原則定義的 JSON 檔案。這與 '-r, --roles'、'--service-name'、'--service-instance'、'--region'、'--resource-type' 及 '--resource' 旗標不能同時使用。</dd>
  <dt>-r, --roles</dt>
  <dd>原則定義的角色名稱。針對特定服務所支援的角色，執行 'bluemix iam roles --service SERVICE_NAME'。此選項與 '-f, --file' 不能同時使用。</dd>
  <dt>-service-name</dt>
  <dd>原則定義的服務名稱。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-service-instance</dt>
  <dd>原則定義的服務實例。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-region</dt>
  <dd>原則定義的地區。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-resource-type</dt>
  <dd>原則定義的資源類型。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-resource</dt>
  <dd>原則定義的資源。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-F, --force</dt>
  <dd>建立服務原則而不進行確認</dd>
</dl>

<strong>範例</strong>：

從 JSON 檔案，建立服務 `test` 的服務原則：

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

更新服務原則

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必要）</dt>
  <dd>服務 ID 的名稱</dd>
  <dt>POLICY_ID（必要）</dt>
  <dd>服務原則的 ID<dd>
  <dt>-v, --version</dt>
  <dd>服務原則的版本</dd>
  <dt>-f, --file</dt>
  <dd>原則定義的 JSON 檔案。這與 '-r, --roles'、'--service-name'、'--service-instance'、'--region'、'--resource-type' 及 '--resource' 旗標不能同時使用。</dd>
  <dt>-r, --roles</dt>
  <dd>原則定義的角色名稱。針對特定服務所支援的角色，執行 'bluemix iam roles --service SERVICE_NAME'。此選項與 '-f, --file' 不能同時使用。</dd>
  <dt>-service-name</dt>
  <dd>原則定義的服務名稱。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-service-instance</dt>
  <dd>原則定義的服務實例。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-region</dt>
  <dd>原則定義的地區。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-resource-type</dt>
  <dd>原則定義的資源類型。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-resource</dt>
  <dd>原則定義的資源。這與 '-f, --file' 旗標不能同時使用。</dd>
  <dt>-F, --force</dt>
  <dd>更新服務原則而不進行確認</dd>
</dl>

<strong>範例</strong>：

從 JSON 檔案，更新服務 `test` 的服務原則 `140798e2-8ea7db3`：

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

刪除服務原則

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必要）</dt>
  <dd>服務 ID 的名稱</dd>
  <dt>POLICY_ID（必要）</dt>
  <dd>服務原則的 ID<dd>
  <dt>-f, --force</dt>
  <dd>刪除而不進行確認</dd>
</dl>

<strong>範例</strong>：

刪除測試 `test` 的原則 `140798e2-8ea7db3`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

列出資源群組

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>--default</dt>
  <dd>取得現行帳戶的預設群組</dd>
  <dt>-r, --resource</dt>
  <dd>隸屬資源的 ID</dd>
  <dt>-o, --resource-origin</dt>
  <dd>隸屬資源的出處。接受值：'CF_ORG'、'IMS_ACCOUNT'。</dd>
</dl>

<strong>範例</strong>：

列出目前設為目標的帳戶下的所有資源群組：

```
bluemix resource groups
```

列出目前設為目標的帳戶的預設群組：

```
bluemix resource groups --default
```

列出其為 CloudFoundry 組織之對映的資源群組

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

顯示資源群組的詳細資料

```
bluemix resource group NAME [--id]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>資源群組的名稱</dd>
  <dt>--id</dt>
  <dd>僅顯示 ID</dd>
</dl>

<strong>範例</strong>：

顯示資源群組 `example-group`：

```
bluemix resource group example-group
```

僅顯示資源群組 `example-group` 的 ID：

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

更新現有資源群組

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>目標資源群組的名稱</dd>
  <dt>-n, --name</dt>
  <dd>資源群組的新名稱</dd>
  <dt>-q, --quota</dt>
  <dd>新配額定義的名稱</dd>
  <dt>-f</dt>
  <dd>強制更新，而不進行確認</dd>
</dl>

<strong>範例</strong>：

將資源群組 `example-group` 重新命名為 `trial-group`：

```
bluemix resource group-update example-group -n trial-group
```

將資源群組 `example-group` 的配額變更為 `free`：

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

列出所有配額定義

```
bluemix resource quotas
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
</dl>

<strong>範例</strong>：

列出所有配額定義：

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

顯示配額定義的詳細資料

```
bluemix resource quota NAME
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>配額名稱</dd>
</dl>

<strong>範例</strong>：顯示配額 `free` 的詳細資料：

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

這個指令的功能及選項與 `cf push` 指令相同。


## bluemix app list
{: #bluemix_app_list}

這個指令的功能及選項與 `cf apps` 指令相同。


## bluemix app show
{: #bluemix_app_show}

這個指令的功能及選項與 `cf app` 指令相同。


## bluemix app delete
{: #bluemix_app_delete}

這個指令的功能及選項與 `cf delete` 指令相同。


## bluemix app rename
{: #bluemix_app_rename}

這個指令的功能及選項與 `cf rename` 指令相同。


## bluemix app start
{: #bluemix_app_start}

這個指令的功能及選項與 `cf start` 指令相同。


## bluemix app stop
{: #bluemix_app_stop}

這個指令的功能及選項與 `cf stop` 指令相同。


## bluemix app restart
{: #bluemix_app_restart}

這個指令的功能及選項與 `cf restart` 指令相同。


## bluemix app restage
{: #bluemix_app_restage}


這個指令的功能及選項與 `cf restage` 指令相同。


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


這個指令的功能及選項與 `cf restart-app-instance` 指令相同。


## bluemix app events
{: #bluemix_app_events}

這個指令的功能及選項與 `cf events` 指令相同。


## bluemix app files
{: #bluemix_app_files}

這個指令的功能及選項與 `cf files` 指令相同。


## bluemix app logs
{: #bluemix_app_logs}

這個指令的功能及選項與 `cf logs` 指令相同。


## bluemix app env
{: #bluemix_app_env}

這個指令的功能及選項與 `cf env` 指令相同。


## bluemix app env-set
{: #bluemix_app_env_set}

這個指令的功能及選項與 `cf set-env` 指令相同。


## bluemix app env-unset
{: #bluemix_app_env_unset}

這個指令的功能及選項與 `cf unset-env` 指令相同。


## bluemix app stacks
{: #bluemix_app_stacks}

這個指令的功能及選項與 `cf stacks` 指令相同。


## bluemix app stack-show
{: #bluemix_app_stack_show}

這個指令的功能及選項與 `cf stack` 指令相同。


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

這個指令的功能及選項與 `cf create-app-manifest` 指令相同。

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

列出網域的憑證資訊。

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
<dl>
<dt>DOMAIN_NAME（必要）</dt>
<dd>管理憑證的網域。</dd>
</dl>


<strong>範例</strong>：

檢視網域 `ibmcxo-eventconnect.com` 的憑證資訊：

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

將憑證新增到現行組織中的指定網域。

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
   <dl>
   <dt>DOMAIN（必要）</dt>
   <dd>要新增憑證的網域。</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i>（必要）</dt>
   <dd>私密金鑰檔案路徑。</dd>
   <dt>-c <i>CERT_FILE</i>（必要）</dt>
   <dd>憑證檔案路徑。</dd>
   <dt>-p <i>PASSWORD</i>（選用）</dt>
   <dd>憑證的密碼。</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i>（選用）</dt>
   <dd>中繼憑證檔案路徑。</dd>
   <dt>-t <i>TRUST_STORE_FILE</i>（選用）</dt>
   <dd>信任儲存庫檔案。</dd>
   </dl>


<strong>範例</strong>：

將憑證新增到網域 `ibmcxo-eventconnect.com`：

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

從現行組織中的指定網域移除憑證。

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：

   <dl>
   <dt>DOMAIN（必要）</dt>
   <dd>要從中移除憑證的網域。</dd>
   <dt>-f（選用）</dt>
   <dd>強制刪除，而不確認。</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

這個指令的功能及選項與 `cf domains` 指令相同。


## bluemix app domain-create
{: #bluemix_app_domain_create}

這個指令的功能及選項與 `cf create-domain` 指令相同。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

這個指令的功能及選項與 `cf delete-domain` 指令相同。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

這個指令的功能及選項與 `cf create-shared-domain` 指令相同。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

這個指令的功能及選項與 `cf delete-shared-domain` 指令相同。

## bluemix app routes
{: #bluemix_app_routes}

這個指令的功能及選項與 `cf routes` 指令相同。


## bluemix app route-check
{: #bluemix_app_route_check}

這個指令的功能及選項與 `cf check-route` 指令相同。


## bluemix app route-map
{: #bluemix_app_route_map}

將路徑對映到具有所指定網域及主機名稱的現有 cf 應用程式或容器群組。

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME（必要）</dt>
   <dd>要與路徑對映之 cf 應用程式或容器群組的名稱。</dd>
   <dt>DOMAIN（必要）</dt>
   <dd>路徑的網域。例如，mychinabluemix.net 或 chinabluemix.net。</dd>
   <dt>-n <i>HOST_NAME</i>（選用）</dt>
   <dd>路徑的主機名稱。如果未提供，則依預設會將主機名稱設為應用程式名稱或容器群組名稱。</dd>
   </dl>

<strong>範例</strong>：

將路徑對映到具有指定網域的 `my-app`：

```
bluemix app route-map my-app mychinabluemix.net
```

將路徑對映到具有指定網域及主機名稱的 'my-container-group'：

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

從現有的 cf 應用程式或容器群組中取消對映指定的路徑。

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME（必要）</dt>
   <dd>cf 應用程式或容器群組的名稱。</dd>
   <dt>DOMAIN（必要）</dt>
   <dd>路徑的網域（例如 mychinabluemix.net 或 chinabluemix.net）。</dd>
   <dt>-n <i>HOST_NAME</i>（選用）</dt>
   <dd>路徑的主機名稱。如果未提供，則依預設會將主機名稱設為應用程式名稱或容器群組名稱。</dd>
   </dl>

<strong>範例</strong>：

從 `my-app` 取消對映 `my-app.mychinabluemix.net`：

```
bluemix app route-unmap my-app mychianbluemix.net
```

從 `my-container-group` 取消對映 `abc.chinabluexmix.net`：

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

這個指令的功能及選項與 `cf create-route` 指令相同。


## bluemix app route-delete
{: #bluemix_app_route_delete}

這個指令的功能及選項與 `cf delete-route` 指令相同。


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

這個指令的功能及選項與 `cf delete-orphaned-routes` 指令相同。


## bluemix app domains
{: #bluemix_app_domains}

這個指令的功能及選項與 `cf domains` 指令相同。


## bluemix app domain-create
{: #bluemix_app_domain_create}

這個指令的功能及選項與 `cf create-domain` 指令相同。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

這個指令的功能及選項與 `cf delete-domain` 指令相同。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

這個指令的功能及選項與 `cf create-shared-domain` 指令相同。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

這個指令的功能及選項與 `cf delete-shared-domain` 指令相同。


## bluemix service offerings
{: #bluemix_service_offerings}


這個指令的功能及選項與 `cf marketplace` 指令相同。


## bluemix service list
{: #bluemix_service_list}

這個指令的功能及選項與 `cf services` 指令相同。


## bluemix service show
{: #bluemix_service_show}

這個指令的功能及選項與 `cf service` 指令相同。


## bluemix service create
{: #bluemix_service_create}

這個指令的功能及選項與 `cf create-service` 指令相同。


## bluemix service update
{: #bluemix_service_update}

這個指令的功能及選項與 `cf update-service` 指令相同。


## bluemix service delete
{: #bluemix_service_delete}

這個指令的功能及選項與 `cf delete-service` 指令相同。


## bluemix service rename
{: #bluemix_service_rename}

這個指令的功能及選項與 `cf rename-service` 指令相同。


## bluemix service bind
{: #bluemix_service_bind}

這個指令的功能及選項與 `cf bind-service` 指令相同。


## bluemix service unbind
{: #bluemix_service_unbind}

這個指令的功能及選項與 `cf unbind-service` 指令相同。


## bluemix service key-create
{: #bluemix_service_key_create}

這個指令的功能及選項與 `cf create-service-key` 指令相同。


## bluemix service key-delete
{: #bluemix_service_key_delete}

這個指令的功能及選項與 `cf delete-service-key` 指令相同。


## bluemix service keys
{: #bluemix_service_keys}

這個指令的功能及選項與 `cf service-keys` 指令相同。


## bluemix service key-show
{: #bluemix_service_key_show}

這個指令的功能及選項與 `cf service-key` 指令相同。


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

這個指令的功能及選項與 `cf create-user-provided-service` 指令相同。


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

這個指令的功能及選項與 `cf update-user-provided-service` 指令相同。


## bluemix resource instances
{: #bluemix_resource_instances}

列出資源實例

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>--resource-name</dt>
  <dd>隸屬資源的名稱</dd>
  <dt>-r, --region</dt>
  <dd>依「地區 ID」進行過濾，如果未指定，預設為現行地區，'-r, --region all' 則顯示所有地區下的資源實例</dd>
  <dt>--long</dt>
  <dd>顯示輸出中的其他欄位</dd>
</dl>

<strong>範例</strong>：

列出資源 `test-resource` 的資源實例：

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

顯示資源實例的詳細資料

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>資源實例的名稱</dd>
  <dt>-r, --region</dt>
  <dd>依「地區 ID」進行過濾，如果未指定，預設為現行地區，'-r, --region all' 則顯示所有地區下的資源實例</dd>
  <dt>--id</dt>
  <dd>顯示資源實例的 ID</dd>
</dl>

<strong>範例</strong>：顯示資源實例 `my-resource-instance` 的詳細資料：

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

建立資源實例

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME（必要）</dt>
  <dd>資源實例的名稱</dd>
  <dt>RESOURCE_NAME 或 RESOURCE_ID（必要）</dt>
  <dd>資源的名稱或 ID</dd>
  <dt>RESOURCE_PLAN_NAME 或 RESOURCE_PLAN_ID（必要）</dt>
  <dd>資源方案的名稱或 ID</dd>
  <dt>-r, --region</dt>
  <dd>要建立資源實例的地區，如果未指定，則預設為現行地區</dd>
  <dt>-t, --tags</dt>
  <dd>標籤</dd>
  <dt>-p, --parameters</dt>
  <dd>要建立資源實例之參數的 JSON 檔案或 JSON 字串</dd>
</dl>

<strong>範例</strong>：使用資源 `test-resource` 的資源方案 `test-resource-plan`，建立名為 `my-resource-instance` 的資源實例：

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

更新資源實例

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>RESOURCE_INSTANCE_NAME（必要）</dt>
  <dd>資源實例的名稱</dd>
  <dt>-n, --name</dt>
  <dd>新的資源實例名稱</dd>
  <dt>-t, --tags</dt>
  <dd>新標籤</dd>
  <dt>--resource-plan-id</dt>
  <dd>新的資源方案 ID</dd>
  <dt>--update-time</dt>
  <dd>自新紀元後付費記錄應該生效的時間（以秒為單位）</dd>
  <dt>-f, --force</dt>
  <dd>強制更新，而不進行確認</dd>
</dl>

<strong>範例</strong>：更新資源實例 `my-resource-instance`，並將其名稱變更為 `new-resource-instance`：

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

刪除資源實例

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-f, --force</dt>
  <dd>強制刪除，而不進行確認</dd>
</dl>

<strong>範例</strong>：刪除資源實例 `my-resource-instance`：

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

顯示與資源別名的連結

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>RESOURCE_ALIAS（必要）</dt>
  <dd>資源別名</dd>
</dl>

<strong>範例</strong>：顯示與資源別名 `my-resource-alias` 的資源連結：

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

顯示資源連結的詳細資料

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>ALIAS_NAME（必要）</dt>
  <dd>資源別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 應用程式名稱</dd>
  <dt>--id</dt>
  <dd>僅顯示 ID。會抑制資源連結的所有其他輸出。</dd>
</dl>

<strong>範例</strong>：顯示資源別名 `my-resource-alias` 與應用程式 `my-app` 之間資源連結的詳細資料：

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

建立資源連結

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>RESOURCE_ALIAS_NAME（必要）</dt>
  <dd>資源別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 應用程式名稱</dd>
  <dt>ROLE_NAME</dt>
  <dd>使用者角色的名稱</dd>
  <dt>--service-id-name</dt>
  <dd>角色所屬服務 ID 的名稱</dd>
  <dt>-f, --force</dt>
  <dd>強制建立，而不進行確認</dd>
</dl>

<strong>範例</strong>：以 `Administrator` 角色，建立資源別名 `my-resource-alias` 與應用程式 `my-app` 之間的資源連結：

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

刪除資源連結

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
<dl>
  <dt>RESOURCE_ALIAS_NAME（必要）</dt>
  <dd>資源別名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 應用程式名稱</dd>
  <dt>-f, --force</dt>
  <dd>強制刪除，而不進行確認</dd>
</dl>

<strong>範例</strong>：刪除資源別名 `my-resource-alias` 與應用程式 `my-app` 之間的資源連結：

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

列出資源實例或資源別名的資源索引鍵

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>--instance-id</dt>
  <dd>資源實例 ID</dd>
  <dt>--instance-name</dt>
  <dd>資源實例名稱</dd>
  <dt>--alias-id</dt>
  <dd>資源別名 ID</dd>
  <dt>--alias-name</dt>
  <dd>資源別名</dd>
</dl>

<strong>範例</strong>：列出資源實例 `my-resource-instance` 的資源索引鍵：

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

顯示資源索引鍵的詳細資料

```
bluemix resource key KEY_NAME [--id]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>KEY_NAME</dt>
  <dd>索引鍵的名稱</dd>
  <dt>--id</dt>
  <dd>顯示資源索引鍵的 ID</dd>
</dl>

<strong>範例</strong>：顯示資源索引鍵 `my-resource-key` 的詳細資料：

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

建立資源索引鍵

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>NAME</dt>
  <dd>索引鍵的名稱</dd>
  <dt>ROLE_NAME</dt>
  <dd>使用者角色的名稱</dd>
  <dt>--instance-id</dt>
  <dd>資源實例 ID</dd>
  <dt>--instance-name</dt>
  <dd>資源實例名稱</dd>
  <dt>--alias-id</dt>
  <dd>資源別名 ID</dd>
  <dt>--alias-name</dt>
  <dd>資源別名</dd>
  <dt>-service-id-name</dt>
  <dd>角色所屬服務 ID 的名稱</dd>
  <dt>-f, --force</dt>
  <dd>強制建立，而不進行確認</dd>
</dl>

<strong>範例</strong>：以 `Administrator` 角色，為資源實例 `my-resource-instance` 建立名為 `my-resource-key` 的資源索引鍵：

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

刪除資源索引鍵

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>KEY_NAME</dt>
  <dd>索引鍵的名稱</dd>
  <dt>-f, --force</dt>
  <dd>強制刪除，而不進行確認</dd>
</dl>

<strong>範例</strong>：刪除資源索引鍵 `my-resource-key`：

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

列出資源實例的別名

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>--instance-id</dt>
  <dd>隸屬資源實例的 ID。</dd>
  <dt>--instance-name</dt>
  <dd>隸屬資源實例的名稱。</dd>
</dl>

<strong>範例</strong>：列出資源實例 `my-resource-instance` 的資源別名：
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

顯示資源別名的詳細資料

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>ALIAS_NAME（必要）</dt>
  <dd>資源別名的名稱</dd>
  <dt>--id</dt>
  <dd>僅顯示給定資源別名的 ID。會抑制別名的所有其他輸出。</dd>
</dl>

<strong>範例</strong>：顯示資源別名 `my-resource-alias` 的詳細資料：
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

建立資源實例的別名

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>ALIAS_NAME（必要）</dt>
  <dd>資源別名的名稱</dd>
  <dt>--instance-id</dt>
  <dd>隸屬資源實例的 ID。</dd>
  <dt>--instance-name</dt>
  <dd>隸屬資源實例的名稱。</dd>
  <dt>-s</dt>
  <dd>在其中建立別名的空間名稱。預設為現行空間。</dd>
  <dt>-t, --tags</dt>
  <dd>標籤清單。</dd>
  <dt>-p, --parameters</dt>
  <dd>參數 JSON 檔案或 JSON 字串。</dd>
</dl>

<strong>範例</strong>：為資源實例 `my-resource-instance` 建立名為 `my-resource-alias` 的資源別名：
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

更新資源別名

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>ALIAS_NAME（必要）</dt>
  <dd>資源別名的名稱</dd>
  <dt>-n, --name</dt>
  <dd>資源別名的新名稱。</dd>
  <dt>-t, --tags</dt>
  <dd>標籤清單。</dd>
  <dt>-p, --parameters</dt>
  <dd>參數 JSON 檔案或 JSON 字串。</dd>
  <dt>-f, --force</dt>
  <dd>強制更新，而不進行使用者確認。</dd>
</dl>

<strong>範例</strong>：更新資源別名 `my-resource-alias`，並將其名稱變更為 `new-resource-alias`：

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

刪除資源別名

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>ALIAS_NAME（必要）</dt>
  <dd>資源別名的名稱</dd>
  <dt>-f, --force</dt>
  <dd>強制刪除，而不進行確認</dd>
</dl>

<strong>範例</strong>：刪除資源別名 `my-resource-alias`：

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

搜尋型錄項目

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-q, --query</dt>
  <dd>搜尋關鍵字</dd>
  <dt>-r, --region</dt>
  <dd>指定要在其中搜尋的地理區域。目前僅支援 "us-south" 及 "united-kingdom"</dd>
  <dt>-k, --kind</dt>
  <dd>依資源類型過濾。目前僅支援 "service-cf"、"iaas"、"runtime"、"template" 及 "dashboard"</dd>
  <dt>-p, --price</dt>
  <dd>依價格過濾。目前僅支援 "free"、"paygo" 及 "bluemix-subscription"</dd>
  <dt>-t, --tag</dt>
  <dd>依標籤過濾。</dd>
  <dt>-sort-by</dt>
  <dd>內容排序方式</dd>
  <dt>-reverse</dt>
  <dd>是否反轉排序順序</dd>
  <dt>-json</dt>
  <dd>輸出原始 JSON 回應</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

搜尋服務 `Automation test`：

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

取得型錄項目

```
bluemix catalog entry [-i ID] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>型錄項目的 ID。</dd>
  <dt>-children</dt>
  <dd>取得型錄項目的所有子項</dd>
  <dt>-json</dt>
  <dd>輸出原始 JSON 回應</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

取得 ID 為 `a0ef1-d3b4j0` 的項目：

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
建立新型錄項目（僅限帳戶的型錄管理者）

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-p, --parent</dt>
  <dd>物件的母項 ID</dd>
  <dt>-c</dt>
  <dd>包含型錄特定配置參數的有效 JSON 物件（透過行內或檔案所提供）。如需所支援配置參數的清單，請參閱特定型錄項目的文件。</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

從 JSON 檔案，建立母項 ID 為 `a0ef1-d3b4j0` 的資源：

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
更新現有型錄項目（僅限帳戶的型錄管理者或編輯者）

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>所更新型錄項目的 ID。</dd>
  <dt>-c</dt>
  <dd>包含型錄特定配置參數的有效 JSON 物件（透過行內或檔案所提供）。如需所支援配置參數的清單，請參閱特定型錄項目的文件。</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

從 JSON 檔案，更新資源 `j402-dnf1i`：

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
取得型錄項目的可見性（僅限帳戶的型錄管理者）

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>型錄項目的 ID。</dd>
  <dt>-json</dt>
  <dd>輸出原始 JSON 回應</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

取得廣域範圍中資源 `j402-dnf1i` 的可見性：

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
更新現有型錄項目的可見性（僅限帳戶的型錄管理者）

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>所更新型錄項目的 ID。</dd>
  <dt>-c</dt>
  <dd>包含型錄特定配置參數的有效 JSON 物件（透過行內或檔案所提供）。如需所支援配置參數的清單，請參閱特定型錄項目的文件。</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

從 JSON 檔案，設定資源 `j402-dnf1i` 的可見性：

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
列出市場中的服務供應項目

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
<dl>
  <dt>-cf</dt>
  <dd>僅顯示 Cloud Foundry 服務</dd>
  <dt>-rc</dt>
  <dd>僅顯示 RC 相容服務</dd>
  <dt>-global</dt>
  <dd>在廣域範圍中操作</dd>
</dl>

<strong>範例</strong>：

顯示廣域範圍中的服務供應項目：

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

檢視 Bluemix 上的樣板範本。

```
bluemix catalog templates [-d]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

   <dl>
   <dt>-d（選用）</dt>
   <dd>如果指定 <i>-d</i> 選項，也會顯示每個範本的說明。否則，只會顯示每一個範本的 ID 及名稱。</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

檢視所指定樣板範本的詳細資訊。

```
bluemix catalog template TEMPLATE_ID
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：
   <dl>
   <dt>TEMPLATE_ID（必要）</dt>
   <dd>樣板範本的 ID。請使用 <i>bluemix templates</i> 來檢視所有範本的 ID。</dd>
   </dl>


<strong>範例</strong>：

檢視範本 `mobileBackendStarter` 的詳細資料：

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

以指定的 URL 及說明，建立根據所指定範本的 cf 應用程式。依預設，新的應用程式會自動啟動。

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>必要條件</strong>：端點、登入、目標

<strong>指令選項</strong>：
   <dl>
   <dt>TEMPLATE_ID（必要）</dt>
   <dd>應用程式在建立時將根據的範本。使用 <i>bluemix templates</i> 來查看所有範本 ID。</dd>
   <dt>CF_APP_NAME（必要）</dt>
   <dd>要建立之 cf 應用程式的名稱。</dd>
   <dt>-u <i>URL</i>（選用）</dt>
   <dd>應用程式的路徑。如果未指定，Bluemix 會自動根據應用程式名稱及預設網域來設定路徑。</dd>
   <dt>-d <i>DESCRIPTION</i>（選用）</dt>
   <dd>應用程式的說明。</dd>
   <dt>--no-start（選用）</dt>
   <dd>建立應用程式之後，不要自動將它啟動。如果未指定，應用程式會在建立之後自動啟動。</dd>
   </dl>


<strong>範例</strong>：

根據 `javaHelloWorld` 範本建立 cf 應用程式 `my-app`：

```
bluemix catalog template-run javaHelloWorld my-app
```

根據 `rubyHelloWorld` 範本建立應用程式 `my-ruby-app`，路徑為 `myrubyapp.chinabluemix.net`，說明為 `My first ruby app on {{site.data.keyword.Bluemix_notm}}.`：

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

根據 `pythonHelloWorld` 範本建立應用程式 `my-python-app`，不自動啟動：

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

顯示帳戶的每月用量和費用。

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

<dl>
  <dt>-d MONTH_DATE（選用）</dt>
  <dd>顯示以 YYYY-MM 格式指定之月份和日期的資料。如果未指定，則會顯示現行月份的用量。</dd>
  <dt>--json（選用）</dt>
  <dd>以 JSON 格式顯示用量結果。</dd>
</dl>

<strong>範例</strong>：

顯示我的帳戶在 2016-06 的用量和費用報告：

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

顯示組織的每月用量詳細資料。只有組織的帳單管理員可以執行此作業。

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

<dl>
  <dt>ORG_NAME（必要）</dt>
  <dd>組織的名稱。</dd>
  <dt>-d MONTH_DATE（選用）</dt>
  <dd>顯示以 YYYY-MM 格式指定之月份和日期的資料。如果未指定，則會顯示現行月份的用量。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>管理組織的地區名稱。如果設為 'all'，則會顯示組織在所有地區的用量。</dd>
  <dt>--json（選用）</dt>
  <dd>以 JSON 格式顯示用量結果。</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

顯示我的帳戶中組織的每月用量摘要。

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>必要條件</strong>：端點、登入

<strong>指令選項</strong>：

<dl>
  <dt>-d MONTH_DATE（選用）</dt>
  <dd>顯示以 YYYY-MM 格式指定之月份和日期的資料。如果未指定，則會顯示現行月份的用量。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>管理組織的地區名稱。如果設為 'all'，則會顯示組織在所有地區的用量摘要。</dd>
  <dt>--json（選用）</dt>
  <dd>以 JSON 格式顯示用量結果。</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

列出 {{site.data.keyword.Bluemix_notm}} CLI 中登錄的所有外掛程式儲存庫。

```
bluemix plugin repos
```

<strong>必要條件</strong>：無


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

將新的外掛程式儲存庫新增至 {{site.data.keyword.Bluemix_notm}} CLI。

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>REPO_NAME（必要）</dt>
   <dd>要新增之儲存庫的名稱。您可以自行為每一個儲存庫定義名稱。</dd>
   <dt>REPO_URL（必要）</dt>
   <dd>要新增之儲存庫的 URL。儲存庫 URL 必須包含通訊協定（例如，http://plugins.ng.bluemix.net 而非 plugins.ng.bluemix.net）。http://plugins.ng.bluemix.net 是 Bluemix CLI 的正式外掛程式儲存庫。</dd>
    </dl>


<strong>範例</strong>：

將 Bluemix CLI 的官方外掛程式儲存庫新增為 `bluemix-repo`：

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

從 {{site.data.keyword.Bluemix_notm}} CLI 移除外掛程式儲存庫。

```
bluemix plugin repo-remove REPO_NAME
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
   <dl>
   <dt>REPO_NAME（必要）</dt>
   <dd>要移除之儲存庫的名稱。</dd>
   </dl>

<strong>範例</strong>：

從 {{site.data.keyword.Bluemix_notm}} CLI 移除 `bluemix-repo` 儲存庫：

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

列出所有已新增之儲存庫或特定儲存庫中所有可用的外掛程式。

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>-r <i>REPO_NAME</i>（選用）</dt>
   <dd>只列出指定儲存庫中的外掛程式。</dd>
   </dl>

<strong>範例</strong>：

列出所有已新增之儲存庫中的所有外掛程式：

```
bluemix plugin repo-plugins
```

列出 `bluemix-repo` 儲存庫中的所有外掛程式：

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

顯示儲存庫中外掛程式的詳細資料。

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>-r <i>REPO_NAME</i>（選用）</dt>
   <dd>儲存庫的名稱。如果未指定儲存庫，則指令會使用預設的外掛程式儲存庫。</dd>
   </dl>

<strong>範例</strong>：

列出儲存庫 "sample-repo" 中外掛程式 "IBM-Containers" 的詳細資料：

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

列出預設儲存庫中外掛程式 "IBM-Containers" 的詳細資料

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

列出 {{site.data.keyword.Bluemix_notm}} CLI 中的所有已安裝外掛程式。

```
bluemix plugin list
```

<strong>必要條件</strong>：無

## bluemix plugin show
{: #bluemix_plugin_show}

顯示已安裝外掛程式的詳細資料

```
bluemix plugin show PLUGIN-NAME
```

<strong>必要條件</strong>：無


## bluemix plugin install
{: #bluemix_plugin_install}

從指定的路徑或儲存庫將特定版本的外掛程式安裝到 {{site.data.keyword.Bluemix_notm}} CLI 中。

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME（必要）</dt>
   <dd>如果未指定 -r <i>REPO_NAME</i>，則會從指定的本端路徑或遠端 URL 來安裝外掛程式。</dd>
   <dt>-r <i>REPO_NAME</i>（選用）</dt>
   <dd>外掛程式二進位檔所在儲存庫的名稱。如果未指定儲存庫，則指令會使用預設的外掛程式儲存庫。</dd>
   <dt>-v <i>VERSION</i>（選用）</dt>
   <dd>要安裝之外掛程式的版本。如果未提供，將安裝外掛程式的最新版本。只有從儲存庫安裝外掛程式時，此選項才有效。</dd>
    </dl>

<strong>範例</strong>：

從本端檔案安裝外掛程式：

```
bluemix plugin install /downloads/new_plugin
```

從遠端 URL 安裝外掛程式：

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

從 `bluemix-repo` 儲存庫安裝最新版本的 `IBM-Containers` 外掛程式：

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
從 `bluemix-repo` 儲存庫安裝版本為 `0.5.800` 的 `IBM-Containers` 外掛程式：
```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

從儲存庫升級外掛程式

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>要更新之外掛程式的名稱。如果未指定，則這個指令會檢查所有已安裝外掛程式的升級。</dd>
 <dt>-r REPO_NAME</dt>
 <dd>外掛程式二進位檔所在儲存庫的名稱。如果未指定，則這個指令會使用預設外掛程式儲存庫。</dd>
 <dt>-v <i>VERSION</i>（選用）</dt>
 <dd>外掛程式要更新到的目標版本。如果未提供，便將外掛程式更新至最新的可用版本。</dd>
 <dt>--all</dt>
 <dd>更新所有可用的外掛程式</dd>
</dl>

<strong>範例</strong>：

檢查外掛程式儲存庫 "My-Repo" 中的所有可用升級：

```
bluemix plugin update -r My-Repo
```

將儲存庫 "My-Repo" 中的外掛程式 "plugin-echo" 升級至最新版本：

```
bluemix plugin update -r My-Repo plugin-echo
```

將儲存庫 "My-Repo" 中的外掛程式 "plugin-echo" 更新為 "1.0.1" 版：

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

從 {{site.data.keyword.Bluemix_notm}} CLI 解除安裝指定的外掛程式。

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>必要條件</strong>：無

<strong>指令選項</strong>：

   <dl>
   <dt>PLUGIN_NAME（必要）</dt>
   <dd>要解除安裝之外掛程式的名稱。</dd>
    </dl>

<strong>範例</strong>：

解除安裝先前安裝的 `IBM-Containers` 外掛程式：

```
bluemix plugin uninstall IBM-Containers
```

