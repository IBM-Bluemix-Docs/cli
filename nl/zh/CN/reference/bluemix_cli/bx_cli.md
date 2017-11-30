---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.Bluemix_notm}} (bx) 命令
{: #bluemix_cli}

版本：0.6.1

{{site.data.keyword.Bluemix_notm}} 命令行界面 (CLI) 提供了一组按名称空间分组的命令，供用户用于与 {{site.data.keyword.Bluemix_notm}} 进行交互。 

从 V0.5.0 开始，{{site.data.keyword.Bluemix_notm}} 命令行客户机在其安装中捆绑了 Cloud Foundry 命令行客户机。如果您已安装 cf CLI，请勿在同一上下文中同时使用 {{site.data.keyword.Bluemix_notm}} CLI 命令 `bx [command]` 和您自己安装的 Cloud Foundry CLI 命令 `cf [command]`。如果要在 {{site.data.keyword.Bluemix_notm}} CLI 上下文中使用 cf CLI 来管理 Cloud Foundry 资源，请改为使用 `bluemix cf [command]`。此外，也不允许使用 `bluemix cf api/login/logout/target`，请改为使用 `bluemix api/login/logout/target`。

下面列出了 {{site.data.keyword.Bluemix_notm}} CLI 支持的详细命令用法，包括命令名称、自变量、选项、先决条件、描述和示例。
{:shortdesc}

**注：***先决条件*列出使用命令前必须执行的操作。没有任何先决条件操作的命令会列出**无**。否则，先决条件可能会包含以下一个或多个操作：

<dl>
<dt>端点</dt>
<dd>使用命令前，必须通过 <code>bluemix api</code> 设置 API 端点。</dd>
<dt>登录</dt>
<dd>使用此命令之前，必须使用 <code>bluemix login</code> 命令登录。如果使用联合标识登录，请使用“--sso”选项通过一次性密码进行认证，或者使用“--apikey”通过 API 密钥进行认证。转至 {{site.data.keyword.Bluemix_notm}} 控制台的**管理** &gt; **安全性** &gt; **Bluemix API 密钥**以创建 API 密钥。
</dd>
<dt>目标</dt>
<dd>使用命令前，必须通过 <code>bluemix target</code> 命令设置组织和空间。</dd>
<dt>Docker</dt>
<dd>必须安装 Docker CLI (docker) 才能运行此命令。</dd>
</dl>

**注：**可以使用 Bluemix 命令的短格式；例如，`bx api` 是 `bluemix api` 的短格式。

使用下表中的索引可查看常用 bluemix 命令：

## 常规 bluemix 命令 
{: #bx_commands_index}

<table summary="常规 bluemix 命令。">
 <caption>表 1. 常规 bluemix 命令</caption>
 <thead>
 <th colspan="5">常规 bluemix 命令</th>
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
 
 ## 用于管理和配置 {{site.data.keyword.BluSoftlayer_notm}} 服务的命令
  {: #bx_commands_softlayer}
  
用于管理 {{site.data.keyword.BluSoftlayer_notm}} 的命令已合并到 Bluemix CLI 中。有关使用 Bluemix CLI 来配置和管理 {{site.data.keyword.BluSoftlayer_notm}} 服务的更多信息，请参阅：[Bluemix CLI {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) 命令](/docs/cli/reference/softlayer/index.md#softlayer_cli)。
 
 ## 用于管理帐户、组织和角色的命令
 {: #bx_commands_account}

<table summary="可用于管理帐户、组织、空间和角色的 Bluemix 命令。">
<caption>表 2. 用于管理帐户、组织、空间和角色的命令</caption>
 <thead>
 <th colspan="5">用于管理帐户、组织、空间和角色的命令</th>
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


 ## 用于管理资源组和资源的命令
{: #bx_commands_resource}

<table summary="可用于管理资源组和资源的 Bluemix 命令。">
<caption>表 3. 用于管理资源组和资源的命令</caption>
  <thead>
    <th colspan="5">用于管理资源组和资源的命令</th>
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

 
 ## 用于管理 API 密钥和策略的命令
 {: #bx_commands_iam}
 <table summary="可用于管理 API 密钥和策略的 Bluemix 命令。">
<caption>表 3. 用于管理 API 密钥和策略的命令</caption>
  <thead>
  <th colspan="5">用于管理 API 密钥和策略的命令</th>
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
 
 ## 用于管理 CF 应用程序及与应用程序相关的域、路径和证书的命令
 {: #bx_commands_apps}

<table summary="可用于管理 CF 应用程序及与应用程序相关的域、路径和证书的 Bluemix 命令。">
<caption>表 4. 用于管理 CF 应用程序及与应用程序相关的域、路径和证书的命令</caption>
 <thead>
 <th colspan="5">用于管理 CF 应用程序及与应用程序相关的域、路径和证书的命令</th>
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
 
 ## 用于管理 Bluemix 服务的命令
 {: #bx_commands_services}

<table summary="可用于管理 Bluemix 服务的 bluemix 命令">
 <caption>表 5. 用于管理 Bluemix 服务的命令</caption>
 <thead>
 <th colspan="5">用于管理 Bluemix 服务的命令</th>
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

 
 ## 用于管理目录、插件和帐单设置的命令
 {: #bx_commands_settings}

<table summary="可用于管理 Bluemix 目录、插件、帐单和安全设置的 bluemix 命令">
<caption>表 6. 用于管理 Bluemix 目录、插件、帐单和安全设置的命令</caption>
 <thead>
 <th colspan="5">用于管理 Bluemix 目录、插件、帐单和安全设置的命令</th>
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
显示 {{site.data.keyword.Bluemix_notm}} CLI 第一级内置命令和受支持名称空间的一般帮助，或者显示特定内置命令或名称空间的帮助。

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>COMMAND|NAMESPACE（可选）</dt>
   <dd>显示其帮助信息的命令或名称空间。如果未指定，将显示 {{site.data.keyword.Bluemix_notm}} CLI 的一般帮助。</dd>
   </dl>



<strong>示例</strong>：

显示 {{site.data.keyword.Bluemix_notm}} CLI 的一般帮助：

```
bluemix help
```

显示 `info` 命令的帮助：

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
设置或查看 {{site.data.keyword.Bluemix_notm}} API 端点。

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
   <dl>
   <dt>API_ENDPOINT（可选）</dt>
   <dd>作为目标的 API 端点，例如 `https://api.chinabluemix.net`。如果未指定 *API_ENDPOINT* 和 `--unset` 选项，将显示当前 API 端点。</dd>
   <dt>--unset（可选）</dt>
   <dd>除去 API 端点设置。</dd>
   <dt>--skip-ssl-validation（可选）</dt>
   <dd>绕过 HTTP 请求的 SSL 验证。</dd>
   </dl>
<strong>示例</strong>：

将 API 端点设置为 api.chinabluemix.net：

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

查看当前 API 端点：

```
bluemix api
```

取消设置 API 端点：

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


将缺省值写入配置文件。

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>HTTP 请求的超时值。缺省值为 60 秒。</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>跟踪对终端或指定文件的 HTTP 请求。</dd>
   <dt>--color true|false</dt>
   <dd>启用或禁用颜色输出。缺省情况下，会启用颜色输出。</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>设置缺省语言环境。如果 LOCALE 为 <i>CLEAR</i>，将删除先前的语言环境。</dd>
   <dt>--check-version true|false</dt>
   <dd>启用或禁用 CLI 版本检查。</dd>
   </dl>

一次只能指定其中一个选项。

<strong>示例</strong>：

将 HTTP 请求超时设置为 30 秒：

```
bluemix config --http-timeout 30
```

启用 HTTP 请求的跟踪输出：

```
bluemix config --trace true
```

跟踪对指定文件 */home/usera/my_trace* 的 HTTP 请求：

```
bluemix config --trace /home/usera/my_trace
```

禁用颜色输出：

```
bluemix config --color false
```

将语言环境设置为 zh_Hans：

```
bluemix config --locale zh_Hans
```

清除语言环境设置：

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

查看基本 {{site.data.keyword.Bluemix_notm}} 信息，包括当前区域、云控制器版本以及一些有用的端点，例如用于登录和交换访问令牌的端点。

```
bluemix info
```

<strong>先决条件</strong>：端点


## bluemix cf
{: #bluemix_cf}

调用嵌入式 CF CLI

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
<dl>
  <dt>-q, --quiet</dt>
  <dd>关闭消息“正在调用 cf 命令...”</dd>
</dl>

<strong>示例</strong>：

列出 CF 应用程序：

```
bluemix cf apps
```

列出 CF 服务，而不显示消息“正在调用 cf 命令...”：

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

用户登录。 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>先决条件</strong>：无

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>命令选项</strong>：
<dl>
  <dt> -a <i>API_ENDPOINT</i>（可选）</dt>
  <dd> API 端点（例如：api.ng.bluemix.net）</dd>
  <dt> --apikey <i>API_KEY 或 @API_KEY_FILE_PATH</i>
  <dd> API 密钥内容或用 @ 指示的 API 密钥文件路径</dd>
  <dt> --sso（可选）</dt>
  <dd> 使用一次性密码登录</dd>
  <dt> -u <i>USERNAME</i>（可选）</dt>
  <dd> 用户名</dd>
  <dt> -p <i>PASSWORD</i>（可选）</dt>
  <dd> 密码</dd>
  <dt> -c <i>ACCOUNT_ID</i>（可选）</dt>
  <dd> 目标帐户的标识</dd>
  <dt> -o <i>ORG_NAME</i>（可选）</dt>
  <dd> 目标组织的名称</dd>
  <dt> -s <i>SPACE_NAME</i>（可选）</dt>
  <dd> 目标空间的名称</dd>
  <dt> --skip-ssl-validation（可选）</dt>
  <dd> 绕过 HTTP 请求的 SSL 验证。建议不要使用此选项。</dd>
</dl>

<strong>示例</strong>：

#### 交互式登录

```
bluemix login
```

使用用户名和密码登录，并设置目标帐户、组织和空间：

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

使用一次性密码登录，并设置目标帐户、组织和空间

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

使用 API 密钥登录并设置目标：

#### API 密钥具有关联的帐户

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### API 密钥没有关联的帐户

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>注：</strong>如果 API 密钥具有关联的帐户，那么不允许切换到其他帐户。

#### 使用一次性密码

```
bluemix login -u UserID --sso
```

然后，CLI 将提供一个 URL 链接并要求输入密码：
```
One Time Code (Get one at https://URL_Link_To_Obtain_Passcode):
```

在浏览器中打开链接，该链接将引导您获取密码。在控制台中输入提供的密码，然后您应该能够登录。

## bluemix logout
{: #bluemix_logout}

注销用户。

```
bluemix logout
```

<strong>先决条件</strong>：无

## bluemix regions
{: #bluemix_regions}

查看 {{site.data.keyword.Bluemix_notm}} 上所有区域的信息。

```
bluemix regions
```

<strong>先决条件</strong>：端点


## bluemix target
{: #bluemix_target}


设置或查看目标帐户、区域、组织或空间。

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>-r <i>REGION_NAME</i>（可选）</dt>
   <dd>要切换到的区域的名称，例如“us-south”或“eu-gb”。</dd>
   <dt>-c <i>ACCOUNT_ID</i>（可选）</dt>
   <dd>要作为目标的帐户的标识。</dd>
   <dt>--cf</dt>
   <dd>以交互方式选择目标组织和空间</dd>
   <dt>-o <i>ORG_NAME</i>（可选）</dt>
   <dd>要作为目标的组织的名称。</dd>
   <dt>-s <i>SPACE_NAME</i>（可选）</dt>
   <dd>要作为目标的空间的名称。</dd>
   </dl>
如果未指定任何选项，那么将显示当前帐户、区域、组织和空间。
<strong>示例</strong>：

设置当前帐户、组织和空间：

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

切换到新区域：

```
bluemix target -r eu-gb
```

查看当前帐户、区域、组织和空间：

```
bluemix target
```

### bluemix update
{: #bluemix_update}

将 CLI 更新到最新版本。

```
bluemix update
```

<strong>先决条件</strong>：无

### bluemix account orgs
{: #bluemix_account_orgs}

列出所有组织

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>-r <i>REGION</i>（可选）</dt>
   <dd>显示其组织信息的区域。如果设置为“all”，将列出所有区域中的所有组织。</dd>
   <dt>--guid（可选）</dt>
   <dd>显示组织的 GUID。</dd>
   </dl>

<strong>示例</strong>：

列出区域 `us-south` 中的所有组织并显示 GUID

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

显示指定组织的信息。

```
bluemix account org ORG_NAME [--guid]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>ORG_NAME（必需）</dt>
   <dd>组织的名称。</dd>
   <dt>--guid（可选）</dt>
   <dd>显示组织的 GUID。</dd>
   </dl>

<strong>示例</strong>：

显示组织 `IBM` 的信息并显示 GUID

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

创建新组织。此操作只能由帐户所有者执行。

```
bluemix account org-create ORG_NAME
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>ORG_NAME（必需）</dt>
   <dd>要创建的组织的名称。</dd>
   </dl>

<strong>示例</strong>：

创建名为 `IBM` 的组织。

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

将组织从当前区域复制到其他区域。

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>ORG_NAME（必需）</dt>
   <dd>要复制的现有组织的名称。</dd>
   <dt>REGION_NAME（必需）</dt>
   <dd>托管所复制组织的区域的名称。</dd>
   </dl>

<strong>示例</strong>：

将组织 `myorg` 复制到区域 `eu-gb`：

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

重命名组织。此操作只能由组织管理员执行。

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>OLD_ORG_NAME（必需）</dt>
   <dd>要重命名的组织的旧名称。</dd>
   <dt>NEW_ORG_NAME（必需）</dt>
   <dd>组织要重命名为的新名称。</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

此命令的功能和选项与 `cf spaces` 命令的相同。


## bluemix account space
{: #bluemix_account_space}

此命令的功能和选项与 `cf space` 命令的相同。


## bluemix account space-create
{: #bluemix_account_space_create}

此命令的功能和选项与 `cf create-space` 命令的相同。


## bluemix account space-rename
{: #bluemix_account_space_rename}


此命令的功能和选项与 `cf rename-space` 命令的相同。


## bluemix account space-delete
{: #bluemix_account_space_delete}


此命令的功能和选项与 `cf delete-space` 命令的相同。

## bluemix account org-users
{: #bluemix_account_org_users}

按角色显示指定组织中的用户。

```
bluemix account org-users ORG_NAME [-a]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>ORG_NAME（必需）</dt>
<dd>组织的名称。</dd>
<dt>-a（可选）</dt>
<dd>列出指定组织中的所有用户，但不按角色分组。</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

将用户添加到组织（需要组织管理员）。

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

从组织除去用户（仅限组织管理员或用户自己）

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>命令选项</strong>：
<dl>
<dt>--force, -f</dt>
<dd>强制删除而不确认。</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

获取当前用户的所有组织角色

```
bluemix account org-roles
```

<strong>先决条件</strong>：端点和登录

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

向用户分配组织角色。此操作只能由组织管理员执行。

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
  <dl>
   <dt>USER_NAME（必需）</dt>
   <dd>要分配的用户的名称。</dd>
   <dt>ORG_NAME（必需）</dt>
   <dd>要将此用户分配到的组织的名称。</dd>
   <dt>ORG_ROLE（必需）</dt>
   <dd>要将此用户分配到的组织角色的名称。例如：
<ul>
   <li>OrgManager：此角色可以邀请和管理用户，选择并更改套餐，以及设置花费限制。</li>
   <li>BillingManager：此角色可以创建和管理缴费帐户和付款信息。</li>
   <li>OrgAuditor：此角色具有对组织信息和报告的只读访问权。</li>
   </ul>
   </dd>
  </dl>

<strong>示例</strong>：

将用户 `Mary` 以 `OrgManager` 角色分配给组织 `IBM`：

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**注**：您可以使用 CLI 设置组织/空间角色，但是如果您想要设置其他许可权，那么必须使用 UI。有关进一步的详细信息，请参阅[分配用户访问权](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)。<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

除去用户的组织角色。此操作只能由组织管理员执行。

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>USER_NAME（必需）</dt>
   <dd>要除去的用户的名称。</dd>
   <dt>ORG_NAME（必需）</dt>
   <dd>要将此用户从中除去的组织的名称。</dd>
   <dt>ORG_ROLE（必需）</dt>
   <dd>要将此用户从中除去的组织角色的名称。例如：
<ul>
   <li>OrgManager：此角色可以邀请和管理用户，选择并更改套餐，以及设置花费限制。</li>
   <li>BillingManager：此角色可以创建和管理缴费帐户和付款信息。</li>
   <li>OrgAuditor：此角色具有对组织信息和报告的只读访问权。</li>
   </ul>
   </dd>
    </dl>

<strong>示例</strong>：

从组织 `IBM` 中除去用户 `Mary` 的 `OrgManager` 角色：

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

按角色显示指定空间中的用户。

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>ORG_NAME（必需）</dt>
   <dd>组织的名称。</dd>
   <dt>SPACE_NAME（必需）</dt>
   <dd>空间的名称。</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

向用户分配空间角色。此操作只能由空间管理员执行。

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

   <dl>
   <dt>USER_NAME（必需）</dt>
   <dd>要分配的用户的名称。</dd>
   <dt>ORG_NAME（必需）</dt>
   <dd>要将此用户分配到的组织的名称。</dd>
   <dt>SPACE_NAME（必需）</dt>
   <dd>要将此用户分配到的空间的名称。</dd>
   <dt>SPACE_ROLE（必需）</dt>
   <dd>要将此用户分配到的空间角色的名称。例如：
<ul>
   <li>SpaceManager：此角色可以邀请和管理用户，以及启用给定空间的功能。</li>
   <li>SpaceDeveloper：此角色可以创建和管理应用程序与服务，以及查看日志和报告。</li>
   <li>SpaceAuditor：此角色可以查看空间的日志、报告和设置。</li>
   </ul></dd>
    </dl>

<strong>示例</strong>：

将用户 `Mary` 以 `SpaceManager` 角色分配给组织 `IBM` 和空间 `Cloud`：

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

除去用户的空间角色。此操作只能由空间管理员执行。

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

   <dl>
   <dt>USER_NAME（必需）</dt>
   <dd>要除去的用户的名称。</dd>
   <dt>ORG_NAME（必需）</dt>
   <dd>要将此用户从中除去的组织的名称。</dd>
   <dt>SPACE_NAME（必需）</dt>
   <dd>要将此用户从中除去的空间的名称。</dd>
   <dt>SPACE_ROLE（必需）</dt>
   <dd>要将此用户从中除去的空间角色的名称。例如：
<ul>
   <li>SpaceManager：此角色可以邀请和管理用户，以及启用给定空间的功能。</li>
   <li>SpaceDeveloper：此角色可以创建和管理应用程序与服务，以及查看日志和报告。</li>
   <li>SpaceAuditor：此角色可以查看空间的日志、报告和设置。</li>
   </ul></dd>
    </dl>


<strong>示例</strong>：

从组织 `IBM` 和空间 `Cloud` 中除去用户 `Mary` 的 `SpaceManager` 角色：

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

列出当前用户的所有帐户

```
bluemix account list
```

<strong>先决条件</strong>：端点和登录


## bluemix account org-account
{: #bluemix_account_org_account}

显示指定组织的帐户（需要组织用户）

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
  <dt>--guid（可选）</dt>
  <dd>仅显示帐户标识</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

显示与帐户关联的用户。此操作只能由帐户所有者执行。

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

从当前帐户中删除用户（仅帐户所有者）

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>USERNAME（必需）</dt>
<dd>用户名</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>帐户标识。如果未指定，缺省值为当前帐户。</dd>
<dt>--force, -f（可选）</dt>
<dd>强制删除而不确认。</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

邀请用户加入已设置组织和空间角色的帐户。此操作只能由帐户所有者执行。

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
   <dt>USER_NAME（必需）</dt>
   <dd>要邀请的用户的名称。</dd>
   <dt>ORG_NAME（必需）</dt>
   <dd>要邀请此用户加入的组织的名称。</dd>
   <dt>ORG_ROLE（必需）</dt>
   <dd>要邀请此用户加入的组织角色的名称。例如：
<ul>
  <li>OrgManager：此角色可以邀请和管理用户，选择并更改套餐，以及设置花费限制。</li>
  <li>BillingManager：此角色可以创建和管理缴费帐户和付款信息。</li>
  <li>OrgAuditor：此角色具有对组织信息和报告的只读访问权。</li>
  </ul> </dd>
   <dt>SPACE_NAME（必需）</dt>
   <dd>要邀请此用户加入的空间的名称。</dd>
   <dt>SPACE_ROLE（必需）</dt>
   <dd>要邀请此用户加入的空间的名称。要邀请此用户加入的空间角色的名称。例如：
<ul>
<li>SpaceManager：此角色可以邀请和管理用户，以及启用给定空间的功能。</li>
<li>SpaceDeveloper：此角色可以创建和管理应用程序与服务，以及查看日志和报告。</li>
<li>SpaceAuditor：此角色可以查看空间的日志、报告和设置。</li>
</ul>
</dd>
</dl>

<strong>示例</strong>：

邀请用户 `Mary` 以 `OrgManager` 角色加入组织 `IBM`，并以 `SpaceAuditor` 角色加入空间 `Cloud`：

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**注**：您可以在邀请期间使用 CLI 设置组织/空间角色，但是如果您想要设置其他许可权，那么必须使用 UI。有关进一步的详细信息，请参阅[分配用户访问权](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess)。<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

向用户重新发送邀请（必须是组织管理员或帐户所有者）

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

列出所有服务标识

```
bluemix iam service-ids --uuid
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-uuid</dt>
  <dd>仅显示服务标识的 UUID</dd>
</dl>

<strong>示例</strong>：列出当前帐户下所有服务标识的 UUID

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

显示服务标识的详细信息

```
bluemix iam service-id NAME [--uuid]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>服务的名称</dd>
  <dt>-uuid</dt>
  <dd>显示服务标识的 UUID</dd>
</dl>

<strong>示例</strong>：

显示服务标识 `sample-test` 的详细信息

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

创建服务标识

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>服务的名称</dd>
  <dt>-d, --description</dt>
  <dd>服务标识的描述</dd>
</dl>

<strong>示例</strong>：

创建服务名称为 `sample-test` 且描述为 `hello, world!` 的服务标识

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
更新服务标识

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>服务的名称</dd>
  <dt>-n, --name</dt>
  <dd>服务的新名称</dd>
  <dt>-d, --description</dt>
  <dd>服务的新描述</dd>
  <dt>-v, --version</dt>
  <dd>服务标识的版本</dd>
  <dt>-f, --force</dt>
  <dd>更新而不确认</dd>
</dl>

<strong>示例</strong>：

将服务标识 `sample-test` 重命名为 `sample-test2` 而不确认

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

更新服务 `sample-test` 版本 `1-0jn39fbefew` 的描述

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

删除服务标识

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>服务的名称</dd>
  <dt>-f, --force</dt>
  <dd>删除而不确认</dd>
</dl>

<strong>示例</strong>：

删除服务标识 `sample-teset` 而不确认

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

列出所有 Bluemix 平台 API 密钥

```
bluemix iam api-keys
```

<strong>先决条件</strong>：端点和登录

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

创建新的 Bluemix 平台 API 密钥

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>NAME（必需）</dt>
<dd>要创建的 API 密钥的名称。</dd>
<dt>-d <i>DESCRIPTION</i>（可选）</dt>
<dd>API 密钥的描述</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>将 API 密钥信息保存到指定的文件。如果未设置，将显示 JSON 内容。</dd>
</dl>

<strong>示例</strong>：

创建 API 密钥并将其保存到文件

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

更新 Bluemix 平台 API 密钥

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>NAME（必需）</dt>
<dd>要更新的 API 密钥的旧名称。</dd>
<dt>-n <i>NAME</i>（可选）</dt>
<dd>API 密钥的新名称</dd>
<dt>-d <i>DESCRIPTION</i>（可选）</dt>
<dd>API 密钥的新描述</dd>
</dl>

<strong>示例</strong>：

更新 API 密钥的描述：

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

删除 Bluemix 平台 API 密钥

```
bluemix iam api-key-delete NAME [-f]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>NAME（必需）</dt>
<dd>要删除的 API 密钥的名称。</dd>
<dt>-f（可选）</dt>
<dd>强制删除而不确认。</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

列出所有服务 API 密钥

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
</dl>

<strong>示例</strong>：

列出绑定到服务 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 的服务 API 密钥：

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

列出服务 API 密钥的详细信息

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-uuid</dt>
  <dd>显示服务 API 密钥的 UUID</dd>
</dl>

<strong>示例</strong>：

显示绑定到服务 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 的服务 API 密钥 `sample-key` 的详细信息：

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

创建服务 API 密钥

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-d, --description</dt>
  <dd>API 密钥的描述</dd>
  <dt>-f, --file</dt>
  <dd>将 API 密钥信息保存到指定的文件。如果未设置，将显示 JSON 内容。</dd>
</dl>

<strong>示例</strong>：

创建绑定到服务 CRN `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` 的服务 API 密钥 `sample-key`：

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

更新服务 API 密钥

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-n, --name</dt>
  <dd>服务 API 密钥的新名称</dd>
  <dt>-d, --description</dt>
  <dd>服务 API 密钥的新描述</dd>
  <dt>-v, --version</dt>
  <dd>服务 API 密钥的版本</dd>
  <dt>-f, --force</dt>
  <dd>更新而不确认</dd>
</dl>

<strong>示例</strong>：

将服务 API 密钥 `sample-key` 重命名为 `new-sample-key`：

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

删除服务 API 密钥

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-f, --force</dt>
  <dd>删除而不确认</dd>
</dl>

<strong>示例</strong>：

删除服务 API 密钥 `sample-key`：

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

列出用户 `name@example.com` 的策略：

```
bluemix iam user-policies name@example.com
```

<strong>先决条件</strong>：端点、登录和目标帐户

<strong>命令选项</strong>：
<dl>
<dt>USER_NAME（必需）</dt>
<dd>策略所属的用户名</dd>
</dl>

<strong>示例</strong>：

列出用户 `name@example.com` 的策略：

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

显示用户策略的详细信息

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>先决条件</strong>：端点、登录和目标帐户

<strong>命令选项</strong>：
<dl>
<dt>USER_NAME（必需）</dt>
<dd>策略所属的用户名</dd>
<dt>POLICY_ID（必需）</dt>
<dd>策略的标识</dd>
</dl>

<strong>示例</strong>：

列出用户 `name@example.com` 的策略 `0bb730daa`：

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

创建用户策略

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>先决条件</strong>：端点、登录和目标帐户

<strong>命令选项</strong>：
<dl>
<dt>USER_NAME（必需）</dt>
<dd>策略所属的用户名</dd>
<dt>-f, --file <i>FILE</i>（可选）</dt>
<dd>策略定义的 JSON 文件</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i>（可选）</dt>
<dt>--service-name <i>SERVICE_NAME</i>（可选）</dt>
<dd>策略定义的服务名称，此项与“-f, --file”标志互斥。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i>（可选）</dt>
<dd>策略定义的服务实例，此项与“-f, --file”标志互斥。</dd>
<dt>--region <i>REGION</i>（可选）</dt>
<dd>策略定义的区域，此项与“-f, --file”标志互斥。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i>（可选）</dt>
<dd>策略定义的资源类型，此项与“-f, --file”标志互斥。</dd>
<dt>--resource <i>RESOURCE</i>（可选）</dt>
<dd>策略定义的资源，此项与“-f, --file”标志互斥。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i>（可选）</dt>
<dd>资源组的名称，此项与“-f, --file”、“--resource”和“--resource-group-id”标志互斥。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i>（可选）</dt>
<dd>资源组的标识，此项与“-f, --file”、“--resource”和“--resource-group-name”标志互斥。</dd>
  <dd>策略定义的角色名称。要了解某个服务所支持的角色，请运行“bluemix iam roles --service SERVICE_NAME”。此选项与“-f, --file”互斥。</dd>
</dl>

<strong>示例</strong>：

通过策略 JSON 文件 `policy.json` 为用户 `name@example.com` 创建用户策略：

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

授予 `name@example.com` 对所有 `sample-service` 资源的 `Administrator` 角色：

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

授予 `name@example.com` 对 `us-south` 区域中样本服务实例 `ServiceId-ade78e9f` 的资源 `key123` 的 `Editor` 角色：

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

授予 `name@example.com` 对标识为 `dda27e49d2a1efca58083a01dfde18f6` 的资源组的 `Operator` 角色：

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

授予 `name@example.com` 对资源组 `sample-resource-group` 的成员的 `Viewer` 角色：

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

授予 `name@example.com` 对标识为 `dda27e49d2a1efca58083a01dfde18f6` 的资源组成员的 `Viewer` 角色：

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

更新用户策略

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>先决条件</strong>：端点、登录和目标帐户

<strong>命令选项</strong>：
<dt>USER_NAME（必需）</dt>
<dd>策略所属的用户名</dd>
<dt>POLICY_ID（必需）</dt>
<dd>要更新的策略的标识</dd>
<dt>-v, --version <i>VERSION</i>（可选）</dt>
<dd>现有策略的版本</dd>
<dt>-f, --file <i>FILE</i>（可选）</dt>
<dd>策略定义的 JSON 文件</dd>
<dt>-f, --file <i>FILE</i>（可选）</dt>
<dd>策略定义的 JSON 文件</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i>（可选）</dt>
<dt>--service-name <i>SERVICE_NAME</i>（可选）</dt>
<dd>策略定义的服务名称，此项与“-f, --file”标志互斥。</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i>（可选）</dt>
<dd>策略定义的服务实例，此项与“-f, --file”标志互斥。</dd>
<dt>--region <i>REGION</i>（可选）</dt>
<dd>策略定义的区域，此项与“-f, --file”标志互斥。</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i>（可选）</dt>
<dd>策略定义的资源类型，此项与“-f, --file”标志互斥。</dd>
<dt>--resource <i>RESOURCE</i>（可选）</dt>
<dd>策略定义的资源，此项与“-f, --file”标志互斥。</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i>（可选）</dt>
<dd>资源组的名称，此项与“-f, --file”、“--resource”和“--resource-group-id”标志互斥。</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i>（可选）</dt>
<dd>资源组的标识，此项与“-f, --file”、“--resource”和“--resource-group-name”标志互斥。</dd>
  <dd>策略定义的角色名称。要了解某个服务所支持的角色，请运行“bluemix iam roles --service SERVICE_NAME”。此选项与“-f, --file”互斥。</dd>
</dl>

<strong>示例</strong>：

使用 JSON 文件中的用户策略来更新用户策略：

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

更新用户策略以授予 `name@example.com` 对所有 `sample-service` 资源的 `Administrator` 角色：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 更新用户策略以授予 `name@example.com` 对 `us-south` 区域中样本服务实例 `ServiceId-ade78e9f` 的资源 `key123` 的 `Editor` 角色：

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

更新用户策略以授予 `name@example.com` 对标识为 `dda27e49d2a1efca58083a01dfde18f6` 的资源组的 `Operator` 角色：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

更新用户策略以授予 `name@example.com` 对资源组 `sample-resource-group` 的成员的 `Viewer` 角色：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

更新用户策略以授予 `name@example.com` 对标识为 `dda27e49d2a1efca58083a01dfde18f6` 的资源组成员的 `Viewer` 角色：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

列出指定服务的所有服务策略

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必需）</dt>
  <dd>服务标识的名称</dd>
  <dt>-json</dt>
  <dd>以 JSON 格式显示策略</dd>
  <dt>-f, --force</dt>
  <dd>显示服务策略而不确认</dd>
</dl>

<strong>示例</strong>：

列出服务 `test` 的策略：

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

显示服务策略的详细信息

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必需）</dt>
  <dd>服务标识的名称</dd>
  <dt>POLICY_ID（必需）</dt>
  <dd>服务策略的标识<dd>
  <dt>-json</dt>
  <dd>以 JSON 格式显示策略</dd>
  <dt>-f, --force</dt>
  <dd>显示服务策略而不确认</dd>
</dl>

<strong>示例</strong>：

显示服务 `test` 的策略 `140798e2-8ea7db3`：

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

创建服务策略

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必需）</dt>
  <dd>服务标识的名称</dd>
  <dt>-f, --file</dt>
  <dd>策略定义的 JSON 文件。此项与“-r, --roles”、“--service-name”、“--service-instance”、“--region”、“--resource-type”和“--resource”标志互斥。</dd>
  <dt>-r, --roles</dt>
  <dd>策略定义的角色名称。要了解某个服务所支持的角色，请运行“bluemix iam roles --service SERVICE_NAME”。此选项与“-f, --file”互斥。</dd>
  <dt>-service-name</dt>
  <dd>策略定义的服务名称。此项与“-f, --file”标志互斥。</dd>
  <dt>-service-instance</dt>
  <dd>策略定义的服务实例。此项与“-f, --file”标志互斥。</dd>
  <dt>-region</dt>
  <dd>策略定义的区域。此项与“-f, --file”标志互斥。</dd>
  <dt>-resource-type</dt>
  <dd>策略定义的资源类型。此项与“-f, --file”标志互斥。</dd>
  <dt>-resource</dt>
  <dd>策略定义的资源。此项与“-f, --file”标志互斥。</dd>
  <dt>-F, --force</dt>
  <dd>创建服务策略而不确认</dd>
</dl>

<strong>示例</strong>：

通过 JSON 文件为服务 `test` 创建服务策略：

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

更新服务策略

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必需）</dt>
  <dd>服务标识的名称</dd>
  <dt>POLICY_ID（必需）</dt>
  <dd>服务策略的标识<dd>
  <dt>-v, --version</dt>
  <dd>服务策略的版本</dd>
  <dt>-f, --file</dt>
  <dd>策略定义的 JSON 文件。此项与“-r, --roles”、“--service-name”、“--service-instance”、“--region”、“--resource-type”和“--resource”标志互斥。</dd>
  <dt>-r, --roles</dt>
  <dd>策略定义的角色名称。要了解某个服务所支持的角色，请运行“bluemix iam roles --service SERVICE_NAME”。此选项与“-f, --file”互斥。</dd>
  <dt>-service-name</dt>
  <dd>策略定义的服务名称。此项与“-f, --file”标志互斥。</dd>
  <dt>-service-instance</dt>
  <dd>策略定义的服务实例。此项与“-f, --file”标志互斥。</dd>
  <dt>-region</dt>
  <dd>策略定义的区域。此项与“-f, --file”标志互斥。</dd>
  <dt>-resource-type</dt>
  <dd>策略定义的资源类型。此项与“-f, --file”标志互斥。</dd>
  <dt>-resource</dt>
  <dd>策略定义的资源。此项与“-f, --file”标志互斥。</dd>
  <dt>-F, --force</dt>
  <dd>更新服务策略而不确认</dd>
</dl>

<strong>示例</strong>：

通过 JSON 文件更新服务 `test` 的服务策略 `140798e2-8ea7db3`：

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

删除服务策略

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>SERVICE_ID_NAME（必需）</dt>
  <dd>服务标识的名称</dd>
  <dt>POLICY_ID（必需）</dt>
  <dd>服务策略的标识<dd>
  <dt>-f, --force</dt>
  <dd>删除而不确认</dd>
</dl>

<strong>示例</strong>：

删除服务 `test` 的策略 `140798e2-8ea7db3`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

列出资源组

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>--default</dt>
  <dd>获取当前帐户的缺省组</dd>
  <dt>-r, --resource</dt>
  <dd>所属资源的标识</dd>
  <dt>-o, --resource-origin</dt>
  <dd>所属资源的来源。接受的值：“CF_ORG”和“IMS_ACCOUNT”。</dd>
</dl>

<strong>示例</strong>：

列出当前目标帐户下的所有资源组：

```
bluemix resource groups
```

列出当前目标帐户的缺省组：

```
bluemix resource groups --default
```

列出作为 Cloud Foundry 组织映射的资源组

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

显示资源组的详细信息

```
bluemix resource group NAME [--id]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>资源组的名称</dd>
  <dt>--id</dt>
  <dd>仅显示标识</dd>
</dl>

<strong>示例</strong>：

显示资源组 `example-group`：

```
bluemix resource group example-group
```

仅显示资源组 `example-group` 的标识：

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

更新现有资源组

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>目标资源组的名称</dd>
  <dt>-n, --name</dt>
  <dd>资源组的新名称</dd>
  <dt>-q, --quota</dt>
  <dd>新配额定义的名称</dd>
  <dt>-f</dt>
  <dd>强制更新而不确认</dd>
</dl>

<strong>示例</strong>：

将资源组 `example-group` 重命名为 `trial-group`：

```
bluemix resource group-update example-group -n trial-group
```

将资源组 `example-group` 的配额更改为 `free`：

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

列出所有配额定义

```
bluemix resource quotas
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
</dl>

<strong>示例</strong>：

列出所有配额定义：

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

显示配额定义的详细信息

```
bluemix resource quota NAME
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>配额的名称</dd>
</dl>

<strong>示例</strong>：显示配额 `free` 的详细信息：

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

此命令的功能和选项与 `cf push` 命令的相同。


## bluemix app list
{: #bluemix_app_list}

此命令的功能和选项与 `cf apps` 命令的相同。


## bluemix app show
{: #bluemix_app_show}

此命令的功能和选项与 `cf app` 命令的相同。


## bluemix app delete
{: #bluemix_app_delete}

此命令的功能和选项与 `cf delete` 命令的相同。


## bluemix app rename
{: #bluemix_app_rename}

此命令的功能和选项与 `cf rename` 命令的相同。


## bluemix app start
{: #bluemix_app_start}

此命令的功能和选项与 `cf start` 命令的相同。


## bluemix app stop
{: #bluemix_app_stop}

此命令的功能和选项与 `cf stop` 命令的相同。


## bluemix app restart
{: #bluemix_app_restart}

此命令的功能和选项与 `cf restart` 命令的相同。


## bluemix app restage
{: #bluemix_app_restage}


此命令的功能和选项与 `cf restage` 命令的相同。


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


此命令的功能和选项与 `cf restart-app-instance` 命令的相同。


## bluemix app events
{: #bluemix_app_events}

此命令的功能和选项与 `cf events` 命令的相同。


## bluemix app files
{: #bluemix_app_files}

此命令的功能和选项与 `cf files` 命令的相同。


## bluemix app logs
{: #bluemix_app_logs}

此命令的功能和选项与 `cf logs` 命令的相同。


## bluemix app env
{: #bluemix_app_env}

此命令的功能和选项与 `cf env` 命令的相同。


## bluemix app env-set
{: #bluemix_app_env_set}

此命令的功能和选项与 `cf set-env` 命令的相同。


## bluemix app env-unset
{: #bluemix_app_env_unset}

此命令的功能和选项与 `cf unset-env` 命令的相同。


## bluemix app stacks
{: #bluemix_app_stacks}

此命令的功能和选项与 `cf stacks` 命令的相同。


## bluemix app stack-show
{: #bluemix_app_stack_show}

此命令的功能和选项与 `cf stack` 命令的相同。


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

此命令的功能和选项与 `cf create-app-manifest` 命令的相同。

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

列出域的证书信息。

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
<dl>
<dt>DOMAIN_NAME（必需）</dt>
<dd>托管证书的域。</dd>
</dl>


<strong>示例</strong>：

查看域 `ibmcxo-eventconnect.com` 的证书信息：

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

将证书添加到当前组织中的指定域。

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
   <dl>
   <dt>DOMAIN（必需）</dt>
   <dd>将证书添加到其中的域。</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i>（必需）</dt>
   <dd>专用密钥文件路径。</dd>
   <dt>-c <i>CERT_FILE</i>（必需）</dt>
   <dd>证书文件路径。</dd>
   <dt>-p <i>PASSWORD</i>（可选）</dt>
   <dd>证书的密码。</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i>（可选）</dt>
   <dd>中间证书文件路径。</dd>
   <dt>-t <i>TRUST_STORE_FILE</i>（可选）</dt>
   <dd>信任库文件。</dd>
   </dl>


<strong>示例</strong>：

将证书添加到域 `ibmcxo-eventconnect.com`：

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

从当前组织中的指定域除去证书。

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：

   <dl>
   <dt>DOMAIN（必需）</dt>
   <dd>要从中除去证书的域。</dd>
   <dt>-f（可选）</dt>
   <dd>强制删除而不确认。</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

此命令的功能和选项与 `cf domains` 命令的相同。


## bluemix app domain-create
{: #bluemix_app_domain_create}

此命令的功能和选项与 `cf create-domain` 命令的相同。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

此命令的功能和选项与 `cf delete-domain` 命令的相同。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

此命令的功能和选项与 `cf create-shared-domain` 命令的相同。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

此命令的功能和选项与 `cf delete-shared-domain` 命令的相同。

## bluemix app routes
{: #bluemix_app_routes}

此命令的功能和选项与 `cf routes` 命令的相同。


## bluemix app route-check
{: #bluemix_app_route_check}

此命令的功能和选项与 `cf check-route` 命令的相同。


## bluemix app route-map
{: #bluemix_app_route_map}

将路径映射到具有指定域和主机名的现有 cf 应用程序或容器组。

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME（必需）</dt>
   <dd>要使用路径映射到的 cf 应用程序或容器组的名称。</dd>
   <dt>DOMAIN（必需）</dt>
   <dd>路径的域。例如，mychinabluemix.net 或 chinabluemix.net。</dd>
   <dt>-n <i>HOST_NAME</i>（可选）</dt>
   <dd>路径的主机名。如果未提供，缺省情况下主机名将设置为应用程序名称或容器组名称。</dd>
   </dl>

<strong>示例</strong>：

使用指定的域将路径映射到 `my-app`：

```
bluemix app route-map my-app mychinabluemix.net
```

使用指定域和主机名将路径映射到“my-container-group”：

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

取消来自现有 cf 应用程序或容器组中的指定路径映射。

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME（必需）</dt>
   <dd>cf 应用程序或容器组的名称。</dd>
   <dt>DOMAIN（必需）</dt>
   <dd>路径的域（例如，mychinabluemix.net 或 chinabluemix.net）。</dd>
   <dt>-n <i>HOST_NAME</i>（可选）</dt>
   <dd>路径的主机名。如果未提供，缺省情况下主机名将设置为应用程序名称或容器组名称。</dd>
   </dl>

<strong>示例</strong>：

从 `my-app` 取消 `my-app.mychinabluemix.net` 的映射：

```
bluemix app route-unmap my-app mychianbluemix.net
```

从 `my-container-group` 取消 `abc.chinabluexmix.net` 的映射：

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

此命令的功能和选项与 `cf create-route` 命令的相同。


## bluemix app route-delete
{: #bluemix_app_route_delete}

此命令的功能和选项与 `cf delete-route` 命令的相同。


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

此命令的功能和选项与 `cf delete-orphaned-routes` 命令的相同。


## bluemix app domains
{: #bluemix_app_domains}

此命令的功能和选项与 `cf domains` 命令的相同。


## bluemix app domain-create
{: #bluemix_app_domain_create}

此命令的功能和选项与 `cf create-domain` 命令的相同。


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

此命令的功能和选项与 `cf delete-domain` 命令的相同。


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

此命令的功能和选项与 `cf create-shared-domain` 命令的相同。


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

此命令的功能和选项与 `cf delete-shared-domain` 命令的相同。


## bluemix service offerings
{: #bluemix_service_offerings}


此命令的功能和选项与 `cf marketplace` 命令的相同。


## bluemix service list
{: #bluemix_service_list}

此命令的功能和选项与 `cf services` 命令的相同。


## bluemix service show
{: #bluemix_service_show}

此命令的功能和选项与 `cf service` 命令的相同。


## bluemix service create
{: #bluemix_service_create}

此命令的功能和选项与 `cf create-service` 命令的相同。


## bluemix service update
{: #bluemix_service_update}

此命令的功能和选项与 `cf update-service` 命令的相同。


## bluemix service delete
{: #bluemix_service_delete}

此命令的功能和选项与 `cf delete-service` 命令的相同。


## bluemix service rename
{: #bluemix_service_rename}

此命令的功能和选项与 `cf rename-service` 命令的相同。


## bluemix service bind
{: #bluemix_service_bind}

此命令的功能和选项与 `cf bind-service` 命令的相同。


## bluemix service unbind
{: #bluemix_service_unbind}

此命令的功能和选项与 `cf unbind-service` 命令的相同。


## bluemix service key-create
{: #bluemix_service_key_create}

此命令的功能和选项与 `cf create-service-key` 命令的相同。


## bluemix service key-delete
{: #bluemix_service_key_delete}

此命令的功能和选项与 `cf delete-service-key` 命令的相同。


## bluemix service keys
{: #bluemix_service_keys}

此命令的功能和选项与 `cf service-keys` 命令的相同。


## bluemix service key-show
{: #bluemix_service_key_show}

此命令的功能和选项与 `cf service-key` 命令的相同。


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

此命令的功能和选项与 `cf create-user-provided-service` 命令的相同。


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

此命令的功能和选项与 `cf update-user-provided-service` 命令的相同。


## bluemix resource instances
{: #bluemix_resource_instances}

列出资源实例

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>--resource-name</dt>
  <dd>所属资源的名称</dd>
  <dt>-r, --region</dt>
  <dd>按区域标识过滤，如果未指定，将缺省为当前区域；使用“-r, --region all” 可显示所有区域下的资源实例</dd>
  <dt>--long</dt>
  <dd>在输出中显示更多字段</dd>
</dl>

<strong>示例</strong>：

列出资源 `test-resource` 的资源实例：

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

显示资源实例的详细信息

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>资源实例的名称</dd>
  <dt>-r, --region</dt>
  <dd>按区域标识过滤，如果未指定，将缺省为当前区域；使用“-r, --region all” 可显示所有区域下的资源实例</dd>
  <dt>--id</dt>
  <dd>显示资源实例的标识</dd>
</dl>

<strong>示例</strong>：显示资源实例 `my-resource-instance` 的详细信息：

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

创建资源实例

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME（必需）</dt>
  <dd>资源实例的名称</dd>
  <dt>RESOURCE_NAME 或 RESOURCE_ID（必需）</dt>
  <dd>资源的名称或标识</dd>
  <dt>RESOURCE_PLAN_NAME 或 RESOURCE_PLAN_ID（必需）</dt>
  <dd>资源套餐的名称或标识</dd>
  <dt>-r, --region</dt>
  <dd>要创建资源实例的区域，如果未指定，将缺省为当前区域</dd>
  <dt>-t, --tags</dt>
  <dd>标记</dd>
  <dt>-p, --parameters</dt>
  <dd>用于创建资源实例的 JSON 文件或 JSON 字符串</dd>
</dl>

<strong>示例</strong>：使用资源 `test-resource` 的资源套餐 `test-resource-plan` 创建名为 `my-resource-instance` 的资源实例：

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

更新资源实例

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>RESOURCE_INSTANCE_NAME（必需）</dt>
  <dd>资源实例的名称</dd>
  <dt>-n, --name</dt>
  <dd>新资源实例名称</dd>
  <dt>-t, --tags</dt>
  <dd>新标记</dd>
  <dt>--resource-plan-id</dt>
  <dd>新资源套餐标识</dd>
  <dt>--update-time</dt>
  <dd>从可收费记录应生效时起到现在的时间（以秒计）</dd>
  <dt>-f, --force</dt>
  <dd>强制更新而不确认</dd>
</dl>

<strong>示例</strong>：更新资源实例 `my-resource-instance`，以将其名称更改为 `new-resource-instance`：

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

删除资源实例

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-f, --force</dt>
  <dd>强制删除而不确认</dd>
</dl>

<strong>示例</strong>：删除资源实例 `my-resource-instance`：

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

显示与资源别名的绑定

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>RESOURCE_ALIAS（必需）</dt>
  <dd>资源别名</dd>
</dl>

<strong>示例</strong>：显示与资源别名 `my-resource-alias` 的资源绑定：

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

显示资源绑定的详细信息

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 应用程序名称</dd>
  <dt>--id</dt>
  <dd>仅显示标识。将禁止资源绑定的所有其他输出。</dd>
</dl>

<strong>示例</strong>：显示资源别名 `my-resource-alias` 和应用程序 `my-app` 之间的资源绑定的详细信息：

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

创建资源绑定

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>RESOURCE_ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 应用程序名称</dd>
  <dt>ROLE_NAME</dt>
  <dd>用户角色的名称</dd>
  <dt>--service-id-name</dt>
  <dd>角色所属的服务标识的名称</dd>
  <dt>-f, --force</dt>
  <dd>强制创建而不确认</dd>
</dl>

<strong>示例</strong>：使用角色 `Administrator` 创建资源别名 `my-resource-alias`和应用程序 `my-app` 之间的资源绑定：

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

删除资源绑定

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
<dl>
  <dt>RESOURCE_ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry 应用程序名称</dd>
  <dt>-f, --force</dt>
  <dd>强制删除而不确认</dd>
</dl>

<strong>示例</strong>：删除资源别名 `my-resource-alias` 和应用程序 `my-app` 之间的资源绑定：

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

列出资源实例或资源别名的资源键

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>--instance-id</dt>
  <dd>资源实例标识</dd>
  <dt>--instance-name</dt>
  <dd>资源实例名称</dd>
  <dt>--alias-id</dt>
  <dd>资源别名标识</dd>
  <dt>--alias-name</dt>
  <dd>资源别名</dd>
</dl>

<strong>示例</strong>：列出资源实例 `my-resource-instance` 的资源键：

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

显示资源键的详细信息

```
bluemix resource key KEY_NAME [--id]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>KEY_NAME</dt>
  <dd>键的名称</dd>
  <dt>--id</dt>
  <dd>显示资源键的标识</dd>
</dl>

<strong>示例</strong>：显示资源键 `my-resource-key` 的详细信息：

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

创建资源键

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>NAME</dt>
  <dd>键的名称</dd>
  <dt>ROLE_NAME</dt>
  <dd>用户角色的名称</dd>
  <dt>--instance-id</dt>
  <dd>资源实例标识</dd>
  <dt>--instance-name</dt>
  <dd>资源实例名称</dd>
  <dt>--alias-id</dt>
  <dd>资源别名标识</dd>
  <dt>--alias-name</dt>
  <dd>资源别名</dd>
  <dt>-service-id-name</dt>
  <dd>角色所属的服务标识的名称</dd>
  <dt>-f, --force</dt>
  <dd>强制创建而不确认</dd>
</dl>

<strong>示例</strong>：使用角色 `Administrator` 为资源实例 `my-resource-instance` 创建名为 `my-resource-key` 的资源键：

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

删除资源键

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>KEY_NAME</dt>
  <dd>键的名称</dd>
  <dt>-f, --force</dt>
  <dd>强制删除而不确认</dd>
</dl>

<strong>示例</strong>：删除资源键 `my-resource-key`：

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

列出资源实例的别名

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>--instance-id</dt>
  <dd>所属资源实例的标识。</dd>
  <dt>--instance-name</dt>
  <dd>所属资源实例的名称。</dd>
</dl>

<strong>示例</strong>：列出资源实例 `my-resource-instance` 的资源别名：
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

显示资源别名的详细信息

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>--id</dt>
  <dd>仅显示给定资源别名的标识。将禁止别名的所有其他输出。</dd>
</dl>

<strong>示例</strong>：显示资源别名 `my-resource-alias` 的详细信息：
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

创建资源实例的别名

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>--instance-id</dt>
  <dd>所属资源实例的标识。</dd>
  <dt>--instance-name</dt>
  <dd>所属资源实例的名称。</dd>
  <dt>-s</dt>
  <dd>在其中创建别名的空间的名称。缺省值为当前空间。</dd>
  <dt>-t, --tags</dt>
  <dd>标记列表。</dd>
  <dt>-p, --parameters</dt>
  <dd>参数 JSON 文件或 JSON 字符串。</dd>
</dl>

<strong>示例</strong>：创建资源实例 `my-resource-instance` 的资源别名 `my-resource-alias`：
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

更新资源别名

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>-n, --name</dt>
  <dd>资源别名的新名称。</dd>
  <dt>-t, --tags</dt>
  <dd>标记列表。</dd>
  <dt>-p, --parameters</dt>
  <dd>参数 JSON 文件或 JSON 字符串。</dd>
  <dt>-f, --force</dt>
  <dd>强制更新而无需用户确认。</dd>
</dl>

<strong>示例</strong>：更新资源别名 `my-resource-alias`，以将其名称更改为 `new-resource-alias`：

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

删除资源别名

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>ALIAS_NAME（必需）</dt>
  <dd>资源别名</dd>
  <dt>-f, --force</dt>
  <dd>强制删除而不确认</dd>
</dl>

<strong>示例</strong>：删除资源别名 `my-resource-alias`：

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

搜索目录条目

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-q, --query</dt>
  <dd>搜索关键字</dd>
  <dt>-r, --region</dt>
  <dd>指定要在其中进行搜索的地理区域。目前仅支持“us-south”和“united-kingdom”</dd>
  <dt>-k, --kind</dt>
  <dd>按资源种类过滤。目前仅支持“service-cf”、“iaas”、“runtime”、“template”和“dashboard”</dd>
  <dt>-p, --price</dt>
  <dd>按价格过滤。目前仅支持“free”、“paygo”和“bluemix-subscription”</dd>
  <dt>-t, --tag</dt>
  <dd>按标记过滤。</dd>
  <dt>-sort-by</dt>
  <dd>要作为排序依据的属性</dd>
  <dt>-reverse</dt>
  <dd>是否反转排序顺序</dd>
  <dt>-json</dt>
  <dd>输出原始 JSON 响应</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

搜索服务 `Automation test`：

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

获取目录条目

```
bluemix catalog entry [-i ID] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>目录条目的标识。</dd>
  <dt>-children</dt>
  <dd>获取目录条目的所有子代</dd>
  <dt>-json</dt>
  <dd>输出原始 JSON 响应</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

获取标识为 `a0ef1-d3b4j0` 的条目：

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
创建新的目录条目（仅限帐户的目录管理员）

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-p, --parent</dt>
  <dd>对象的父标识</dd>
  <dt>-c</dt>
  <dd>包含特定于目录的配置参数的有效 JSON 对象，以内联方式或文件形式提供。要获取受支持的配置参数的列表，请参阅特定目录条目的文档。</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

通过 JSON 文件创建父标识为 `a0ef1-d3b4j0` 资源：

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
更新现有目录条目（仅限帐户的目录管理员或编辑者）

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>正在更新的目录条目的标识。</dd>
  <dt>-c</dt>
  <dd>包含特定于目录的配置参数的有效 JSON 对象，以内联方式或文件形式提供。要获取受支持的配置参数的列表，请参阅特定目录条目的文档。</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

通过 JSON 文件更新资源 `j402-dnf1i`：

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
获取目录条目的可视性（仅限帐户的目录管理员）

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>目录条目的标识。</dd>
  <dt>-json</dt>
  <dd>输出原始 JSON 响应</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

获取资源 `j402-dnf1i` 在全球范围的可视性：

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
更新现有目录条目的可视性（仅限帐户的目录管理员）

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-i, --id</dt>
  <dd>正在更新的目录条目的标识。</dd>
  <dt>-c</dt>
  <dd>包含特定于目录的配置参数的有效 JSON 对象，以内联方式或文件形式提供。要获取受支持的配置参数的列表，请参阅特定目录条目的文档。</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

通过 JSON 文件设置资源 `j402-dnf1i` 的可视性：

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
列出市场中的服务产品

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
<dl>
  <dt>-cf</dt>
  <dd>仅显示 Cloud Foundry 服务</dd>
  <dt>-rc</dt>
  <dd>仅显示 RC 兼容服务</dd>
  <dt>-global</dt>
  <dd>在全球范围运行</dd>
</dl>

<strong>示例</strong>：

显示全球范围的服务产品：

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

查看 Bluemix 上的样板模板。

```
bluemix catalog templates [-d]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

   <dl>
   <dt>-d（可选）</dt>
   <dd>如果指定了 <i>-d</i> 选项，那么还会显示每个模板的描述。否则，只显示每个模板的标识和名称。</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

查看指定样板模板的详细信息。

```
bluemix catalog template TEMPLATE_ID
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：
   <dl>
   <dt>TEMPLATE_ID（必需）</dt>
   <dd>样板模板的标识。使用 <i>bluemix templates</i> 可查看所有模板的标识。</dd>
   </dl>


<strong>示例</strong>：

查看模板 `mobileBackendStarter` 的详细信息：

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

使用指定 URL 和描述基于指定模板创建 cf 应用程序。缺省情况下，新应用程序将自动启动。

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>先决条件</strong>：端点、登录和目标

<strong>命令选项</strong>：
   <dl>
   <dt>TEMPLATE_ID（必需）</dt>
   <dd>创建应用程序时将基于的模板。使用 <i>bluemix templates</i> 可查看所有模板的标识。</dd>
   <dt>CF_APP_NAME（必需）</dt>
   <dd>要创建的 cf 应用程序的名称。</dd>
   <dt>-u <i>URL</i>（可选）</dt>
   <dd>应用程序的路径。如果未指定，Bluemix 将基于应用程序名称和缺省域自动设置路径。</dd>
   <dt>-d <i>DESCRIPTION</i>（可选）</dt>
   <dd>应用程序的描述。</dd>
   <dt>--no-start（可选）</dt>
   <dd>应用程序创建后不自动启动。如果未指定，应用程序创建后将自动启动。</dd>
   </dl>


<strong>示例</strong>：

基于 `javaHelloWorld` 模板创建 cf 应用程序 `my-app`：

```
bluemix catalog template-run javaHelloWorld my-app
```

基于 `rubyHelloWorld` 模板创建应用程序 `my-ruby-app`，路径为 `myrubyapp.chinabluemix.net`，描述为 `My first ruby app on {{site.data.keyword.Bluemix_notm}}.`：

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

基于 `pythonHelloWorld` 模板创建应用程序 `my-python-app`，不带自动启动：

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

显示帐户的每月使用情况和成本。

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

<dl>
  <dt>-d MONTH_DATE（可选）</dt>
  <dd>显示使用 YYYY-MM 格式指定的月份和日期的数据。如果未指定，那么会显示当月的使用情况。</dd>
  <dt>--json（可选）</dt>
  <dd>以 JSON 格式显示使用情况结果。</dd>
</dl>

<strong>示例</strong>：

显示 2016 年 6 月我的帐户的使用情况和成本报告：

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

显示组织的每月使用情况详细信息。此操作只能由组织的记帐管理员执行。

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

<dl>
  <dt>ORG_NAME（必需）</dt>
  <dd>组织的名称。</dd>
  <dt>-d MONTH_DATE（可选）</dt>
  <dd>显示使用 YYYY-MM 格式指定的月份和日期的数据。如果未指定，那么会显示当月的使用情况。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>托管组织的区域名称。如果设置为“all”，那么会显示所有区域中的组织使用情况。</dd>
  <dt>--json（可选）</dt>
  <dd>以 JSON 格式显示使用情况结果。</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

显示我的帐户中组织的每月使用情况摘要。

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>先决条件</strong>：端点和登录

<strong>命令选项</strong>：

<dl>
  <dt>-d MONTH_DATE（可选）</dt>
  <dd>显示使用 YYYY-MM 格式指定的月份和日期的数据。如果未指定，那么会显示当月的使用情况。</dd>
  <dt>-r REGION_NAME</dt>
  <dd>托管组织的区域的名称。如果设置为“all”，那么会显示所有区域中组织的使用情况摘要。</dd>
  <dt>--json（可选）</dt>
  <dd>以 JSON 格式显示使用情况结果。</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

列出 {{site.data.keyword.Bluemix_notm}} CLI 中注册的所有插件存储库。

```
bluemix plugin repos
```

<strong>先决条件</strong>：无


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

将新的插件存储库添加到 {{site.data.keyword.Bluemix_notm}} CLI 中。

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>REPO_NAME（必需）</dt>
   <dd>要添加的存储库的名称。可以为每个存储库定义您自己的名称。</dd>
   <dt>REPO_URL（必需）</dt>
   <dd>要添加的存储库的 URL。存储库 URL 必须包含协议（例如，http://plugins.ng.bluemix.net，而不是 plugins.ng.bluemix.net）。http://plugins.ng.bluemix.net 是 Bluemix CLI 的官方插件存储库。</dd>
    </dl>


<strong>示例</strong>：

将 Bluemix CLI 的官方插件存储库添加为 `bluemix-repo`：

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

从 {{site.data.keyword.Bluemix_notm}} CLI 中除去插件存储库。

```
bluemix plugin repo-remove REPO_NAME
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
   <dl>
   <dt>REPO_NAME（必需）</dt>
   <dd>要除去的存储库的名称。</dd>
   </dl>

<strong>示例</strong>：

从 {{site.data.keyword.Bluemix_notm}} CLI 中除去 `bluemix-repo` 存储库：

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

列出所有添加的存储库或特定存储库中的所有可用插件。

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>-r <i>REPO_NAME</i>（可选）</dt>
   <dd>仅列出指定存储库中的插件。</dd>
   </dl>

<strong>示例</strong>：

列出所有添加的存储库中的所有插件：

```
bluemix plugin repo-plugins
```

列出 `bluemix-repo` 存储库中的所有插件：

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

显示存储库中插件的详细信息。

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>-r <i>REPO_NAME</i>（可选）</dt>
   <dd>存储库的名称。如果未指定存储库，此命令将使用缺省插件存储库。</dd>
   </dl>

<strong>示例</strong>：

列出存储库“sample-repo”中插件“IBM-Containers”的详细信息：

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

列出缺省存储库中插件“IBM-Containers”的详细信息

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

列出 {{site.data.keyword.Bluemix_notm}} CLI 中的所有已安装插件。

```
bluemix plugin list
```

<strong>先决条件</strong>：无

## bluemix plugin show
{: #bluemix_plugin_show}

显示已安装插件的详细信息

```
bluemix plugin show PLUGIN-NAME
```

<strong>先决条件</strong>：无


## bluemix plugin install
{: #bluemix_plugin_install}

从指定的路径或存储库将特定版本的插件安装到 {{site.data.keyword.Bluemix_notm}} CLI 中。

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME（必需）</dt>
   <dd>如果未指定 -r <i>REPO_NAME</i>，那么将从指定的本地路径或远程 URL 安装插件。</dd>
   <dt>-r <i>REPO_NAME</i>（可选）</dt>
   <dd>插件二进制文件所在的存储库的名称。如果未指定存储库，此命令将使用缺省插件存储库。</dd>
   <dt>-v <i>VERSION</i>（可选）</dt>
   <dd>要安装的插件的版本。如果未提供，将安装插件的最新版本。此选项仅对从存储库安装插件有效。</dd>
    </dl>

<strong>示例</strong>：

从本地文件安装插件：

```
bluemix plugin install /downloads/new_plugin
```

从远程 URL 安装插件：

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

从 `bluemix-repo` 存储库安装最新版本的 `IBM-Containers` 插件：

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
从 `bluemix-repo` 存储库安装版本为 `0.5.800` 的 `IBM-Containers` 插件：

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

升级存储库中的插件

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>要更新的插件的名称。如果未指定，此命令将检查安装的所有插件的升级。</dd>
 <dt>-r REPO_NAME</dt>
 <dd>插件二进制文件所在的存储库的名称。如果未指定，此命令将使用缺省插件存储库。</dd>
 <dt>-v <i>VERSION</i>（可选）</dt>
 <dd>要更新到的插件版本。如果未提供，那么将插件更新到最新可用版本。</dd>
 <dt>--all</dt>
 <dd>更新所有可用的插件</dd>
</dl>

<strong>示例</strong>：

检查插件存储库“My-Repo”中所有可用的升级：

```
bluemix plugin update -r My-Repo
```

将存储库“My-Repo”中的插件“plugin-echo”升级到最新版本：

```
bluemix plugin update -r My-Repo plugin-echo
```

将存储库“My-Repo”中的插件“plugin-echo”升级到版本“1.0.1”：

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

从 {{site.data.keyword.Bluemix_notm}} CLI 中卸载指定的插件。

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>先决条件</strong>：无

<strong>命令选项</strong>：

   <dl>
   <dt>PLUGIN_NAME（必需）</dt>
   <dd>要卸载的插件的名称。</dd>
    </dl>

<strong>示例</strong>：

卸载先前安装的 `IBM-Containers` 插件：

```
bluemix plugin uninstall IBM-Containers
```

