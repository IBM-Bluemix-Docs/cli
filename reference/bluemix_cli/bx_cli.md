---



copyright:

  years: 2015, 2017
lastupdated: "2017-11-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.Bluemix_notm}} (bx) commands
{: #bluemix_cli}

Version: 0.6.2

The {{site.data.keyword.Bluemix_notm}} command line interface (CLI) provides a set of commands that are grouped by namespace for users to interact with {{site.data.keyword.Bluemix_notm}}.

Starting from version 0.5.0, {{site.data.keyword.Bluemix_notm}} command line client bundles a Cloud Foundry command line client in its installation. If you have your own cf cli installed, do not use both {{site.data.keyword.Bluemix_notm}} CLI commands `bx [command]` and Cloud Foundry CLI commands `cf [command]` of your own installation in the same context. Instead, use `bluemix cf [command]` if you want to use cf cli to manage Cloud Foundry resources in {{site.data.keyword.Bluemix_notm}} CLI context.  Note that `bluemix cf api/login/logout/target` is not allowed, and you must use `bluemix api/login/logout/target` instead.

The following lists detailed commands that are supported by {{site.data.keyword.Bluemix_notm}} CLI, including their names, arguments, options, prerequisites, descriptions, and examples.
{:shortdesc}

**Note:** *Prerequisites* list which actions are required before using the command. Commands that have no prerequisite actions list **None**. Otherwise, prerequisites might include one or more of the following actions:

<dl>
<dt>Endpoint</dt>
<dd>An API endpoint must be set through the <code>bluemix api</code> before using the command.</dd>
<dt>Login</dt>
<dd>Login by using the <code>bluemix login</code> command is required before using this command.
If logging in with federated ID, use '--sso' option to authenticate with one time passcode, or use '--apikey' to authenticate with API key. Go to {{site.data.keyword.Bluemix_notm}} console **Manage** &gt; **Security** &gt; **Platform API keys** to create API keys.
</dd>
<dt>Target</dt>
<dd>The <code>bluemix target</code> command must be used to set an org and space before using this command.</dd>
<dt>Docker</dt>
<dd>The Docker CLI (docker) must be installed to run this command.</dd>
</dl>

**Note:** You can use the short format of bluemix commands; for example, `bx api` is short for `bluemix api`.

Use the indexes in the following tables to refer to the frequently used bluemix commands.

## General bluemix commands
{: #bx_commands_index}

<table summary="General bluemix commands.">
<caption>Table 1. General bluemix commands</caption>
 <thead>
 <th colspan="5">General bluemix commands</th>
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

 ## Commands for managing and configuring {{site.data.keyword.BluSoftlayer_notm}} infrastructure services (bluemix sl)
  {: #bx_commands_softlayer}

The commands for managing {{site.data.keyword.BluSoftlayer_notm}} infrastructure have been merged into the {{site.data.keyword.Bluemix_notm}} CLI. For more information on using the {{site.data.keyword.Bluemix_notm}} CLI to configure and manage {{site.data.keyword.BluSoftlayer_notm}} infrastructure services, see: [{{site.data.keyword.Bluemix_notm}} CLI {{site.data.keyword.BluSoftlayer_notm}} infrastructure (bluemix sl) commands](/docs/cli/reference/softlayer/index.md#softlayer_cli).

 ## Commands for managing accounts, orgs, and roles
 {: #bx_commands_account}

<table summary="bluemix commands that you can use to manage accounts, orgs, spaces and roles.">
<caption>Table 2. Commands for managing accounts, orgs, spaces and roles</caption>
 <thead>
 <th colspan="5">Commands for managing accounts, orgs, spaces, and roles</th>
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


 ## Commands for managing resource groups and resources
{: #bx_commands_resource}

<table summary="bluemix command that you can use to manage resource groups and resources.">
  <caption>Table 3. Commands for managing resource groups and resources</caption>
  <thead>
    <th colspan="5">Commands for managing resource groups and resources</th>
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
      <td>[bluemix resource service-instances](bx_cli.html#bluemix_resource_service_instances)</td>
      <td>[bluemix resource service-instance](bx_cli.html#bluemix_resource_service_instance)</td>
      <td>[bluemix resource service-instance-create](bx_cli.html#bluemix_resource_service_instance_create)</td>
      <td>[bluemix resource service-instance-update](bx_cli.html#bluemix_resource_service_instance_update)</td>
      <td>[bluemix resource service-instance-delete](bx_cli.html#bluemix_resource_service_instance_delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource service-bindings](bx_cli.html#bluemix_resource_service_bindings)</td>
      <td>[bluemix resource service-binding](bx_cli.html#bluemix_resource_service_binding)</td>
      <td>[bluemix resource service-binding-create](bx_cli.html#bluemix_resource_service_binding_create)</td>
      <td>[bluemix resource service-binding-delete](bx_cli.html#bluemix_resource_service_binding_delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource service-keys](bx_cli.html#bluemix_resource_service_keys)</td>
      <td>[bluemix resource service-key](bx_cli.html#bluemix_resource_service_key)</td>
      <td>[bluemix resource service-key-create](bx_cli.html#bluemix_resource_service_key_create)</td>
      <td>[bluemix resource service-key-delete](bx_cli.html#bluemix_resource_service_key_delete)</td>
    </tr>
    <tr>
      <td>[bluemix resource service-aliases](bx_cli.html#bluemix_resource_service_aliases)</td>
      <td>[bluemix resource service-alias](bx_cli.html#bluemix_resource_service_alias)</td>
      <td>[bluemix resource service-alias-create](bx_cli.html#bluemix_resource_service_alias_create)</td>
      <td>[bluemix resource service-alias-update](bx_cli.html#bluemix_resource_service_alias_update)</td>
      <td>[bluemix resource service-alias-delete](bx_cli.html#bluemix_resource_service_alias_delete)</td>
    </tr>
  </tbody>
</table>


 ## Commands for managing API keys and policies
 {: #bx_commands_iam}
 <table summary="bluemix commands that you can use to manage API keys and policies.">
 <caption>Table 3. Commands for managing API keys and policies</caption>
  <thead>
  <th colspan="5">Commands for managing API keys and policies</th>
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

 ## Commands for managing cf apps and app related domains, routes, and certificates
 {: #bx_commands_apps}

<table summary="bluemix commands that you can use to manage cf apps and app related domains, routes and certificates.">
<caption>Table 4. Commands for managing cf apps and app related domains, routes and certificates</caption>
 <thead>
 <th colspan="5">Commands for managing cf apps and app related domains, routes and certificates</th>
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

 ## Commands for managing {{site.data.keyword.Bluemix_notm}} services
 {: #bx_commands_services}

<table summary="bluemix commands that you can use to manage {{site.data.keyword.Bluemix_notm}} services.">
<caption>Table 5. Commands for managing {{site.data.keyword.Bluemix_notm}} services</caption>
 <thead>
 <th colspan="5">Commands for managing {{site.data.keyword.Bluemix_notm}} services</th>
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


 ## Commands for managing catalog, plug-ins, and billing settings
 {: #bx_commands_settings}

<table summary="bluemix commands that you can use to manage the {{site.data.keyword.Bluemix_notm}} catalog, plug-ins, billing, and security settings.">
<caption>Table 6. Commands for managing the {{site.data.keyword.Bluemix_notm}} catalog, plug-ins, billing, and security settings</caption>
 <thead>
 <th colspan="5">Commands for managing {{site.data.keyword.Bluemix_notm}} catalog, plug-ins, billing, and security settings</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix catalog search](bx_cli.html#bluemix_catalog_search)</td>
  <td>[bluemix catalog entry](bx_cli.html#bluemix_catalog_entry)</td>
  <td>[bluemix catalog entry-create](bx_cli.html#bluemix_catalog_entry_create)</td>
  <td>[bluemix catalog entry-update](bx_cli.html#bluemix_catalog_entry_update)</td>
  <td>[bluemix catalog entry-delete](bx_cli.html#bluemix_catalog_entry_delete)</td>
 </tr>
 <tr>
  <td>[bluemix catalog entry-visibility](bx_cli.html#bluemix_catalog_entry_visibility)</td>
  <td>[bluemix catalog service-marketplace](bx_cli.html#bluemix_catalog_service_marketplace)</td>
  <td>[bluemix catalog entry-visibility-set](bx_cli.html#bluemix_catalog_entry_visibility_set)</td>
  <td>[bluemix catalog templates](bx_cli.html#bluemix_catalog_templates)</td>
  <td>[bluemix catalog template](bx_cli.html#bluemix_catalog_template)</td>
 </tr>
 <tr>
  <td>[bluemix plugin repos](bx_cli.html#bluemix_plugin_repos)</td>
  <td>[bluemix plugin repo-add](bx_cli.html#bluemix_plugin_repo_add)</td>
  <td>[bluemix plugin repo-remove](bx_cli.html#bluemix_plugin_repo_remove)</td>
  <td>[bluemix plugin repo-plugins](bx_cli.html#bluemix_plugin_repo_plugins)</td>
 </tr>
 <tr>
  <td>[bluemix plugin repo-plugin](bx_cli.html#bluemix_plugin_repo_plugin)</td>
  <td>[bluemix plugin list](bx_cli.html#bluemix_plugin_list)</td>
  <td>[bluemix plugin install](bx_cli.html#bluemix_plugin_install)</td>
  <td>[bluemix plugin uninstall](bx_cli.html#bluemix_plugin_uninstall)</td>
  <td>[bluemix plugin update](bx_cli.html#bluemix_plugin_update)</td>
 </tr>
 <tr>
  <td>[bluemix billing account-usage](bx_cli.html#bluemix_billing_account_usage)</td>
  <td>[bluemix billing org-usage](bx_cli.html#bluemix_billing_org_usage)</td>
  <td>[bluemix billing orgs-usage-summary](bx_cli.html#bluemix_billing_orgs_usage_summary)</td>
 </tr>
 </tbody>
 </table>

## bluemix help
{: #bluemix_help}
Display the general help for first-level built-in commands and supported namespaces of {{site.data.keyword.Bluemix_notm}} CLI, or the help for a specific built-in command or namespace.

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>Prerequisites</strong>: None

<strong>Command options</strong>:

   <dl>
   <dt>COMMAND|NAMESPACE (optional)</dt>
   <dd>The command or namespace that help is displayed for. If not specified, the general help for {{site.data.keyword.Bluemix_notm}} CLI is shown.</dd>
   </dl>



<strong>Examples</strong>:

Display general help for {{site.data.keyword.Bluemix_notm}} CLI:

```
bluemix help
```

Display help for the `info` command:

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
Set or view the {{site.data.keyword.Bluemix_notm}} API endpoint.

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>Prerequisites</strong>: None

<strong>Command options</strong>:
   <dl>
   <dt>API_ENDPOINT (optional)</dt>
   <dd>The API endpoint that is targeted, for example, `https://api.chinabluemix.net`. If both *API_ENDPOINT* and `--unset` options are not specified, the current API endpoint is displayed.</dd>
   <dt>--unset (optional)</dt>
   <dd>Remove the API endpoint setting.</dd>
   <dt>--skip-ssl-validation (optional)</dt>
   <dd>Bypass SSL validation of HTTP requests.</dd>
   </dl>
<strong>Examples</strong>:

Set the API endpoint to api.chinabluemix.net:

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

View the current API endpoint:

```
bluemix api
```

Unset the API endpoint:

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


Write default values to the configuration file.

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>The timeout value for HTTP requests. The default value is 60 seconds.</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>Trace HTTP requests to the terminal or specified file.</dd>
   <dt>--color true|false</dt>
   <dd>Enable or disable color output. Color output is enabled by default.</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>Set a default locale. If LOCALE is <i>CLEAR</i>, the previous locale is deleted.</dd>
   <dt>--check-version true|false</dt>
   <dd>Enable or disable CLI version check.</dd>
   </dl>

Only one of these options can be specified at a time.

<strong>Examples</strong>:

Set HTTP request timeout to 30 seconds:

```
bluemix config --http-timeout 30
```

Enable trace output for HTTP requests:

```
bluemix config --trace true
```

Trace HTTP requests to a specified file */home/usera/my_trace*:

```
bluemix config --trace /home/usera/my_trace
```

Disable color output:

```
bluemix config --color false
```

Set the locale to zh_Hans:

```
bluemix config --locale zh_Hans
```

Clear the locale settings:

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

View the basic {{site.data.keyword.Bluemix_notm}} information, including the current region, the cloud controller version, and some useful endpoints, such as endpoints for login and exchanging access token.

```
bluemix info
```

<strong>Prerequisites</strong>:  Endpoint


## bluemix cf
{: #bluemix_cf}

Invoke embedded CF CLI

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:
<dl>
  <dt>-q, --quiet</dt>
  <dd>Turn off message "Invoking cf command..."</dd>
</dl>

<strong>Examples</strong>:

List cf apps:

```
bluemix cf apps
```

List cf services without message "Invoking cf command...":

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

Log in user.

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>Prerequisites</strong>:  None

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>Command options</strong>:
<dl>
  <dt> -a <i>API_ENDPOINT</i> (optional)</dt>
  <dd> API endpoint (For example: api.ng.bluemix.net)</dd>
  <dt> --apikey <i>API_KEY or @API_KEY_FILE_PATH</i>
  <dd> API key content or the path of an API key file indicated by @</dd>
  <dt> --sso (optional) </dt>
  <dd> Use a one-time passcode to login </dd>
  <dt> -u <i>USERNAME</i> (optional)</dt>
  <dd> Username</dd>
  <dt> -p <i>PASSWORD</i> (optional)</dt>
  <dd> Password</dd>
  <dt> -c <i>ACCOUNT_ID</i> (optional) </dt>
  <dd> ID of the target account</dd>
  <dt> -o <i>ORG_NAME</i> (optional) </dt>
  <dd> Name of the target organization </dd>
  <dt> -s <i>SPACE_NAME</i> (optional) </dt>
  <dd> Name of the target space</dd>
  <dt> --skip-ssl-validation (optional) </dt>
  <dd> Bypass SSL validation of HTTP requests. This option is not recommended.</dd>
</dl>

<strong>Examples</strong>:

#### Interactive login

```
bluemix login
```

Log in with user name and password, and set target account, org and space:

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

Log in with one time passcode and set target account, org and space

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

Log in with API key and set targets:

#### API key has account associated

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### API key has no account associated

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>Note:</strong> If the API Key has an associated account, switching to another account is not allowed.

#### Use one time passcode

```
bluemix login -u UserID --sso
```

Then the CLI will provide a URL link and ask for passcode:
```
One Time Code (Get one at https://URL_Link_To_Obtain_Passcode):
```

Open the link in browser, which will guide you to get the passcode. Type in the given passcode in console, and you should be able to login.

## bluemix logout
{: #bluemix_logout}

Log out user.

```
bluemix logout
```

<strong>Prerequisites</strong>:  None

## bluemix regions
{: #bluemix_regions}

View the information for all regions on {{site.data.keyword.Bluemix_notm}}.

```
bluemix regions
```

<strong>Prerequisites</strong>:  Endpoint


## bluemix target
{: #bluemix_target}


Set or view the target account, region, organization or space.

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>-r <i>REGION_NAME</i> (optional)</dt>
   <dd>Name of the region to be switched to, such as 'us-south' or 'eu-gb'.</dd>
   <dt>-c <i>ACCOUNT_ID</i> (optional)</dt>
   <dd>The ID of the account to be targeted.</dd>
   <dt>--cf</dt>
   <dd>Interactively select the target organization and space</dd>
   <dt>-o <i>ORG_NAME</i> (optional)</dt>
   <dd>The name of the organization to be targeted.</dd>
   <dt>-s <i>SPACE_NAME</i> (optional)</dt>
   <dd>The name of the space to be targeted.</dd>
   </dl>
If none of the options are specified, the current account, region, org and space are displayed.

<strong>Examples</strong>:

Set the current account, organization and space:

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

Switch to a new region:

```
bluemix target -r eu-gb
```

View the current account, region, org and space:

```
bluemix target
```

### bluemix update
{: #bluemix_update}

Update the CLI to the latest version.

```
bluemix update
```

<strong>Prerequisites</strong>:  None

### bluemix account orgs
{: #bluemix_account_orgs}

List all organizations

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>-r <i>REGION</i> (optional)</dt>
   <dd>For which region the organization information is shown. If set to 'all', all organizations in all regions are listed.</dd>
   <dt>--guid (optional)</dt>
   <dd>Display the GUID of the organizations.</dd>
   </dl>

<strong>Examples</strong>:

List all the organizations in region: `us-south` with the GUID displayed

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

Show the information for the specified organization.

```
bluemix account org ORG_NAME [--guid]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization.</dd>
   <dt>--guid (optional)</dt>
   <dd>Display the GUID of the organization.</dd>
   </dl>

<strong>Examples</strong>:

Show the information of organization `IBM` with the GUID displayed

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

Create a new organization. This operation can only be performed by account owner.

```
bluemix account org-create ORG_NAME [-f]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization being created.</dd>
   <dt>-f</dt>
   <dd>Force creation without confirmation.</dd>
   </dl>

<strong>Examples</strong>:

Create an organization named `IBM`.

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

Replicate an org from the current region to another region.

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the existing org that is to be replicated.</dd>
   <dt>REGION_NAME (required)</dt>
   <dd>The name of the region that hosts the replicated org.</dd>
   </dl>

<strong>Examples</strong>:

Replicate the org `myorg` to the region `eu-gb`:

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

Rename an organization. This operation can be done only by an org manager.

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>OLD_ORG_NAME (required)</dt>
   <dd>The old name of the org that is to be renamed.</dd>
   <dt>NEW_ORG_NAME (required)</dt>
   <dd>The new name of the org that it is renamed to.</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

List all spaces

```
bluemix account spaces [-o ORG_NAME] [-r REGION-NAME]
```

<strong>Command options</strong>:
   <dl>
   <dt>-o</dt>
   <dd>Organization name. List the spaces under the organization specified. Default to current organization if not specified.</dd>
   <dt>-r</dt>
   <dd>Region name. List the spaces under the region specified. Default to current region if not specified.</dd>
   </dl>



## bluemix account space
{: #bluemix_account_space}

This command has the same function and options as the `cf space` command.


## bluemix account space-create
{: #bluemix_account_space_create}

This command has the same function and options as the `cf create-space` command.


## bluemix account space-rename
{: #bluemix_account_space_rename}


This command has the same function and options as the `cf rename-space` command.


## bluemix account space-delete
{: #bluemix_account_space_delete}


This command has the same function and options as the `cf delete-space` command.

## bluemix account org-users
{: #bluemix_account_org_users}

Display users in the specified organization by role.

```
bluemix account org-users ORG_NAME [-a]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>ORG_NAME (required)</dt>
<dd>The name of the organization.</dd>
<dt>-a (optional)</dt>
<dd>List all the users in the specified organization, not grouped by role.</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

Add a user into org (org manager required).

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

Remove a user from org (org manager or user him/herself only)

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>Command options</strong>:
<dl>
<dt>--force, -f</dt>
<dd>Force deletion without confirmation.</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

Get all organization roles of the current user

```
bluemix account org-roles [-u USER_ID]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
  <dl>
   <dt>-u</dt>
   <dd>User ID. If not specified, default to current user.</dd>
  </dl>

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

Assign an organization role to a user. This operation can be performed only by an organization manager.

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
  <dl>
   <dt>USER_NAME (required)</dt>
   <dd>The name of the user being assigned.</dd>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization this user is assigned to.</dd>
   <dt>ORG_ROLE (required)</dt>
   <dd>The name of the organization role this user is assigned to. For example:
   <ul>
   <li>OrgManager: This role can invite and manage users, select and change plans, and set spending limits.</li>
   <li>BillingManager: This role can create and manage the billing account and payment information.</li>
   <li>OrgAuditor: This role has read-only access to org information and reports.</li>
   </ul>
   </dd>
  </dl>

<strong>Examples</strong>:

Assign user `Mary` to the organization `IBM` as `OrgManager` role:

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**Note**: You can set org/space roles using the CLI, but if you want to set the other permissions, you have to use the UI. For further details, see [Assigning user access](/docs/iam/assignaccess.html#assignaccess).
<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

Remove an organization role from a user. This operation can be performed only by an organization manager.

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>USER_NAME (required)</dt>
   <dd>The name of the user being removed.</dd>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization this user is removed from.</dd>
   <dt>ORG_ROLE (required)</dt>
   <dd>The name of the organization role this user is removed from. For example:
   <ul>
   <li>OrgManager: This role can invite and manage users, select and change plans, and set spending limits.</li>
   <li>BillingManager: This role can create and manage the billing account and payment information.</li>
   <li>OrgAuditor: This role has read-only access to org information and reports.</li>
   </ul>
   </dd>
    </dl>

<strong>Examples</strong>:

Remove user `Mary` from the organization `IBM` as `OrgManager` role:

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

Display users in the specified space by role.

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization.</dd>
   <dt>SPACE_NAME (required)</dt>
   <dd>The name of the space.</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

Assign a space role to a user. This operation can be performed only by a space manager.

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

   <dl>
   <dt>USER_NAME (required)</dt>
   <dd>The name of the user being assigned.</dd>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization this user is assigned to.</dd>
   <dt>SPACE_NAME (required)</dt>
   <dd>The name of the space this user is assigned to.</dd>
   <dt>SPACE_ROLE (required)</dt>
   <dd>The name of the space role this user is assigned to. For example:
   <ul>
   <li>SpaceManager: This role can invite and manage users, and enable features for a given space.</li>
   <li>SpaceDeveloper: This role can create and manage apps and services, and see logs and reports.</li>
   <li>SpaceAuditor: This role can view logs, reports, and settings for the space.</li>
   </ul></dd>
    </dl>

<strong>Examples</strong>:

Assign user `Mary` to the organization `IBM` and space `Cloud` as `SpaceManager` role:

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

Remove a space role from a user. This operation can be performed only by a space manager.

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

   <dl>
   <dt>USER_NAME (required)</dt>
   <dd>The name of the user being removed.</dd>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization this user is removed from.</dd>
   <dt>SPACE_NAME (required)</dt>
   <dd>The name of the space this user is removed from.</dd>
   <dt>SPACE_ROLE (required)</dt>
   <dd>The name of the space role this user is removed from. For example:
   <ul>
   <li>SpaceManager: This role can invite and manage users, and enable features for a given space.</li>
   <li>SpaceDeveloper: This role can create and manage apps and services, and see logs and reports.</li>
   <li>SpaceAuditor: This role can view logs, reports, and settings for the space.</li>
   </ul></dd>
    </dl>


<strong>Examples</strong>:

Remove user `Mary` from the organization `IBM` and space `Cloud` as `SpaceManager` role:

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

List all accounts of the current user

```
bluemix account list
```

<strong>Prerequisites</strong>:  Endpoint, Login


## bluemix account org-account
{: #bluemix_account_org_account}

Display the account of specified organization(org user required)

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
  <dt>--guid (optional)</dt>
  <dd>Display account ID only</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

Displays users associated with the account. This operation can be performed only by the account owner.

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

Delete a user from the current account(account owner only)

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>USERNAME (required)</dt>
<dd>Username</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>Account ID. If not specified, default to current account.</dd>
<dt>--force, -f (optional)</dt>
<dd>Force deletion without confirmation.</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

Invites a user to the account with an organization and space role already set. This operation can be performed only by the account owner.

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
   <dt>USER_NAME (required)</dt>
   <dd>The name of the user being invited.</dd>
   <dt>ORG_NAME (required)</dt>
   <dd>The name of the organization this user is invited to.</dd>
   <dt>ORG_ROLE (required)</dt>
   <dd>The name of the organization role this user is invited to. For example:
   <ul>
  <li>OrgManager: This role can invite and manage users, select and change plans, and set spending limits.</li>
  <li>BillingManager: This role can create and manage the billing account and payment information.</li>
  <li>OrgAuditor: This role has read-only access to org information and reports.</li>
  </ul> </dd>
   <dt>SPACE_NAME (required)</dt>
   <dd>The name of the space this user is invited to.</dd>
   <dt>SPACE_ROLE (required)</dt>
   <dd>The name of the space this user is invited to. The name of the space role this user is invited to. For example:
   <ul>
<li>SpaceManager: This role can invite and manage users, and enable features for a given space.</li>
<li>SpaceDeveloper: This role can create and manage apps and services, and see logs and reports.</li>
<li>SpaceAuditor: This role can view logs, reports, and settings for the space.</li>
</ul>
</dd>
</dl>

<strong>Examples</strong>:

Invite user `Mary` to the organization `IBM` as `OrgManager` role and the space `Cloud` as `SpaceAuditor` role:

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**Note**: You can set org/space roles during the invite using the CLI, but if you want to set the other permissions, you have to use the UI. For further details, see [Assigning user access](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

Resend invitation to a user(org manager or account owner is required)

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

List all service IDs

```
bluemix iam service-ids --uuid
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Show UUID of service IDs only</dd>
</dl>

<strong>Examples</strong>:
List UUID of all service IDs under current account

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

Display details of a service ID

```
bluemix iam service-id NAME [--uuid]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service</dd>
  <dt>-uuid</dt>
  <dd>Display the UUID of the service ID</dd>
</dl>

<strong>Examples</strong>:

Show details of service ID `sample-test`

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

Create a service ID

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service</dd>
  <dt>-d, --description</dt>
  <dd>Description of the service ID</dd>
</dl>

<strong>Examples</strong>:

Create a service ID with service name `sample-test` and description `hello, world!`

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
Update a service ID

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service</dd>
  <dt>-n, --name</dt>
  <dd>New name of the service</dd>
  <dt>-d, --description</dt>
  <dd>New description of the service</dd>
  <dt>-v, --version</dt>
  <dd>Version of the service ID</dd>
  <dt>-f, --force</dt>
  <dd>Update without confirmation</dd>
</dl>

<strong>Examples</strong>:

Rename service ID `sample-test` to `sample-test-2` without confirmation

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

Update description of service `sample-test` version `1-0jn39fbefew`

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

Delete a service ID

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service</dd>
  <dt>-f, --force</dt>
  <dd>Delete without confirmation</dd>
</dl>

<strong>Examples</strong>:

Delete service ID `sample-teset` without confirmation

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

List all {{site.data.keyword.Bluemix_notm}} platform API keys

```
bluemix iam api-keys
```

<strong>Prerequisites</strong>:  Endpoint, Login

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

Create a new {{site.data.keyword.Bluemix_notm}} platform API key

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>NAME (required)</dt>
<dd>Name of the API key to be created.</dd>
<dt>-d <i>DESCRIPTION</i> (optional)</dt>
<dd>Description of the API key</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>Save API key information to specified file. If not set, the JSON content will be displayed.</dd>
</dl>

<strong>Examples</strong>:

Create an API key and save to a file

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Update a {{site.data.keyword.Bluemix_notm}} platform API key

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>NAME (required)</dt>
<dd>The old name of the API key to be updated.</dd>
<dt>-n <i>NAME</i> (optional)</dt>
<dd>The new name of the API key</dd>
<dt>-d <i>DESCRIPTION</i> (optional)</dt>
<dd>The new description of the API key</dd>
</dl>

<strong>Examples</strong>:

Update the description of an API key:

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Delete a {{site.data.keyword.Bluemix_notm}} platform API key

```
bluemix iam api-key-delete NAME [-f]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>NAME (required)</dt>
<dd>Name of the API key to be deleted.</dd>
<dt>-f  (optional)</dt>
<dd>Force deletion without confirmation.</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

List all API keys of a service

```
bluemix iam service-api-keys SERVICE_ID
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
</dl>

<strong>Examples</strong>:

List all API keys of service `sample-service` :

```
bluemix iam service-api-keys sample-service
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

List details of a service API key

```
bluemix iam service-api-key NAME SERVICE_ID [--uuid]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Display the UUID of service API key</dd>
</dl>

<strong>Examples</strong>:

Show details of service API key `sample-key` of service `sample-service` :

```
bluemix iam service-api-key sample-key sample-service
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

Create a service API key

```
bluemix iam service-api-key-create NAME SERVICE_ID [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-d, --description</dt>
  <dd>Description of the API key</dd>
  <dt>-f, --file</dt>
  <dd>Save API key information to specified file. If not set, the JSON content will be displayed.</dd>
</dl>

<strong>Examples</strong>:

Create a service API key `sample-key` for service `sample-service` :

```
bluemix iam service-api-key-create sample-key sample-service
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

Update a service API key

```
bluemix iam service-api-key-update NAME SERVICE_ID  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-n, --name</dt>
  <dd>New name of the service API key</dd>
  <dt>-d, --description</dt>
  <dd>New description of the service API key</dd>
  <dt>-v, --version</dt>
  <dd>Version of the service API key</dd>
  <dt>-f, --force</dt>
  <dd>Update without confirmation</dd>
</dl>

<strong>Examples</strong>:

Rename service API key `sample-key` to `new-sample-key` :

```
bluemix iam service-api-key-update sample-key sample-service -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

Delete a service API key

```
bluemix iam service-api-key-delete NAME SERVICE_ID [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Delete without confirmation</dd>
</dl>

<strong>Examples</strong>:

Delete service API key `sample-key` :

```
bluemix iam service-api-key-delete sample-key sample-service
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

List policies of user `name@example.com`:

```
bluemix iam user-policies name@example.com
```

<strong>Prerequisites</strong>:  Endpoint, Login, Account Targeted

<strong>Command options</strong>:
<dl>
<dt>USER_NAME (required)</dt>
<dd>User name to whom the policies belong</dd>
</dl>

<strong>Examples</strong>:

List policies of user `name@example.com`:

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

Display details of a user policy

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>Prerequisites</strong>:  Endpoint, Login, Account Targeted

<strong>Command options</strong>:
<dl>
<dt>USER_NAME (required)</dt>
<dd>User name to whom the policy belongs</dd>
<dt>POLICY_ID (required)</dt>
<dd>ID of the policy</dd>
</dl>

<strong>Examples</strong>:

List policy `0bb730daa` of user `name@example.com`:

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

Create a user policy

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>Prerequisites</strong>:  Endpoint, Login, Account Targeted

<strong>Command options</strong>:
<dl>
<dt>USER_NAME (required)</dt>
<dd>User name to whom the policy belongs to</dd>
<dt>-f, --file <i>FILE</i> (optional)</dt>
<dd>JSON file of policy definition</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (optional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (optional)</dt>
<dd>Service name of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (optional)</dt>
<dd>Service instance of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--region <i>REGION</i> (optional)</dt>
<dd>Region of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (optional)</dt>
<dd>Resource type of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource <i>RESOURCE</i> (optional)</dt>
<dd>Resource of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (optional)</dt>
<dd>Name of the resource group, This is exclusive with '-f, --file', '--resource' and '--resource-group-id' flags.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (optional)</dt>
<dd>ID of the resource group, This is exclusive with '-f, --file', '--resource' and '--resource-group-name' flags.</dd>
  <dd>Role names of the policy definition. For supported roles of a specific service, run 'bluemix iam roles --service SERVICE_NAME'. This option is exclusive with '-f, --file'.</dd>
</dl>

<strong>Examples</strong>:

Create user policy for user `name@example.com` from policy JSON file `policy.json`:

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

Give `name@example.com` `Administrator` role for all `sample-service` resources:

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

Give `name@example.com` `Editor` role for resource `key123` of sample service instance `ServiceId-ade78e9f` in `us-south` region:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Give `name@example.com` `Operator` role for resource group with ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Give `name@example.com` `Viewer` role for the members of resource group `sample-resource-group`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

Give `name@example.com` `Viewer` role for the members of resource group with ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

Update a user policy

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>Prerequisites</strong>:  Endpoint, Login, Account Targeted

<strong>Command options</strong>:
<dt>USER_NAME (required)</dt>
<dd>User name to whom the policy belongs to</dd>
<dt>POLICY_ID (required)</dt>
<dd>ID of the policy to update</dd>
<dt>-v, --version <i>VERSION</i> (optional)</dt>
<dd>Version of existing policy</dd>
<dt>-f, --file <i>FILE</i> (optional)</dt>
<dd>JSON file of policy definition</dd>
<dt>-f, --file <i>FILE</i> (optional)</dt>
<dd>JSON file of policy definition</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (optional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (optional)</dt>
<dd>Service name of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (optional)</dt>
<dd>Service instance of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--region <i>REGION</i> (optional)</dt>
<dd>Region of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (optional)</dt>
<dd>Resource type of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource <i>RESOURCE</i> (optional)</dt>
<dd>Resource of the policy definition, This is exclusive with '-f, --file' flag.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (optional)</dt>
<dd>Name of the resource group, This is exclusive with '-f, --file', '--resource' and '--resource-group-id' flags.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (optional)</dt>
<dd>ID of the resource group, This is exclusive with '-f, --file', '--resource' and '--resource-group-name' flags.</dd>
  <dd>Role names of the policy definition. For supported roles of a specific service, run 'bluemix iam roles --service SERVICE_NAME'. This option is exclusive with '-f, --file'.</dd>
</dl>

<strong>Examples</strong>:

Update user policy with the one in JSON file：

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

Update user policy to give `name@example.com` `Administrator` role for all `sample-service` resources：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 Update user policy to give `name@example.com` `Editor` role for resource `key123` of sample service instance `ServiceId-ade78e9f` in `us-south` region:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Update user policy to give `name@example.com` `Operator` role for resource group with ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Update user policy to give `name@example.com` `Viewer` role for members of resource group `sample-resource-group`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

Update user policy to give `name@example.com` `Viewer` role for members of resource group with ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

List all service policies of specified service

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ID_NAME (required)</dt>
  <dd>Name of service ID</dd>
  <dt>-json</dt>
  <dd>Display policy in JSON format</dd>
  <dt>-f, --force</dt>
  <dd>Display service policies without confirmation</dd>
</dl>

<strong>Examples</strong>:

List policies of service `test`:

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

Display details of a service policy

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ID_NAME (required)</dt>
  <dd>Name of service ID</dd>
  <dt>POLICY_ID (required)</dt>
  <dd>ID of the service policy<dd>
  <dt>-json</dt>
  <dd>Display policy in JSON format</dd>
  <dt>-f, --force</dt>
  <dd>Display service policy without confirmation</dd>
</dl>

<strong>Examples</strong>:

Show policy `140798e2-8ea7db3` of service `test`:

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

Create a service policy

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ID_NAME (required)</dt>
  <dd>Name of service ID</dd>
  <dt>-f, --file</dt>
  <dd>JSON file of policy definition. This is exclusive with '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' and '--resource' flags.</dd>
  <dt>-r, --roles</dt>
  <dd>Role names of the policy definition. For supported roles of a specific service, run 'bluemix iam roles --service SERVICE_NAME'. This option is exclusive with '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Service name of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-service-instance</dt>
  <dd>Service instance of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-region</dt>
  <dd>Region of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-resource-type</dt>
  <dd>Resource type of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-resource</dt>
  <dd>Resource of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-F, --force</dt>
  <dd>Create service policy without confirmation</dd>
</dl>

<strong>Examples</strong>:

Create service policy from JSON file for service `test`:

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

Update a service policy

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ID_NAME (required)</dt>
  <dd>Name of service ID</dd>
  <dt>POLICY_ID (required)</dt>
  <dd>ID of the service policy<dd>
  <dt>-v, --version</dt>
  <dd>Version of the service policy</dd>
  <dt>-f, --file</dt>
  <dd>JSON file of policy definition. This is exclusive with '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' and '--resource' flags.</dd>
  <dt>-r, --roles</dt>
  <dd>Role names of the policy definition. For supported roles of a specific service, run 'bluemix iam roles --service SERVICE_NAME'. This option is exclusive with '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Service name of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-service-instance</dt>
  <dd>Service instance of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-region</dt>
  <dd>Region of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-resource-type</dt>
  <dd>Resource type of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-resource</dt>
  <dd>Resource of the policy definition. This is exclusive with '-f, --file' flag.</dd>
  <dt>-F, --force</dt>
  <dd>Update service policy without confirmation</dd>
</dl>

<strong>Examples</strong>:

Update service policy `140798e2-8ea7db3` from JSON file for service `test`:

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

Delete a service policy

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ID_NAME (required)</dt>
  <dd>Name of service ID</dd>
  <dt>POLICY_ID (required)</dt>
  <dd>ID of the service policy<dd>
  <dt>-f, --force</dt>
  <dd>Delete without confirmation</dd>
</dl>

<strong>Examples</strong>:

Delete policy `140798e2-8ea7db3` of service `test`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

List resource groups

```
bluemix resource groups [--default]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--default</dt>
  <dd>Get default group of current account</dd>
</dl>

<strong>Examples</strong>:

List all resource groups under currently targeted account:

```
bluemix resource groups
```

List default group of currentluy targeted account:

```
bluemix resource groups --default
```

## bluemix resource group
{: #bluemix_resource_group}

Show details of a resource group

```
bluemix resource group NAME [--id]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the resource group</dd>
  <dt>--id</dt>
  <dd>Show ID only</dd>
</dl>

<strong>Examples</strong>:

Show resource group `example-group`:

```
bluemix resource group example-group
```

Show only ID of resource group `example-group`:

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

Update an existing resource group

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the target resource group</dd>
  <dt>-n, --name</dt>
  <dd>New name of the resource group</dd>
  <dt>-q, --quota</dt>
  <dd>Name of the new quota definition</dd>
  <dt>-f</dt>
  <dd>Force update without confirmation</dd>
</dl>

<strong>Examples</strong>:

Rename resource group `example-group` to `trial-group`:

```
bluemix resource group-update example-group -n trial-group
```

Change the quota of resource group `example-group` to `free`:

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

List all quota definitions

```
bluemix resource quotas
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
</dl>

<strong>Examples</strong>:

List all quota definitions:

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

Show details of a quota definition

```
bluemix resource quota NAME
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the quota</dd>
</dl>

<strong>Examples</strong>:
Show details of quota `free`:

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

This command has the same function and options as the `cf push` command.


## bluemix app list
{: #bluemix_app_list}

This command has the same function and options as the `cf apps` command.


## bluemix app show
{: #bluemix_app_show}

This command has the same function and options as the `cf app` command.


## bluemix app delete
{: #bluemix_app_delete}

This command has the same function and options as the `cf delete` command.


## bluemix app rename
{: #bluemix_app_rename}

This command has the same function and options as the `cf rename` command.


## bluemix app start
{: #bluemix_app_start}

This command has the same function and options as the `cf start` command.


## bluemix app stop
{: #bluemix_app_stop}

This command has the same function and options as the `cf stop` command.


## bluemix app restart
{: #bluemix_app_restart}

This command has the same function and options as the `cf restart` command.


## bluemix app restage
{: #bluemix_app_restage}


This command has the same function and options as the `cf restage` command.


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


This command has the same function and options as the `cf restart-app-instance` command.


## bluemix app events
{: #bluemix_app_events}

This command has the same function and options as the `cf events` command.


## bluemix app files
{: #bluemix_app_files}

This command has the same function and options as the `cf files` command.


## bluemix app logs
{: #bluemix_app_logs}

This command has the same function and options as the `cf logs` command.


## bluemix app env
{: #bluemix_app_env}

This command has the same function and options as the `cf env` command.


## bluemix app env-set
{: #bluemix_app_env_set}

This command has the same function and options as the `cf set-env` command.


## bluemix app env-unset
{: #bluemix_app_env_unset}

This command has the same function and options as the `cf unset-env` command.


## bluemix app stacks
{: #bluemix_app_stacks}

This command has the same function and options as the `cf stacks` command.


## bluemix app stack-show
{: #bluemix_app_stack_show}

This command has the same function and options as the `cf stack` command.


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

This command has the same function and options as the `cf create-app-manifest` command.

## bluemix app domain-cert
{: #bluemix_app_domain_cert}

List the certificate information of a domain.

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
<dl>
<dt>DOMAIN_NAME (required)</dt>
<dd>The domain that hosts the certificate.</dd>
</dl>


<strong>Examples</strong>:

View the certificate information of the domain `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

Add a certificate to the specified domain in the current org.

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>Prerequisites</strong>:  Endpoint, Login, Target

<strong>Command options</strong>:
   <dl>
   <dt>DOMAIN (required)</dt>
   <dd>The domain that the certificate is added to.</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i> (required)</dt>
   <dd>The private key file path.</dd>
   <dt>-c <i>CERT_FILE</i> (required)</dt>
   <dd>The certificate file path.</dd>
   <dt>-p <i>PASSWORD</i> (optional)</dt>
   <dd>The password for the certificate.</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i> (optional)</dt>
   <dd>The intermediate certificate file path.</dd>
   <dt>-t <i>TRUST_STORE_FILE</i> (optional)</dt>
   <dd>The trust store file.</dd>
   </dl>


<strong>Examples</strong>:

Add a certificate to the domain `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

Remove a certificate from the specified domain in current org.

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>Prerequisites</strong>:  Endpoint, Login, Target

<strong>Command options</strong>:

   <dl>
   <dt>DOMAIN (required)</dt>
   <dd>Domain to remove the certificate from.</dd>
   <dt>-f  (optional)</dt>
   <dd>Force deletion without confirmation.</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

This command has the same function and options as the `cf domains` command.


## bluemix app domain-create
{: #bluemix_app_domain_create}

This command has the same function and options as the `cf create-domain` command.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

This command has the same function and options as the `cf delete-domain` command.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

This command has the same function and options as the `cf create-shared-domain` command.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

This command has the same function and options as the `cf delete-shared-domain` command.

## bluemix app routes
{: #bluemix_app_routes}

This command has the same function and options as the `cf routes` command.


## bluemix app route-check
{: #bluemix_app_route_check}

This command has the same function and options as the `cf check-route` command.


## bluemix app route-map
{: #bluemix_app_route_map}

Map a route to an existing cf application or container group that has the specified domain and host name.

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Prerequisites</strong>:  Endpoint, Login, Target

<strong>Command options</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (required)</dt>
   <dd>The name of the cf application or container group to be mapped with a route.</dd>
   <dt>DOMAIN (required)</dt>
   <dd>The domain of the route. For example, mychinabluemix.net or chinabluemix.net. </dd>
   <dt>-n <i>HOST_NAME</i> (optional)</dt>
   <dd>The host name of the route. If not provided, the host name is set to the app name or container group name by default.</dd>
   </dl>

<strong>Examples</strong>:

Map a route to `my-app` with specified domain:

```
bluemix app route-map my-app mychinabluemix.net
```

Map a route to 'my-container-group' with specified domain and host name:

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

Unmap the specified route from an existing cf application or container group.

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Prerequisites</strong>:  Endpoint, Login, Target

<strong>Command options</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (required)</dt>
   <dd>The name of the cf application or container group.</dd>
   <dt>DOMAIN (required)</dt>
   <dd>The domain of the route (for example, mychinabluemix.net or chinabluemix.net).</dd>
   <dt>-n <i>HOST_NAME</i> (optional)</dt>
   <dd>The host name of the route. If not provided, the host name is set to app name or container group name by default.</dd>
   </dl>

<strong>Examples</strong>:

Unmap `my-app.mychinabluemix.net` from `my-app`:

```
bluemix app route-unmap my-app mychianbluemix.net
```

Unmap `abc.chinabluexmix.net` from `my-container-group`:

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

This command has the same function and options as the `cf create-route` command.


## bluemix app route-delete
{: #bluemix_app_route_delete}

This command has the same function and options as the `cf delete-route` command.


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

This command has the same function and options as the `cf delete-orphaned-routes` command.


## bluemix app domains
{: #bluemix_app_domains}

This command has the same function and options as the `cf domains` command.


## bluemix app domain-create
{: #bluemix_app_domain_create}

This command has the same function and options as the `cf create-domain` command.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

This command has the same function and options as the `cf delete-domain` command.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

This command has the same function and options as the `cf create-shared-domain` command.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

This command has the same function and options as the `cf delete-shared-domain` command.


## bluemix service offerings
{: #bluemix_service_offerings}


This command has the same function and options as the `cf marketplace` command.


## bluemix service list
{: #bluemix_service_list}

This command has the same function and options as the `cf services` command.


## bluemix service show
{: #bluemix_service_show}

This command has the same function and options as the `cf service` command.


## bluemix service create
{: #bluemix_service_create}

This command has the same function and options as the `cf create-service` command.


## bluemix service update
{: #bluemix_service_update}

This command has the same function and options as the `cf update-service` command.


## bluemix service delete
{: #bluemix_service_delete}

This command has the same function and options as the `cf delete-service` command.


## bluemix service rename
{: #bluemix_service_rename}

This command has the same function and options as the `cf rename-service` command.


## bluemix service bind
{: #bluemix_service_bind}

This command has the same function and options as the `cf bind-service` command.


## bluemix service unbind
{: #bluemix_service_unbind}

This command has the same function and options as the `cf unbind-service` command.


## bluemix service key-create
{: #bluemix_service_key_create}

This command has the same function and options as the `cf create-service-key` command.


## bluemix service key-delete
{: #bluemix_service_key_delete}

This command has the same function and options as the `cf delete-service-key` command.


## bluemix service keys
{: #bluemix_service_keys}

This command has the same function and options as the `cf service-keys` command.


## bluemix service key-show
{: #bluemix_service_key_show}

This command has the same function and options as the `cf service-key` command.


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

This command has the same function and options as the `cf create-user-provided-service` command.


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

This command has the same function and options as the `cf update-user-provided-service` command.


## bluemix resource service-instances
{: #bluemix_resource_service_instances}

List service instances

```
bluemix resource service-instances [--service-name SERVICE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--service-name</dt>
  <dd>Name of belonging service</dd>
  <dt>-r, --region</dt>
  <dd>Filter by Region ID, default to current region if not specified, '-r, --region all' to display service instances under all regions</dd>
  <dt>--long</dt>
  <dd>Show additional fields in output</dd>
</dl>

<strong>Examples</strong>:

List service instances of service `test-service`:

```
bluemix resource service-instances --service-name test-service
```

## bluemix resource service-instance
{: #bluemix_resource_service_instance}

Show details of a service instance

```
bluemix resource service-instance NAME [-r, --region REGION] [--id]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service instance</dd>
  <dt>-r, --region</dt>
  <dd>Filter by Region ID, default to current region if not specified, '-r, --region all' to display service instances under all regions</dd>
  <dt>--id</dt>
  <dd>Display the ID of service instance</dd>
</dl>

<strong>Examples</strong>:
Show details of service instance `my-service-instance`:

```
bluemix resource service-instance my-service-instance
```

## bluemix resource service-instance-create
{: #bluemix_resource_service_instance_create}

Create a service instance

```
bluemix resource service-instance-create NAME SERVICE_NAME|SERVICE_ID SERVICE_PLAN_NAME|SERVICE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME (required)</dt>
  <dd>Name of the service instance</dd>
  <dt>SERVICE_NAME or SERVICE_ID (required)</dt>
  <dd>Name or ID of the service</dd>
  <dt>SERVICE_PLAN_NAME or SERVICE_PLAN_ID (required)</dt>
  <dd>Name or ID of the service plan</dd>
  <dt>-r, --region</dt>
  <dd>Region to create the service instance, default to current region if not specified</dd>
  <dt>-t, --tags</dt>
  <dd>Tags</dd>
  <dt>-p, --parameters</dt>
  <dd>JSON file or JSON string of parameters to create service instance</dd>
</dl>

<strong>Examples</strong>:
Create a service instance named `my-service-instance` using service plan `test-service-plan` of service `test-service`:

```
bluemix resource service-instance-create my-service-instance test-service test-service-plan
```

## bluemix resource service-instance-update
{: #bluemix_resource_service_instance_update}

Update service instance

```
bluemix resource service-instance-update SERVICE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--service-plan-id SERVICE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_INSTANCE_NAME (required)</dt>
  <dd>Name of the service instance</dd>
  <dt>-n, --name</dt>
  <dd>New service instance name</dd>
  <dt>-t, --tags</dt>
  <dd>New tags</dd>
  <dt>--service-plan-id</dt>
  <dd>New Service Plan ID</dd>
  <dt>--update-time</dt>
  <dd>Time in seconds since epoch when the chargeable record should take effect</dd>
  <dt>-f, --force</dt>
  <dd>Force update without confirmation</dd>
</dl>

<strong>Examples</strong>:
Update service instance `my-service-instance`, change its name to `new-service-instance`:

```
bluemix resource service-instance-update my-service-instance -n new-service-instance
```

## bluemix resource service-instance-delete
{: #bluemix_resource_service_instance_delete}

Delete service instance

```
bluemix resource service-instance-delete NAME [-f, --force] [--recursive]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Force deletion without confirmation</dd>
  <dt>--recursive</dt>
  <dd>Delete all belonging resources</dd>
</dl>

<strong>Examples</strong>:
Delete resource service-instance `my-service-instance`:

```
bluemix resource service-instance-delete my-service-instance
```

## bluemix resource service-bindings
{: #bluemix_resource_service_bindings}

Show bindings to the service alias

```
bluemix resource bindings SERVICE_ALIAS
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ALIAS (required)</dt>
  <dd>Service alias name</dd>
</dl>

<strong>Examples</strong>:
Show resource bindings to service alias `my-service-alias`:

```
bluemix resource bindings my-service-alias
```
## bluemix resource service-binding
{: #bluemix_resource_service_binding}

Show details of a service binding

```
bluemix resource service-binding ALIAS_NAME APP_NAME [--id]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>ALIAS_NAME (required)</dt>
  <dd>Service alias name</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry application name</dd>
  <dt>--id</dt>
  <dd>Only display the ID. All other output for the service binding is suppressed.</dd>
</dl>

<strong>Examples</strong>:
Show details of service binding between service alias `my-service-alias` and app `my-app`:

```
bluemix resource bindings my-service-alias my-app
```

## bluemix resource service-binding-create
{: #bluemix_resource_service_binding_create}

Create a service binding

```
bluemix resource service-binding-create SERVICE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ALIAS_NAME (required)</dt>
  <dd>Service alias name</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry application name</dd>
  <dt>ROLE_NAME</dt>
  <dd>Name of the user role</dd>
  <dt>--service-id-name</dt>
  <dd>Name of the service ID which the role belongs to</dd>
  <dt>-f, --force</dt>
  <dd>Force creation without confirmation</dd>
</dl>

<strong>Examples</strong>:
Create a service bindings between service alias `my-service-alias` and app `my-app` with role `Administrator`:

```
bluemix resource service-binding-create my-service-alias my-app Administrator
```
## bluemix resource service-binding-delete
{: #bluemix_resource_service_binding_delete}

Delete a service binding

```
bluemix resource service-binding-delete SERVICE_ALIAS APP_NAME [-f, --force]
```

<strong>Prerequisites</strong>: None

<strong>Command Options</strong>:
<dl>
  <dt>SERVICE_ALIAS_NAME (required)</dt>
  <dd>Service alias name</dd>
  <dt>APP_NAME</dt>
  <dd>CloudFoundry application name</dd>
  <dt>-f, --force</dt>
  <dd>Force deletion without confirmation</dd>
</dl>

<strong>Examples</strong>:
Delete the service binding between service alias `my-service-alias` and app `my-app`:

```
bluemix resource service-binding-delete my-service-alias my-app
```

## bluemix resource service-keys
{: #bluemix_resource_service_keys}

List service keys of service instance or service alias

```
bluemix resource service-keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>Service Instance ID</dd>
  <dt>--instance-name</dt>
  <dd>Service Instance Name</dd>
  <dt>--alias-id</dt>
  <dd>Service Alias ID</dd>
  <dt>--alias-name</dt>
  <dd>Service Alias Name</dd>
</dl>

<strong>Examples</strong>:
List service keys of service instance `my-service-instance`:

```
bluemix resource service-keys --instance-name my-service-instance
```

## bluemix resource service-key
{: #bluemix_resource_service_key}

Show details of a service key

```
bluemix resource service-key KEY_NAME [--id]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Name of the key</dd>
  <dt>--id</dt>
  <dd>Display the ID of service key</dd>
</dl>

<strong>Examples</strong>:
Show details of service keys `my-service-key`:

```
bluemix resource service-key my-service-key
```

## bluemix resource service-key-create
{: #bluemix_resource_service_key_create}

Create a service key

```
bluemix resource service-key-create NAME ROLE_NAME ( --instance-id SERVICE_INSTANCE_ID | --instance-name SERVICE_INSTANCE_NAME | --alias-id SERVICE_ALIAS_ID | --alias-name SERVICE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>NAME</dt>
  <dd>Name of the key</dd>
  <dt>ROLE_NAME</dt>
  <dd>Name of the user role</dd>
  <dt>--instance-id</dt>
  <dd>Service Instance ID</dd>
  <dt>--instance-name</dt>
  <dd>Service Instance Name</dd>
  <dt>--alias-id</dt>
  <dd>Service Alias ID</dd>
  <dt>--alias-name</dt>
  <dd>Service Alias Name</dd>
  <dt>-service-id-name</dt>
  <dd>Name of the service ID which the role belongs to</dd>
  <dt>-f, --force</dt>
  <dd>Force creation without confirmation</dd>
</dl>

<strong>Examples</strong>:
Create a service key named `my-service-key` with role `Administrator` for service instance `my-service-instance`:

```
bluemix resource service-key-create my-service-key Administrator --instance-name my-service-instance
```

## bluemix resource service-key-delete
{: #bluemix_resource_service_key_delete}

Delete a service key

```
bluemix resource service-key-delete KEY_NAME [-f, --forece]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Name of the key</dd>
  <dt>-f, --force</dt>
  <dd>Force deletion without confirmation</dd>
</dl>

<strong>Examples</strong>:
Delete service key `my-service-key`:

```
bluemix resource service-key-delete my-service-key
```

## bluemix resource service-aliases
{: #bluemix_resource_service_aliases}

List aliases for a service instance

```
bluemix resource service-aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID of the belonging service instance.</dd>
  <dt>--instance-name</dt>
  <dd>Name of the belonging service instance.</dd>
</dl>

<strong>Examples</strong>:
List service aliases for service instance `my-service-instance`:
```
bluemix resource service-aliases my-service-instance
```

## bluemix resource service-alias
{: #bluemix_resource_service_alias}

Show details of a service alias

```
bluemix resource service-alias ALIAS_NAME [--id]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>ALIAS_NAME (required)</dt>
  <dd>Name of the service alias</dd>
  <dt>--id</dt>
  <dd>Only display the given service alias's ID. All other output for the alias is suppressed.</dd>
</dl>

<strong>Examples</strong>:
Show details of service alias `my-service-alias`:
```
bluemix resource service-aliase  my-service-alias
```

## bluemix resource service-alias-create
{: #bluemix_resource_service_alias_create}

Create an alias of a service instance

```
bluemix resource service-alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>ALIAS_NAME (required)</dt>
  <dd>Name of the service alias</dd>
  <dt>--instance-id</dt>
  <dd>ID of the belonging service instance.</dd>
  <dt>--instance-name</dt>
  <dd>Name of the belonging service instance.</dd>
  <dt>-s</dt>
  <dd>Name of the space in which the alias is created. Default is the current space.</dd>
  <dt>-t, --tags</dt>
  <dd>Tags list.</dd>
  <dt>-p, --parameters</dt>
  <dd>Parameters JSON file or JSON string.</dd>
</dl>

<strong>Examples</strong>:
Create a service alias named `my-service-alias` of service instance `my-service-instance`:
```
bluemix resource service-aliase-create my-service-alias --instance-name my-service-instance
```

## bluemix resource service-alias-update
{: #bluemix_resource_service_alias_update}

Update an service alias

```
bluemix resource service-alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>ALIAS_NAME (required)</dt>
  <dd>Name of the service alias</dd>
  <dt>-n, --name</dt>
  <dd>New name of the service alias.</dd>
  <dt>-t, --tags</dt>
  <dd>Tags list.</dd>
  <dt>-p, --parameters</dt>
  <dd>Parameters JSON file or JSON string.</dd>
  <dt>-f, --force</dt>
  <dd>Force update without user confirmation.</dd>
</dl>

<strong>Examples</strong>:
Update service alias `my-service-alias`, change its name to `new-service-alias`:

```
bluemix resource service-alias-update my-service-alias -n new-service-alias
```

## bluemix resource service-alias-delete
{: #bluemix_resource_service_alias_delete}

Delete a service alias

```
bluemix resource service-alias-delete ALIAS_NAME [-f, --force]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>ALIAS_NAME (required)</dt>
  <dd>Name of the service alias</dd>
  <dt>-f, --force</dt>
  <dd>Force deletion without confirmation</dd>
</dl>

<strong>Examples</strong>:
Delete service alias `my-service-alias`:

```
bluemix resource service-alias-delete my-service-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

Search catalog entries

```
bluemix catalog search <QUERY> [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--col COLUMNS] [--reverse] [--json] [--csv] [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-r, --region</dt>
  <dd>Specify the geographic region to search within. Currently only "us-south" and "united-kingdom" are supported</dd>
  <dt>-k, --kind</dt>
  <dd>Filter by kind of resources. Currently only "service-cf", "iaas", "runtime", "template", and "dashboard" are supported</dd>
  <dt>-p, --price</dt>
  <dd>Filter by price. Currently only "free", "paygo", "bluemix-subscription" are supported</dd>
  <dt>-t, --tag</dt>
  <dd>Filter by tag.</dd>
  <dt>--sort-by</dt>
  <dd>Property to sort by</dd>
  <dt>--col</dt>
  <dd>Specify additional columns for the table. Currently "group", "provider", and "tags"</dd>
  <dt>--reverse</dt>
  <dd>Whether to reverse the sorting order</dd>
  <dt>--json</dt>
  <dd>Output original JSON response</dd>
  <dt>--csv</dt>
  <dd>Output CSV file</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Search service `Automation test`:

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

Get a catalog entry

```
bluemix catalog entry ID [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--children</dt>
  <dd>Get all children for the catalog entry</dd>
  <dt>--json</dt>
  <dd>Output original JSON response</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Get entry with ID `a0ef1-d3b4j0`:

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
Create a new catalog entry(catalog admin of an account only)

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-p, --parent</dt>
  <dd>Parent ID of the object</dd>
  <dt>-c</dt>
  <dd>Valid JSON object containing catalog-specific configuration parameters, provided either in-line or in a file. For a list of supported configuration parameters, see documentation for the particular catalog entry.</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Create resource from JSON file with parent ID `a0ef1-d3b4j0`:

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
Update an existing catalog entry(catalog admin or editor of an account only)

```
bluemix catalog entry-update ID [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-c</dt>
  <dd>Valid JSON object containing catalog-specific configuration parameters, provided either in-line or in a file. For a list of supported configuration parameters, see documentation for the particular catalog entry.</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Update resource `j402-dnf1i` from JSON file:

```
bluemix update 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-delete
{: #bluemix_catalog_entry_delete}
Delete a catalog entry(catalog admin of an account only)
```
bluemix catalog entry-delete ID [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Delete resource `j402-dnf1i`:

```
bluemix catalog delete 'j402-dnf1i'
```


## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
Get the visibility for a catalog entry(catalog admin of an account only)

```
bluemix catalog entry-visibility ID [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>-json</dt>
  <dd>Output original JSON response</dd>
  <dt>-global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Get visibility of resource `j402-dnf1i` in global scope:

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
Update the visibility of an existing catalog entry(catalog admin of an account only)

```
bluemix catalog entry-visibility-set ID [--includes-add LIST] [--includes-remove LIST] [--excludes-add LIST] [--excludes-remove LIST] [--owner ID or Email] [--restrict] [--unrestrict] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>

  <dt>--includes-add</dt>
  <dd>Adding an account (or list of comma separated accounts) to the includes list, granting visibility to the entry. Email or Account GUIDs are acceptable</dd>
  <dt>--includes-remove</dt>
  <dd>Removing an account (or list of comma separated accounts) from the includes list, revoking visibility to the entry. Email or Account GUIDs are acceptable</dd>  
  <dt>--excludes-add</dt>
  <dd>Adding an account (or list of comma separated accounts) to the excludes list. Email or Account GUIDs are acceptable</dd>
  <dt>--excludes-remove</dt>
  <dd>Removing an account (or list of comma separated accounts) from the excludes list, revoking visibility to the entry. If the account was set by global admins, the account admins cannot remove the account.Email or Account GUIDs are acceptable</dd>
  <dt>--owner</dt>
  <dd>Changing the owner of an object. Email or Account GUIDs are acceptable.</dd>
  <dt>--restrict</dt>
  <dd>Changing the restriction of the visibility object to 'Private'</dd>
  <dt>--unrestrict</dt>
  <dd>Changing the restriction of the visibility object to 'Public'</dd>  
  <dt>-c</dt>
  <dd>Valid JSON object containing catalog-specific configuration parameters, provided either in-line or in a file. For a list of supported configuration parameters, see documentation for the particular catalog entry.</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Set visibility of resource `j402-dnf1i` from JSON file:

```
bluemix catalog entry-visibility-set 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
List service offerings in the marketplace

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>Prerequisites</strong>: Endpoint, Login, Target

<strong>Command Options</strong>:
<dl>
  <dt>--cf</dt>
  <dd>Show Cloud Foundry services only</dd>
  <dt>--rc</dt>
  <dd>Show RC compatible services only</dd>
  <dt>--global</dt>
  <dd>Operate in global scope</dd>
</dl>

<strong>Examples</strong>:

Show service offerings in global scope:

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

View the boilerplate templates on Bluemix.

```
bluemix catalog templates [-d]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

   <dl>
   <dt>-d (optional)</dt>
   <dd>If the <i>-d</i> option is specified, the description of each template is also displayed. Otherwise, only the ID and name of each template is shown.</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

View the detailed information of a specified boilerplate template.

```
bluemix catalog template TEMPLATE_ID
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:
   <dl>
   <dt>TEMPLATE_ID (required)</dt>
   <dd>The ID of the boilerplate template. Use <i>bluemix templates</i> to view all templates' IDs.</dd>
   </dl>


<strong>Examples</strong>:

View details of the template `mobileBackendStarter`:

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

Create a cf application that is based on the specified template with the specified URL and description. By default, the new app is started automatically.

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>Prerequisites</strong>:  Endpoint, Login, Target

<strong>Command options</strong>:
   <dl>
   <dt>TEMPLATE_ID (required)</dt>
   <dd>The template that the application will be based on when it is created. Use <i>bluemix templates</i> to see all templates' ID.</dd>
   <dt>CF_APP_NAME (required)</dt>
   <dd>The name of the cf application to be created.</dd>
   <dt>-u <i>URL</i> (optional)</dt>
   <dd>The route of the application. If not specified, the route is set by {{site.data.keyword.Bluemix_notm}} automatically based on your app name and default domain.</dd>
   <dt>-d <i>DESCRIPTION</i> (optional)</dt>
   <dd>Description of the application.</dd>
   <dt>--no-start (optional)</dt>
   <dd>Do not start the application automatically after it is created. If not specified, the application is started automatically after it is created.</dd>
   </dl>


<strong>Examples</strong>:

Create a cf application `my-app` based on `javaHelloWorld` template:

```
bluemix catalog template-run javaHelloWorld my-app
```

Create an application `my-ruby-app` based on `rubyHelloWorld` template with route `myrubyapp.chinabluemix.net` and description `My first ruby app on {{site.data.keyword.Bluemix_notm}}.`:

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

Create an application `my-python-app` based on `pythonHelloWorld` template without automatic start:

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

Show monthly usage and costs of your account.

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

<dl>
  <dt>-d MONTH_DATE (optional)</dt>
  <dd>Display data for month and date specifying by using the YYYY-MM format. If not specified, usage of the current month is shown.</dd>
  <dt>--json (optional)</dt>
  <dd>Display the usage result in JSON format.</dd>
</dl>

<strong>Examples</strong>:

Show my account's usage and cost report in 2016-06:

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

Show monthly usage details of an org. This operation can be done only by a billing manager of the org.

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

<dl>
  <dt>ORG_NAME (required)</dt>
  <dd>Name of the org.</dd>
  <dt>-d MONTH_DATE (optional)</dt>
  <dd>Display data for month and date specified by using the YYYY-MM format. If not specified, usage of the current month is shown.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Name of the region that hosts the org. If set to 'all', org usage in all regions is shown.</dd>
  <dt>--json (optional)</dt>
  <dd>Display the usage result in JSON format.</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

Show monthly usage summary for orgs in my account.

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Prerequisites</strong>:  Endpoint, Login

<strong>Command options</strong>:

<dl>
  <dt>-d MONTH_DATE (optional)</dt>
  <dd>Display data for month and date specified by using the YYYY-MM format. If not specified, usage of the current month is shown.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Name of the region that hosts the orgs. If set to 'all', usage summary of the orgs in all regions is shown.</dd>
  <dt>--json (optional)</dt>
  <dd>Display the usage result in JSON format.</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

List all plugin repositories that are registered in {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repos
```

<strong>Prerequisites</strong>:  None


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

Add a new plugin repository to {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:

   <dl>
   <dt>REPO_NAME (required)</dt>
   <dd>The name of the repository to be added. You can define your own name for each repository.</dd>
   <dt>REPO_URL (required)</dt>
   <dd>The URL of the repository to be added. The repository URL must contain the protocol (for example, http://plugins.ng.bluemix.net instead of plugins.ng.bluemix.net). http://plugins.ng.bluemix.net is the official plugin repository of {{site.data.keyword.Bluemix_notm}} CLI.</dd>
    </dl>


<strong>Examples</strong>:

Add the official plugin repository of {{site.data.keyword.Bluemix_notm}} CLI as `bluemix-repo`:

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

Remove a plugin repository from {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repo-remove REPO_NAME
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:
   <dl>
   <dt>REPO_NAME (required)</dt>
   <dd>The name of the repository to be removed.</dd>
   </dl>

<strong>Examples</strong>:

Remove `bluemix-repo` repository from {{site.data.keyword.Bluemix_notm}} CLI:

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

List all available plugins in all added repositories or a specific repository.

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (optional)</dt>
   <dd>List only the plugins in specified repository.</dd>
   </dl>

<strong>Examples</strong>:

List all plugins in all added repositories:

```
bluemix plugin repo-plugins
```

List all plugins in the `bluemix-repo` repository:

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

Show the details of a plug-in in the repository.

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (optional)</dt>
   <dd>The name of the repository. If no repository is specified, the command uses the default plug-in repository.å</dd>
   </dl>

<strong>Examples</strong>:

List details of plugin "IBM-Containers" in repository "sample-repo":

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

List details of plugin "IBM-Containers" in default repository

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

List all installed plugins in {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin list
```

<strong>Prerequisites</strong>:  None

## bluemix plugin show
{: #bluemix_plugin_show}

Show details of an installed plug-in

```
bluemix plugin show PLUGIN-NAME
```

<strong>Prerequisites</strong>:  None


## bluemix plugin install
{: #bluemix_plugin_install}

Install the specific version of plugin to {{site.data.keyword.Bluemix_notm}} CLI from the specified path or repository.

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME (required)</dt>
   <dd>If -r <i>REPO_NAME</i> is not specified, plugin is installed from the specified local path or remote URL.</dd>
   <dt>-r <i>REPO_NAME</i> (optional)</dt>
   <dd>The name of the repository where the plugin binary is located. If no repository is specified, the command uses the default plug-in repository.</dd>
   <dt>-v <i>VERSION</i> (optional)</dt>
   <dd>The version of the plugin to be installed. If not provided, the latest version of the plugin is installed. This option is valid only when you install the plugin from the repository.</dd>
    </dl>

<strong>Examples</strong>:

Install a plugin from the local file:

```
bluemix plugin install /downloads/new_plugin
```

Install a plugin from the remote URL:

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

Install the `IBM-Containers` plugin of the latest version from the `bluemix-repo` repository:

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
Install the `IBM-Containers` plugin with the  version `0.5.800` from the `bluemix-repo` repository:

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

Upgrade the plug-in from a repository

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>Name of the plugin to update. If not specified, the command checks upgrades for all plug-ins installed.</dd>
 <dt>-r REPO_NAME</dt>
 <dd>The name of the repository where the plugin binary is located. If not specified, the command uses the default plug-in repository.</dd>
 <dt>-v <i>VERSION</i> (optional)</dt>
 <dd>The version of the plugin to be updated to. If not provided, update the plugin to the the latest available version.</dd>
 <dt>--all</dt>
 <dd>Update all available plug-ins</dd>
</dl>

<strong>Examples</strong>:

check for all available upgrade in plugin repository "My-Repo":

```
bluemix plugin update -r My-Repo
```

Upgrade plugin "plugin-echo" in repository "My-Repo" to the latest:

```
bluemix plugin update -r My-Repo plugin-echo
```

Update plugin "plugin-echo" in repository "My-Repo" to version "1.0.1":

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

Uninstall the specified plugin from {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>Prerequisites</strong>:  None

<strong>Command options</strong>:

   <dl>
   <dt>PLUGIN_NAME (required)</dt>
   <dd>The name of the plugin to be uninstalled.</dd>
    </dl>

<strong>Examples</strong>:

Uninstall the `IBM-Containers` plugin that was previously installed:

```
bluemix plugin uninstall IBM-Containers
```
