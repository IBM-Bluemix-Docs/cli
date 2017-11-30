---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Comandos do {{site.data.keyword.Bluemix_notm}} (bx)
{: #bluemix_cli}

Versão: 0.6.1

A interface de linha de comandos (CLI) do {{site.data.keyword.Bluemix_notm}} fornece um conjunto de comandos que são agrupados por namespace para que os usuários interajam com o {{site.data.keyword.Bluemix_notm}}. 

A partir da versão 0.5.0, o cliente da linha de comandos do {{site.data.keyword.Bluemix_notm}} empacota um cliente da linha de comandos Cloud Foundry em sua instalação. Se você tiver seu próprio cf cli instalado, não use os comandos da CLI do {{site.data.keyword.Bluemix_notm}} `bx [command]` e os comandos da CLI do Cloud Foundry `cf [command]` de sua própria instalação no mesmo contexto. Em vez disso, use `bluemix cf [command]` se desejar usar cf cli para gerenciar os recursos do Cloud Foundry no contexto da CLI do {{site.data.keyword.Bluemix_notm}}.  Além disso, `bluemix cf api/login/logout/target` não é permitido, use `bluemix api/login/logout/target`.

O seguinte lista os comandos de uso detalhadas que são suportados pela CLI do {{site.data.keyword.Bluemix_notm}}, incluindo seus nomes, argumentos, opções, pré-requisitos, descrições e exemplos.
{:shortdesc}

**Nota:** *Pré-requisitos* listam quais ações são necessárias antes de usar o comando. Os comandos que não têm ações de pré-requisito listam **Nenhum**. Caso contrário, os pré-requisitos podem incluir uma ou mais das ações a seguir:

<dl>
<dt>Nó de Extremidade</dt>
<dd>Um terminal de API deve ser configurado por meio de <code>bluemix api</code> antes de usar o comando.</dd>
<dt>Login</dt>
<dd>É necessário efetuar login usando o comando <code>bluemix login</code> antes de usar esse comando.
Se estiver efetuando login com o ID federado, use a opção '--sso' para se autenticar com uma senha única ou use '--apikey' para se autenticar com a chave API. Acesse o console do {{site.data.keyword.Bluemix_notm}}: **Gerenciar** &gt; **Segurança** &gt; **Chaves API do Bluemix** para criar chaves API.
</dd>
<dt>Destino</dt>
<dd>O comando <code>bluemix target</code> deve ser usado para configurar uma organização e um espaço antes de usar esse comando.</dd>
<dt>Docker</dt>
<dd>A CLI do Docker (docker) deve estar instalada para executar esse comando.</dd>
</dl>

**Nota:** é possível usar o formato curto de comandos bluemix; por exemplo, `bx api` é a abreviação de `bluemix api`.

Use os índices nas tabelas a seguir para referir-se aos comandos do Bluemix usados frequentemente.

## Comandos gerais do Bluemix 
{: #bx_commands_index}

<table summary="Comandos gerais do Bluemix.">
<caption>Tabela 1. Comandos gerais do Bluemix</caption>
 <thead>
 <th colspan="5">Comandos gerais do Bluemix</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix help
](bx_cli.html#bluemix_help)</td>
 <td>[bluemix api
](bx_cli.html#bluemix_api)</td>
 <td>[bluemix config](bx_cli.html#bluemix_config)</td>
 <td>[bluemix info](bx_cli.html#bluemix_info)</td>
 <td>[bluemix cf](bx_cli.html#bluemix_cf)</td>
 </tr>
 <tr>
 <td>[bluemix login](bx_cli.html#bluemix_login) </td>
 <td>[bluemix logout](bx_cli.html#bluemix_logout) </td>
 <td>[bluemix regions](bx_cli.html#bluemix_regions)</td>
 <td>[bluemix target
](bx_cli.html#bluemix_target)</td>
 <td>[bluemix update](bx_cli.html#bluemix_update)</td>
 </tr>
 </tbody>
 </table>
 
 ## Comandos para gerenciar e configurar serviços do {{site.data.keyword.BluSoftlayer_notm}}
  {: #bx_commands_softlayer}
  
Os comandos para gerenciar o {{site.data.keyword.BluSoftlayer_notm}}} foram mesclados na CLI do Bluemix. Para obter mais informações sobre como usar a CLI do Bluemix para configurar e gerenciar os serviços do {{site.data.keyword.BluSoftlayer_notm}}, veja: [Comandos do {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) da CLI do Bluemix](/docs/cli/reference/softlayer/index.md#softlayer_cli).
 
 ## Comandos para gerenciar contas, organizações e funções
 {: #bx_commands_account}

<table summary="Comandos do Bluemix que podem ser usados para gerenciar contas, organizações, espaços e funções.">
<caption>Tabela 2. Comandos para gerenciar contas, organizações, espaços e funções</caption>
 <thead>
 <th colspan="5">Comandos para gerenciar contas, organizações, espaços e funções</th>
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


 ## Comandos para gerenciar recursos e grupos de recursos
{: #bx_commands_resource}

<table summary="Comando do Bluemix que pode ser usado para gerenciar grupos de recursos e recursos.">
  <caption>Tabela 3. Comandos para gerenciar grupos de recursos e recursos</caption>
  <thead>
    <th colspan="5">Comandos para gerenciar recursos e grupos de recursos</th>
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

 
 ## Comandos para gerenciar chaves API e políticas
 {: #bx_commands_iam}
 <table summary="Comandos do Bluemix que podem ser usados para gerenciar chaves API e políticas.">
 <caption>Tabela 3. Comandos para gerenciar chaves API e políticas</caption>
  <thead>
  <th colspan="5">Comandos para gerenciar chaves API e políticas</th>
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
 
 ## Comandos para gerenciar apps cf e domínios, rotas e certificados relacionados ao app
 {: #bx_commands_apps}

<table summary="Comandos do Bluemix que podem ser usados para gerenciar apps cf e domínios, rotas e certificados relacionados aos apps.">
<caption>Tabela 4. Comandos para gerenciar apps cf e domínios, rotas e certificados relacionados ao app</caption>
 <thead>
 <th colspan="5">Comandos para gerenciar apps cf e domínios, rotas e certificados relacionados aos apps</th>
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
 
 ## Comandos para gerenciar serviços do Bluemix
 {: #bx_commands_services}

<table summary="comandos do Bluemix que podem ser usados para gerenciar serviços do Bluemix.">
<caption>Tabela 5. Comandos para gerenciar serviços do Bluemix</caption>
 <thead>
 <th colspan="5">Comandos para gerenciar serviços do Bluemix</th>
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

 
 ## Comandos para gerenciar configurações de catálogo, de plug-ins e de faturamento
 {: #bx_commands_settings}

<table summary="comandos do Bluemix que podem ser usados para gerenciar catálogo, plug-ins, faturamento e configurações de segurança do Bluemix.">
<caption>Tabela 6. Comandos para gerenciar catálogo, plug-ins, faturamento e configurações de segurança do Bluemix</caption>
 <thead>
 <th colspan="5">Comandos para gerenciar catálogo, plug-ins, faturamento e configurações de segurança do Bluemix</th>
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
  <td>[bluemix plugin repos
](bx_cli.html#bluemix_plugin_repos)</td>
  <td>[bluemix plugin repo-add](bx_cli.html#bluemix_plugin_repo_add)</td>
  <td>[bluemix plugin repo-remove](bx_cli.html#bluemix_plugin_repo_remove)</td>
  <td>[bluemix plugin repo-plugins](bx_cli.html#bluemix_plugin_repo_plugins)</td>
  <td>[bluemix plugin repo-plugin](bx_cli.html#bluemix_plugin_repo_plugin)</td>
 </tr>
 <tr>
  <td>[bluemix plugin list
](bx_cli.html#bluemix_plugin_list)</td>
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
Exiba a ajuda geral para comandos integrados de primeiro nível e namespaces suportados da CLI {{site.data.keyword.Bluemix_notm}} ou a ajuda para um comando ou namespace integrado específico.

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>COMMAND|NAMESPACE (opcional)</dt>
   <dd>O comando ou namespace para o qual a ajuda é exibida. Se não especificado, a ajuda geral para a CLI do {{site.data.keyword.Bluemix_notm}} será mostrada.</dd>
   </dl>



<strong>Exemplos</strong>:

Exiba a ajuda geral para a CLI do {{site.data.keyword.Bluemix_notm}}:

```
bluemix help
```

Exiba a ajuda para o comando `info`:

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
Configure ou visualize o terminal da API do {{site.data.keyword.Bluemix_notm}}.

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
   <dl>
   <dt>API_ENDPOINT (opcional)</dt>
   <dd>O terminal da API que é o destino, por exemplo, `https://api.chinabluemix.net`. Se as opções *API_ENDPOINT* e `--unset` não forem ambas especificadas, o terminal de API atual será exibido.</dd>
   <dt>--unset (opcional)</dt>
   <dd>Remova a configuração do terminal de API.</dd>
   <dt>--skip-ssl-validation (opcional)</dt>
   <dd>Validação SSL de bypass de solicitações de HTTP.</dd>
   </dl>
<strong>Exemplos</strong>:

Configure o terminal da API para api.chinabluemix.net:

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

Visualize o terminal de API atual:

```
bluemix api
```

Desconfigure o terminal de API:

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


Grave os valores padrão no arquivo de configuração.

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>O valor de tempo limite para solicitações de HTTP. O valor padrão é 60 segundos.</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>Rastreie solicitações de HTTP para o terminal ou arquivo especificado.</dd>
   <dt>--color true|false</dt>
   <dd>Ative ou desative a saída de cor. A saída de cor é ativada por padrão.</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>Configure um código padrão de idioma. Se LOCALE for <i>CLEAR</i>, o código de idioma anterior será excluído.</dd>
   <dt>--check-version true|false</dt>
   <dd>Ative ou desative a verificação de versão da CLI.</dd>
   </dl>

Somente uma dessas opções pode ser especificada por vez.

<strong>Exemplos</strong>:

Configure o tempo limite de solicitação de HTTP como 30 segundos:

```
bluemix config --http-timeout 30
```

Ative a saída de rastreio para solicitações de HTTP:

```
bluemix config --trace true
```

Rastreie solicitações de HTTP para um arquivo especificado */home/usera/my_trace*:

```
bluemix config --trace /home/usera/my_trace
```

Desative a saída de cor:

```
bluemix config --color false
```

Configure o código de idioma como zh_Hans:

```
bluemix config --locale zh_Hans
```

Limpe as configurações do código de idioma:

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

Visualize as informações básicas do {{site.data.keyword.Bluemix_notm}}, incluindo a região atual, a versão do controlador de nuvem e alguns terminais úteis, como terminais para login e a troca de token de acesso.

```
bluemix info
```

<strong>Pré-requisitos</strong>: Terminal


## bluemix cf
{: #bluemix_cf}

Chamar o CF CLI integrado

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
<dl>
  <dt>-q, --quiet</dt>
  <dd>Desativar a mensagem "Chamando comando cf..."</dd>
</dl>

<strong>Exemplos</strong>:

Liste apps cf:

```
bluemix cf apps
```

Listar serviços cf sem a mensagem "Chamando comando cf...":

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

Efetue login do usuário. 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>Pré-requisitos</strong>: Nenhum

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>Opções de comando</strong>:
<dl>
  <dt> -a <i>API_ENDPOINT</i> (opcional)</dt>
  <dd> Terminal de API (Por exemplo: api.ng.bluemix.net)</dd>
  <dt> --apikey <i>API_KEY ou @API_KEY_FILE_PATH</i>
  <dd> Conteúdo da chave API ou o caminho de um arquivo de chave API indicado por @</dd>
  <dt> --sso (opcional) </dt>
  <dd> Use uma senha única para efetuar login </dd>
  <dt> -u <i>USERNAME</i> (opcional)</dt>
  <dd> Username</dd>
  <dt> -p <i>PASSWORD</i> (opcional)</dt>
  <dd> Senha</dd>
  <dt> -c <i>ACCOUNT_ID</i> (opcional) </dt>
  <dd> ID da conta de destino</dd>
  <dt> -o <i>ORG_NAME</i> (opcional) </dt>
  <dd> Nome da organização de destino </dd>
  <dt> -s <i>SPACE_NAME</i> (opcional) </dt>
  <dd> Nome do espaço de destino</dd>
  <dt> --skip-ssl-validation (opcional) </dt>
  <dd> Validação SSL de bypass de solicitações de HTTP. Essa opção não é recomendada.</dd>
</dl>

<strong>Exemplos</strong>:

#### Login interativo

```
bluemix login
```

Efetuar login com nome de usuário e senha e configurar a conta de destino, a organização e o espaço:

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

Efetuar login com uma senha única e configurar a conta de destino, a organização e o espaço

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

Efetuar login com a chave API e configurar os destinos:

#### A chave API tem conta associada

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### A chave API não tem conta associada

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>Nota:</strong> se a chave API tiver uma conta associada, não será permitido alternar para outra conta.

#### Usar uma senha única

```
bluemix login -u UserID --sso
```

Em seguida, a CLI fornecerá um link de URL e solicitará a senha:
```
One Time Code (Get one at https://URL_Link_To_Obtain_Passcode):
```

Abra o link no navegador, que fornecerá instrução para obter a senha. Digite a senha especificada no console e você poderá efetuar login.

## bluemix logout
{: #bluemix_logout}

Efetue logout do usuário.

```
bluemix logout
```

<strong>Pré-requisitos</strong>: Nenhum

## bluemix regions
{: #bluemix_regions}

Visualize as informações para todas as regiões no {{site.data.keyword.Bluemix_notm}}.

```
bluemix regions
```

<strong>Pré-requisitos</strong>: Terminal


## bluemix target
{: #bluemix_target}


Configure ou visualize a conta de destino, região, organização ou espaço.

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>-r <i>REGION_NAME</i> (opcional)</dt>
   <dd>Nome da região a ser alternada, como 'us-south' ou 'eu-gb'.</dd>
   <dt>-c <i>ACCOUNT_ID</i> (opcional)</dt>
   <dd>O ID da conta que será o destino.</dd>
   <dt>--cf</dt>
   <dd>Selecione de forma interativa o espaço e a organização de destino</dd>
   <dt>-o <i>ORG_NAME</i> (opcional)</dt>
   <dd>O nome da organização que será o destino.</dd>
   <dt>-s <i>SPACE_NAME</i> (opcional)</dt>
   <dd>O nome do espaço que será o destino.</dd>
   </dl>
Se nenhuma das opções for especificada, a conta, a região, a organização e o espaço atuais serão exibidos.

<strong>Exemplos</strong>:

Configure a conta atual, a organização e o espaço:

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

Alterne para uma nova região:

```
bluemix target -r eu-gb
```

Visualize a conta, a região, a organização e o espaço atuais:

```
bluemix target
```

### bluemix update
{: #bluemix_update}

Atualize a CLI para a versão mais recente.

```
bluemix update
```

<strong>Pré-requisitos</strong>: Nenhum

### bluemix account orgs
{: #bluemix_account_orgs}

Liste todas as organizações

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>-r <i>REGION</i> (opcional)</dt>
   <dd>Para qual região as informações da organização são mostradas. Se configurado como 'all', todas as organizações em todas as regiões serão listadas.</dd>
   <dt>--guid (opcional)</dt>
   <dd>Exiba o GUID das organizações.</dd>
   </dl>

<strong>Exemplos</strong>:

Liste todas as organizações na região: `us-south` com o GUID exibido

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

Mostre as informações para a organização especificada.

```
bluemix account org ORG_NAME [--guid]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização.</dd>
   <dt>--guid (opcional)</dt>
   <dd>Exiba o GUID da organização.</dd>
   </dl>

<strong>Exemplos</strong>:

Mostre as informações da organização `IBM` com o GUID exibido

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

Criar uma nova organização. Essa operação pode ser executada somente pelo proprietário da conta.

```
bluemix account org-create ORG_NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização que está sendo criada.</dd>
   </dl>

<strong>Exemplos</strong>:

Crie uma organização denominada `IBM`.

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

Replique uma organização a partir da região atual para outra região.

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização existente que deve ser replicada.</dd>
   <dt>REGION_NAME (necessário)</dt>
   <dd>O nome da região que hospeda a organização replicada.</dd>
   </dl>

<strong>Exemplos</strong>:

Replique a organização `myorg` para a região `eu-gb`:

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

Renomeie uma organização. Essa operação pode ser executada somente por um gerenciador de organização.

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>OLD_ORG_NAME (necessário)</dt>
   <dd>O nome antigo da organização que deve ser renomeada.</dd>
   <dt>NEW_ORG_NAME (necessário)</dt>
   <dd>O novo nome da organização para o qual ela é renomeada.</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

Esse comando tem a mesma função e opções que o comando `cf spaces`.


## bluemix account space
{: #bluemix_account_space}

Esse comando tem a mesma função e opções que o comando `cf space`.


## bluemix account space-create
{: #bluemix_account_space_create}

Esse comando tem a mesma função e opções que o comando `cf create-space`.


## bluemix account space-rename
{: #bluemix_account_space_rename}


Esse comando tem a mesma função e opções que o comando `cf rename-space`.


## bluemix account space-delete
{: #bluemix_account_space_delete}


Esse comando tem a mesma função e opções que o comando `cf delete-space`.

## bluemix account org-users
{: #bluemix_account_org_users}

Exiba usuários na organização especificada por função.

```
bluemix account org-users ORG_NAME [-a]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>ORG_NAME (necessário)</dt>
<dd>O nome da organização.</dd>
<dt>-a (opcional)</dt>
<dd>Liste todos os usuários na organização especificada, não agrupados por função.</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

Inclua um usuário na organização (gerenciador de organização requerido).

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

Remova um usuário da organização (gerente da organização ou o próprio usuário somente)

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>Opções de comando</strong>:
<dl>
<dt>--force, -f</dt>
<dd>Force a exclusão sem confirmação.</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

Obtenha todas as funções de organização do usuário atual

```
bluemix account org-roles
```

<strong>Pré-requisitos</strong>: Terminal, Login

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

Designe uma função de organização a um usuário. Essa operação pode ser executada somente por um gerenciador de organização.

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
  <dl>
   <dt>USER_NAME ((necessário))</dt>
   <dd>O nome do usuário que está sendo designado.</dd>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização para a qual esse usuário é designado.</dd>
   <dt>ORG_ROLE (necessário)</dt>
   <dd>O nome da função de organização para a qual esse usuário é designado. Por
exemplo:
   <ul>
   <li>OrgManager: essa função pode convidar e gerenciar usuários, selecionar e mudar planos e configurar limites de gastos.</li>
   <li>BillingManager: essa função pode criar e gerenciar a conta de cobrança e informações de pagamento.</li>
   <li>OrgAuditor: essa função possui acesso somente leitura para informações e relatórios da organização.</li>
   </ul>
   </dd>
  </dl>

<strong>Exemplos</strong>:

Designe o usuário `Mary` à organização do `IBM` como função `OrgManager`:

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: é possível configurar as funções de organização/espaço usando a CLI, mas se você desejar configurar as outras permissões, precisará usar a UI. Para obter detalhes adicionais, veja [Designando o acesso de usuário](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

Remover uma função de organização de um usuário. Essa operação pode ser executada somente por um gerenciador de organização.

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>USER_NAME ((necessário))</dt>
   <dd>O nome do usuário que está sendo removido.</dd>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização da qual esse usuário é removido.</dd>
   <dt>ORG_ROLE (necessário)</dt>
   <dd>O nome da função de organização da qual esse usuário é removido. Por
exemplo:
   <ul>
   <li>OrgManager: essa função pode convidar e gerenciar usuários, selecionar e mudar planos e configurar limites de gastos.</li>
   <li>BillingManager: essa função pode criar e gerenciar a conta de cobrança e informações de pagamento.</li>
   <li>OrgAuditor: essa função possui acesso somente leitura para informações e relatórios da organização.</li>
   </ul>
   </dd>
    </dl>

<strong>Exemplos</strong>:

Remova o usuário `Mary` da organização `IBM` como função `OrgManager`:

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

Exiba usuários no espaço especificado por função.

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização.</dd>
   <dt>SPACE_NAME (necessário)</dt>
   <dd>O nome do espaço.</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

Designe uma função de espaço a um usuário. Essa operação pode ser executada somente por um gerenciador de espaço.

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

   <dl>
   <dt>USER_NAME ((necessário))</dt>
   <dd>O nome do usuário que está sendo designado.</dd>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização para a qual esse usuário é designado.</dd>
   <dt>SPACE_NAME (necessário)</dt>
   <dd>O nome do espaço para o qual esse usuário é designado.</dd>
   <dt>SPACE_ROLE (necessário)</dt>
   <dd>O nome da função de espaço para a qual esse usuário é designado. Por
exemplo:
   <ul>
   <li>SpaceManager: essa função pode convidar e gerenciar usuários e ativar recursos para um determinado espaço.</li>
   <li>SpaceDeveloper: essa função pode criar e gerenciar aplicativos e serviços, bem como ver logs e relatórios.</li>
   <li>SpaceAuditor: essa função pode visualizar logs, relatórios e configurações para o espaço.</li>
   </ul></dd>
    </dl>

<strong>Exemplos</strong>:

Designe o usuário `Mary` à organização `IBM` e espaço `Cloud` como função `SpaceManager`:

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

Remova uma função de espaço de um usuário. Essa operação pode ser executada somente por um gerenciador de espaço.

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

   <dl>
   <dt>USER_NAME ((necessário))</dt>
   <dd>O nome do usuário que está sendo removido.</dd>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização da qual esse usuário é removido.</dd>
   <dt>SPACE_NAME (necessário)</dt>
   <dd>O nome do espaço do qual esse usuário é removido.</dd>
   <dt>SPACE_ROLE (necessário)</dt>
   <dd>O nome da função de espaço da qual esse usuário é removido. Por
exemplo:
   <ul>
   <li>SpaceManager: essa função pode convidar e gerenciar usuários e ativar recursos para um determinado espaço.</li>
   <li>SpaceDeveloper: essa função pode criar e gerenciar aplicativos e serviços, bem como ver logs e relatórios.</li>
   <li>SpaceAuditor: essa função pode visualizar logs, relatórios e configurações para o espaço.</li>
   </ul></dd>
    </dl>


<strong>Exemplos</strong>:

Remova o usuário `Mary` da organização `IBM` e espaço `Cloud` como função `SpaceManager`:

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

Liste todas as contas do usuário atual

```
bluemix account list
```

<strong>Pré-requisitos</strong>: Terminal, Login


## bluemix account org-account
{: #bluemix_account_org_account}

Exibir a conta da organização especificada (usuário da organização necessário)

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
  <dt>--guid (opcional)</dt>
  <dd>Exibir somente o ID da conta</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

Exibe os usuários associados à conta. Essa operação pode ser executada somente pelo proprietário da conta.

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

Exclua um usuário da conta atual (somente o proprietário da conta)

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>USERNAME (necessário)</dt>
<dd>Username</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>ID da conta. Se não especificado, o padrão será a conta atual.</dd>
<dt>--force, -f (opcional)</dt>
<dd>Force a exclusão sem confirmação.</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

Convida um usuário para a conta com uma função de organização e espaço já configurada. Essa operação pode ser executada somente pelo proprietário da conta.

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
   <dt>USER_NAME ((necessário))</dt>
   <dd>O nome do usuário que está sendo convidado.</dd>
   <dt>ORG_NAME (necessário)</dt>
   <dd>O nome da organização para a qual esse usuário é convidado.</dd>
   <dt>ORG_ROLE (necessário)</dt>
   <dd>O nome da função de organização para a qual esse usuário é convidado. Por
exemplo:
   <ul>
  <li>OrgManager: essa função pode convidar e gerenciar usuários, selecionar e mudar planos e configurar limites de gastos.</li>
  <li>BillingManager: essa função pode criar e gerenciar a conta de cobrança e informações de pagamento.</li>
  <li>OrgAuditor: essa função possui acesso somente leitura para informações e relatórios da organização.</li>
  </ul> </dd>
   <dt>SPACE_NAME (necessário)</dt>
   <dd>O nome do espaço para o qual esse usuário é convidado.</dd>
   <dt>SPACE_ROLE (necessário)</dt>
   <dd>O nome do espaço para o qual esse usuário é convidado. O nome da função do espaço para o qual esse usuário é convidado. Por
exemplo:
   <ul>
<li>SpaceManager: essa função pode convidar e gerenciar usuários e ativar recursos para um determinado espaço.</li>
<li>SpaceDeveloper: essa função pode criar e gerenciar aplicativos e serviços, bem como ver logs e relatórios.</li>
<li>SpaceAuditor: essa função pode visualizar logs, relatórios e configurações para o espaço.</li>
</ul>
</dd>
</dl>

<strong>Exemplos</strong>:

Convide o usuário `Mary` para a organização `IBM` como função `OrgManager` e o espaço `Cloud` como função `SpaceAuditor`:

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: é possível configurar as funções de organização/espaço durante o convite usando a CLI, mas se você desejar configurar as outras permissões, precisará usar a UI. Para obter detalhes adicionais, veja [Designando o acesso de usuário](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

Reenviar o convite a um usuário (é necessário ser o gerente da organização ou o proprietário da conta)

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

Listar todos os IDs de serviço

```
bluemix iam service-ids --uuid
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Mostrar somente o UUID dos IDs de serviço</dd>
</dl>

<strong>Exemplos</strong>:
liste o UUID de todos os IDs de serviço na conta atual

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

Exibir detalhes de um ID de serviço

```
bluemix iam service-id NAME [--uuid]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do serviço</dd>
  <dt>-uuid</dt>
  <dd>Exibir o UUID do ID de serviço</dd>
</dl>

<strong>Exemplos</strong>:

Mostre detalhes do ID de serviço `sample-test`

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

Criar um ID de serviço

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do serviço</dd>
  <dt>-d, --description</dt>
  <dd>Descrição do ID de serviço</dd>
</dl>

<strong>Exemplos</strong>:

Crie um ID de serviço com o nome de serviço `sample-test` e a descrição `hello, world!`

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
Atualizar um ID de serviço

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do serviço</dd>
  <dt>-n, --name</dt>
  <dd>Novo nome do serviço</dd>
  <dt>-d, --description</dt>
  <dd>Nova descrição do serviço</dd>
  <dt>-v, --version</dt>
  <dd>Versão do ID de serviço</dd>
  <dt>-f, --force</dt>
  <dd>Atualizar sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Renomeie o ID de serviço `sample-test` para `sample-test-2` sem confirmação

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

Atualize a descrição de serviço `sample-test` versão `1-0jn39fbefew`

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

Excluir um ID de serviço

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do serviço</dd>
  <dt>-f, --force</dt>
  <dd>Excluir sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Exclua o ID de serviço `sample-teset` sem confirmação

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

Listar todas as chaves API da plataforma do Bluemix

```
bluemix iam api-keys
```

<strong>Pré-requisitos</strong>: Terminal, Login

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

Criar uma nova chave API da Plataforma do Bluemix

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>NAME (necessário)</dt>
<dd>Nome da chave API a ser criada.</dd>
<dt>-d <i>DESCRIPTION</i> (opcional)</dt>
<dd>Descrição da chave de API</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>Salve as informações da chave API para o arquivo especificado. Se não configuradas, o conteúdo JSON será exibido.</dd>
</dl>

<strong>Exemplos</strong>:

Crie uma chave API e salve em um arquivo

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Atualizar uma chave API da plataforma do Bluemix

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>NAME (necessário)</dt>
<dd>O nome antigo da chave API a ser atualizada.</dd>
<dt>-n <i>NAME</i> (opcional)</dt>
<dd>O nome novo da chave API</dd>
<dt>-d <i>DESCRIPTION</i> (opcional)</dt>
<dd>A nova descrição da chave API</dd>
</dl>

<strong>Exemplos</strong>:

Atualize a descrição de uma chave API:

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Excluir uma chave API da plataforma do Bluemix

```
bluemix iam api-key-delete NAME [-f]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>NAME (necessário)</dt>
<dd>Nome da chave API a ser excluída.</dd>
<dt>-f (opcional)</dt>
<dd>Force a exclusão sem confirmação.</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

Listar todas as chaves API de serviço

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
</dl>

<strong>Exemplos</strong>:

Liste as chaves API de serviço ligadas ao CRN de serviço `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

Listar detalhes de uma chave API de serviço

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Exibir o UUID da chave API de serviço</dd>
</dl>

<strong>Exemplos</strong>:

Mostre detalhes da chave API de serviço `sample-key` ligada ao CRN de serviço `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

Criar uma chave API de serviço

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-d, --description</dt>
  <dd>Descrição da chave de API</dd>
  <dt>-f, --file</dt>
  <dd>Salve as informações da chave API para o arquivo especificado. Se não configuradas, o conteúdo JSON será exibido.</dd>
</dl>

<strong>Exemplos</strong>:

Crie uma chave API de serviço `sample-key` ligada ao CRN de serviço `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

Atualizar uma chave API de serviço

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-n, --name</dt>
  <dd>Novo nome da chave API de serviço</dd>
  <dt>-d, --description</dt>
  <dd>Nova descrição da chave API de serviço</dd>
  <dt>-v, --version</dt>
  <dd>Versão da chave API de serviço</dd>
  <dt>-f, --force</dt>
  <dd>Atualizar sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Renomeie a chave API de serviço `sample-key` para `new-sample-key`:

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

Excluir uma chave API de serviço

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Excluir sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Exclua a chave API de serviço `sample-key`:

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

Listar as políticas do usuário `name@example.com`:

```
bluemix iam user-policies name@example.com
```

<strong>Pré-requisitos</strong>: terminal, login, conta de destino

<strong>Opções de comando</strong>:
<dl>
<dt>USER_NAME ((necessário))</dt>
<dd>Nome do usuário ao qual as políticas pertencem</dd>
</dl>

<strong>Exemplos</strong>:

Listar as políticas do usuário `name@example.com`:

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

Exibir detalhes de uma política do usuário

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>Pré-requisitos</strong>: terminal, login, conta de destino

<strong>Opções de comando</strong>:
<dl>
<dt>USER_NAME ((necessário))</dt>
<dd>Nome do usuário ao qual a política pertence</dd>
<dt>POLICY_ID (necessário)</dt>
<dd>ID da política</dd>
</dl>

<strong>Exemplos</strong>:

Liste a política `0bb730daa` do usuário `name@example.com`:

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

Criar uma política do usuário

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>Pré-requisitos</strong>: terminal, login, conta de destino

<strong>Opções de comando</strong>:
<dl>
<dt>USER_NAME ((necessário))</dt>
<dd>Nome do usuário ao qual a política pertence</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Arquivo JSON de definição de política</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (opcional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (opcional)</dt>
<dd>Nome do serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (opcional)</dt>
<dd>Instância de serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--region <i>REGION</i> (opcional)</dt>
<dd>Região da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (opcional)</dt>
<dd>Tipo de recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (opcional)</dt>
<dd>Recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (opcional)</dt>
<dd>Nome do grupo de recursos. Isso é exclusivo com as sinalizações '-f, --file', '--resource' e '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (opcional)</dt>
<dd>ID do grupo de recursos. Isso é exclusivo com as sinalizações '-f, --file', '--resource' e '--resource-group-name'.</dd>
  <dd>Os nomes de função da definição de política. Para obter as funções suportadas de um serviço específico, execute 'bluemix iam roles --service SERVICE_NAME'. Essa opção é exclusiva com '-f, --file'.</dd>
</dl>

<strong>Exemplos</strong>:

Crie a política de usuário para o usuário `name@example.com` do arquivo JSON de política `policy.json`:

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

Dê a `name@example.com` a função `Administrator` para todos os recursos `sample-service`:

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

Dê a `name@example.com` a função `Editor` para o recurso `key123` da instância de serviço de amostra `ServiceId-ade78e9f` na região `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Dê a `name@example.com` a função `Operator` para o grupo de recursos com ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Dê a `name@example.com` a função `Viewer` para os membros do grupo de recursos `sample-resource-group`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

Dê a `name@example.com` a função `Viewer` para os membros do grupo de recursos com ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

Atualizar uma política do usuário

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>Pré-requisitos</strong>: terminal, login, conta de destino

<strong>Opções de comando</strong>:
<dt>USER_NAME ((necessário))</dt>
<dd>Nome do usuário ao qual a política pertence</dd>
<dt>POLICY_ID (necessário)</dt>
<dd>ID da política a ser atualizada</dd>
<dt>-v, --version <i>VERSION</i> (opcional)</dt>
<dd>Versão da política existente</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Arquivo JSON de definição de política</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Arquivo JSON de definição de política</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (opcional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (opcional)</dt>
<dd>Nome do serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (opcional)</dt>
<dd>Instância de serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--region <i>REGION</i> (opcional)</dt>
<dd>Região da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (opcional)</dt>
<dd>Tipo de recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (opcional)</dt>
<dd>Recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (opcional)</dt>
<dd>Nome do grupo de recursos. Isso é exclusivo com as sinalizações '-f, --file', '--resource' e '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (opcional)</dt>
<dd>ID do grupo de recursos. Isso é exclusivo com as sinalizações '-f, --file', '--resource' e '--resource-group-name'.</dd>
  <dd>Os nomes de função da definição de política. Para obter as funções suportadas de um serviço específico, execute 'bluemix iam roles --service SERVICE_NAME'. Essa opção é exclusiva com '-f, --file'.</dd>
</dl>

<strong>Exemplos</strong>:

Atualize a política de usuário com aquela do arquivo JSON

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

Atualize a política de usuário para dar a `name@example.com` a função `Administrator` para todos os recursos `sample-service`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 Atualize a política de usuário para dar a `name@example.com` a função `Editor` para o recurso `key123` da instância de serviço de amostra `ServiceId-ade78e9f` na região `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Atualize a política de usuário para dar a `name@example.com` a função `Operator` para o grupo de recursos com ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Atualize a política de usuário para dar a `name@example.com` a função `Viewer` para os membros do grupo de recursos `sample-resource-group`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

Atualize a política de usuário para dar a `name@example.com` a função `Viewer` para membros do grupo de recursos com ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

Listar todas as políticas de serviço do serviço especificado

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necessário)</dt>
  <dd>Nome do ID de serviço</dd>
  <dt>-json</dt>
  <dd>Exibir a política no formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Exibir políticas de serviço sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Liste políticas do serviço `test`:

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

Exibir detalhes de uma política de serviço

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necessário)</dt>
  <dd>Nome do ID de serviço</dd>
  <dt>POLICY_ID (necessário)</dt>
  <dd>ID da política de serviço<dd>
  <dt>-json</dt>
  <dd>Exibir a política no formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Exibir política de serviço sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Mostre a política `140798e2-8ea7db3` do serviço `test`:

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

Criar uma política de serviço

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necessário)</dt>
  <dd>Nome do ID de serviço</dd>
  <dt>-f, --file</dt>
  <dd>Arquivo JSON de definição de política. Isso é exclusivo com as sinalizações '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' e '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Os nomes de função da definição de política. Para obter as funções suportadas de um serviço específico, execute 'bluemix iam roles --service SERVICE_NAME'. Essa opção é exclusiva com '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nome do serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Instância de serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Região da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo de recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Criar política de serviço sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Crie a política de serviço do arquivo JSON para o serviço `test`:

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

Atualizar uma política de serviço

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necessário)</dt>
  <dd>Nome do ID de serviço</dd>
  <dt>POLICY_ID (necessário)</dt>
  <dd>ID da política de serviço<dd>
  <dt>-v, --version</dt>
  <dd>Versão da política de serviço</dd>
  <dt>-f, --file</dt>
  <dd>Arquivo JSON de definição de política. Isso é exclusivo com as sinalizações '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' e '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Os nomes de função da definição de política. Para obter as funções suportadas de um serviço específico, execute 'bluemix iam roles --service SERVICE_NAME'. Essa opção é exclusiva com '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nome do serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Instância de serviço da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Região da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo de recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Recurso da definição de política. Isso é exclusivo com a sinalização '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Atualizar a política de serviço sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Atualize a política de serviço `140798e2-8ea7db3` do arquivo JSON para o serviço `test`:

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

Excluir uma política de serviço

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necessário)</dt>
  <dd>Nome do ID de serviço</dd>
  <dt>POLICY_ID (necessário)</dt>
  <dd>ID da política de serviço<dd>
  <dt>-f, --force</dt>
  <dd>Excluir sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Exclua a política `140798e2-8ea7db3` do serviço `test`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

Listar grupos de recursos

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>--default</dt>
  <dd>Obter grupo padrão da conta atual</dd>
  <dt>-r, --resource</dt>
  <dd>ID do recurso pertencente</dd>
  <dt>-o, --resource-origin</dt>
  <dd>Origem de recurso pertencente. Valores aceitos: 'CF_ORG', 'IMS_ACCOUNT'.</dd>
</dl>

<strong>Exemplos</strong>:

Liste todos os grupos de recursos sob a conta destinada atualmente:

```
bluemix resource groups
```

Liste o grupo padrão da conta destinada atualmente:

```
bluemix resource groups --default
```

Liste os grupos de recursos que são o mapeamento de uma organização CloudFoundry

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

Mostrar detalhes de um grupo de recursos

```
bluemix resource group NAME [--id]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do grupo de recursos</dd>
  <dt>--id</dt>
  <dd>Mostrar somente o ID</dd>
</dl>

<strong>Exemplos</strong>:

Mostre o grupo de recursos `example-group`:

```
bluemix resource group example-group
```

Mostre apenas o ID do grupo de recursos `example-group`:

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

Atualizar um grupo de recursos existente

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome do grupo de recursos de destino</dd>
  <dt>-n, --name</dt>
  <dd>Novo nome do grupo de recursos</dd>
  <dt>-q, --quota</dt>
  <dd>Nome da nova definição de cota</dd>
  <dt>-f</dt>
  <dd>Forçar atualização sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:

Renomeie o grupo de recursos `example-group` para `trial-group`:

```
bluemix resource group-update example-group -n trial-group
```

Mude a cota do grupo de recursos `example-group` para `free`:

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

Listar todas as definições de cota

```
bluemix resource quotas
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
</dl>

<strong>Exemplos</strong>:

Liste todas as definições de cota:

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

Mostrar detalhes de uma definição de cota

```
bluemix resource quota NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome da cota</dd>
</dl>

<strong>Exemplos</strong>:
mostre detalhes da cota `free`:

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

Esse comando tem a mesma função e opções que o comando `cf push`.


## bluemix app list
{: #bluemix_app_list}

Esse comando tem a mesma função e opções que o comando `cf apps`.


## bluemix app show
{: #bluemix_app_show}

Esse comando tem a mesma função e opções que o comando `cf app`.


## bluemix app delete
{: #bluemix_app_delete}

Esse comando tem a mesma função e opções que o comando `cf delete`.


## bluemix app rename
{: #bluemix_app_rename}

Esse comando tem a mesma função e opções que o comando `cf rename`.


## bluemix app start
{: #bluemix_app_start}

Esse comando tem a mesma função e opções que o comando `cf start`.


## bluemix app stop
{: #bluemix_app_stop}

Esse comando tem a mesma função e opções que o comando `cf stop`.


## bluemix app restart
{: #bluemix_app_restart}

Esse comando tem a mesma função e opções que o comando `cf restart`.


## bluemix app restage
{: #bluemix_app_restage}


Esse comando tem a mesma função e opções que o comando `cf restage`.


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


Esse comando tem a mesma função e opções que o comando `cf restart-app-instance`.


## bluemix app events
{: #bluemix_app_events}

Esse comando tem a mesma função e opções que o comando `cf events`.


## bluemix app files
{: #bluemix_app_files}

Esse comando tem a mesma função e opções que o comando `cf files`.


## bluemix app logs
{: #bluemix_app_logs}

Esse comando tem a mesma função e opções que o comando `cf logs`.


## bluemix app env
{: #bluemix_app_env}

Esse comando tem a mesma função e opções que o comando `cf env`.


## bluemix app env-set
{: #bluemix_app_env_set}

Esse comando tem a mesma função e opções que o comando `cf set-env`.


## bluemix app env-unset
{: #bluemix_app_env_unset}

Esse comando tem a mesma função e opções que o comando `cf unset-env`.


## bluemix app stacks
{: #bluemix_app_stacks}

Esse comando tem a mesma função e opções que o comando `cf stacks`.


## bluemix app stack-show
{: #bluemix_app_stack_show}

Esse comando tem a mesma função e opções que o comando `cf stack`.


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

Esse comando tem a mesma função e opções que o comando `cf create-app-manifest`.

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

Liste as informações de certificado de um domínio.

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
<dl>
<dt>DOMAIN_NAME (necessário)</dt>
<dd>O domínio que hospeda o certificado.</dd>
</dl>


<strong>Exemplos</strong>:

Visualize as informações de certificado do domínio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

Inclua um certificado no domínio especificado na organização atual.

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
   <dl>
   <dt>DOMAIN (necessário)</dt>
   <dd>O domínio no qual o certificado é incluído.</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i> (necessário)</dt>
   <dd>O caminho de arquivo de chave privado.</dd>
   <dt>-c <i>CERT_FILE</i> (necessário)</dt>
   <dd>O caminho de arquivo de certificado.</dd>
   <dt>-p <i>PASSWORD</i> (opcional)</dt>
   <dd>A senha para o certificado.</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i> (opcional)</dt>
   <dd>O caminho de arquivo de certificado intermediário.</dd>
   <dt>-t <i>TRUST_STORE_FILE</i> (opcional)</dt>
   <dd>O arquivo de armazenamento confiável.</dd>
   </dl>


<strong>Exemplos</strong>:

Inclua um certificado no domínio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

Remova um certificado do domínio especificado na organização atual.

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:

   <dl>
   <dt>DOMAIN (necessário)</dt>
   <dd>Domínio do qual remover o certificado.</dd>
   <dt>-f (opcional)</dt>
   <dd>Force a exclusão sem confirmação.</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

Esse comando tem a mesma função e opções que o comando `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Esse comando tem a mesma função e opções que o comando `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Esse comando tem a mesma função e opções que o comando `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-shared-domain`.

## bluemix app routes
{: #bluemix_app_routes}

Esse comando tem a mesma função e opções que o comando `cf routes`.


## bluemix app route-check
{: #bluemix_app_route_check}

Esse comando tem a mesma função e opções que o comando `cf check-route`.


## bluemix app route-map
{: #bluemix_app_route_map}

Mapeie uma rota para um aplicativo cf ou grupo de contêiner existente que tenha o domínio e o nome do host especificados.

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (obrigatório)</dt>
   <dd>O nome do aplicativo cf ou grupo de contêiner a ser mapeado com uma rota.</dd>
   <dt>DOMAIN (necessário)</dt>
   <dd>O domínio da rota. Por exemplo, mychinabluemix.net ou chinabluemix.net. </dd>
   <dt>-n <i>HOST_NAME</i> (opcional)</dt>
   <dd>O nome do host da rota. Se não fornecido, o nome do host será configurado para o nome do app ou grupo de contêiner por padrão.</dd>
   </dl>

<strong>Exemplos</strong>:

Mapeie uma rota para `my-app` com o domínio especificado:

```
bluemix app route-map my-app mychinabluemix.net
```

Mapeie uma rota para 'my-container-group' com o domínio e nome do host especificados:

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

Remova o mapeamento da rota especificada de um aplicativo cf ou grupo de contêiner existente.

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (obrigatório)</dt>
   <dd>O nome do aplicativo cf ou grupo de contêiner.</dd>
   <dt>DOMAIN (necessário)</dt>
   <dd>O domínio da rota (por exemplo, mychinabluemix.net ou chinabluemix.net).</dd>
   <dt>-n <i>HOST_NAME</i> (opcional)</dt>
   <dd>O nome do host da rota. Se não fornecido, o nome do host será configurado para o nome do app ou grupo de contêiner por padrão.</dd>
   </dl>

<strong>Exemplos</strong>:

Remover o mapeamento `my-app.mychinabluemix.net` de `my-app`:

```
bluemix app route-unmap my-app mychianbluemix.net
```

Remover o mapeamento `abc.chinabluexmix.net` de `my-container-group`:

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

Esse comando tem a mesma função e opções que o comando `cf create-route`.


## bluemix app route-delete
{: #bluemix_app_route_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-route`.


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-orphaned-routes`.


## bluemix app domains
{: #bluemix_app_domains}

Esse comando tem a mesma função e opções que o comando `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Esse comando tem a mesma função e opções que o comando `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Esse comando tem a mesma função e opções que o comando `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-shared-domain`.


## bluemix service offerings
{: #bluemix_service_offerings}


Esse comando tem a mesma função e opções que o comando `cf marketplace`.


## bluemix service list
{: #bluemix_service_list}

Esse comando tem a mesma função e opções que o comando `cf services`.


## bluemix service show
{: #bluemix_service_show}

Esse comando tem a mesma função e opções que o comando `cf service`.


## bluemix service create
{: #bluemix_service_create}

Esse comando tem a mesma função e opções que o comando `cf create-service`.


## bluemix service update
{: #bluemix_service_update}

Esse comando tem a mesma função e opções que o comando `cf update-service`.


## bluemix service delete
{: #bluemix_service_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-service`.


## bluemix service rename
{: #bluemix_service_rename}

Esse comando tem a mesma função e opções que o comando `cf rename-service`.


## bluemix service bind
{: #bluemix_service_bind}

Esse comando tem a mesma função e opções que o comando `cf bind-service`.


## bluemix service unbind
{: #bluemix_service_unbind}

Esse comando tem a mesma função e opções que o comando `cf unbind-service`.


## bluemix service key-create
{: #bluemix_service_key_create}

Esse comando tem a mesma função e opções que o comando `cf create-service-key`.


## bluemix service key-delete
{: #bluemix_service_key_delete}

Esse comando tem a mesma função e opções que o comando `cf delete-service-key`.


## bluemix service keys
{: #bluemix_service_keys}

Esse comando tem a mesma função e opções que o comando `cf service-keys`.


## bluemix service key-show
{: #bluemix_service_key_show}

Esse comando tem a mesma função e opções que o comando `cf service-key`.


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

Esse comando tem a mesma função e opções que o comando `cf create-user-provided-service`.


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

Esse comando tem a mesma função e opções que o comando `cf update-user-provided-service`.


## bluemix resource instances
{: #bluemix_resource_instances}

Listar instâncias de recursos

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>--resource-name</dt>
  <dd>Nome do recurso pertencente</dd>
  <dt>-r, --region</dt>
  <dd>Filtrar por ID da região, padrão para a região atual, se não especificado, '-r, --region all' para exibir as instâncias de recursos em todas as regiões</dd>
  <dt>--long</dt>
  <dd>Mostrar campos adicionais na saída</dd>
</dl>

<strong>Exemplos</strong>:

Liste as instâncias de recursos do recurso `test-resource`:

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

Mostrar detalhes de uma instância de recurso

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome da instância de recurso</dd>
  <dt>-r, --region</dt>
  <dd>Filtrar por ID da região, padrão para a região atual, se não especificado, '-r, --region all' para exibir as instâncias de recursos em todas as regiões</dd>
  <dt>--id</dt>
  <dd>Exibir o ID de instância de recurso</dd>
</dl>

<strong>Exemplos</strong>:
mostre detalhes da instância de recurso `my-resource-instance`:

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

Criar uma instância de recurso

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NAME (necessário)</dt>
  <dd>Nome da instância de recurso</dd>
  <dt>RESOURCE_NAME ou RESOURCE_ID (necessário)</dt>
  <dd>Nome ou ID do recurso</dd>
  <dt>RESOURCE_PLAN_NAME ou RESOURCE_PLAN_ID (necessário)</dt>
  <dd>Nome ou ID do plano de recursos</dd>
  <dt>-r, --region</dt>
  <dd>Região para criar a instância de recurso, padrão para a região atual, se não especificada</dd>
  <dt>-t, --tags</dt>
  <dd>Tags</dd>
  <dt>-p, --parameters</dt>
  <dd>Arquivo JSON ou sequência JSON de parâmetros para criar a instância de recurso</dd>
</dl>

<strong>Exemplos</strong>:
crie uma instância de recurso chamada `my-resource-instance` usando o plano de recursos `test-resource-plan` do recurso `test-resource`:

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

Atualizar a instância de recurso

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>RESOURCE_INSTANCE_NAME (necessário)</dt>
  <dd>Nome da instância de recurso</dd>
  <dt>-n, --name</dt>
  <dd>Nome da nova instância de recurso</dd>
  <dt>-t, --tags</dt>
  <dd>Novas tags</dd>
  <dt>--resource-plan-id</dt>
  <dd>ID do novo plano de recursos</dd>
  <dt>--update-time</dt>
  <dd>Tempo em segundos desde a época em que o registro debitável deve entrar em vigor</dd>
  <dt>-f, --force</dt>
  <dd>Forçar atualização sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
atualize a instância de recurso `my-resource-instance`, mude seu nome para `new-resource-instance`:

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

Excluir a instância de recurso

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Forçar exclusão sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
exclua a instância de recurso `my-resource-instance`:

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

Mostrar ligações para o alias do recurso

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>RESOURCE_ALIAS (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
</dl>

<strong>Exemplos</strong>:
mostre as ligações de recursos para o alias do recurso `my-resource-alias`:

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

Mostrar detalhes de uma ligação de recurso

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>APP_NAME</dt>
  <dd>Nome do aplicativo CloudFoundry</dd>
  <dt>--id</dt>
  <dd>Exibir somente o ID. Todas as outras saídas para a ligação de recursos são suprimidas.</dd>
</dl>

<strong>Exemplos</strong>:
mostre detalhes da ligação de recurso entre o alias de recurso `my-resource-alias` e o app `my-app`:

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

Criar uma ligação de recurso

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>APP_NAME</dt>
  <dd>Nome do aplicativo CloudFoundry</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nome da função de usuário</dd>
  <dt>--service-id-name</dt>
  <dd>Nome do ID de serviço ao qual a função pertence</dd>
  <dt>-f, --force</dt>
  <dd>Forçar a criação sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
crie ligações de um recurso entre o alias de recurso `my-resource-alias` e o app `my-app` com a função `Administrator`:

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

Excluir uma ligação do recurso

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>APP_NAME</dt>
  <dd>Nome do aplicativo CloudFoundry</dd>
  <dt>-f, --force</dt>
  <dd>Forçar exclusão sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
exclua a ligação de recurso entre o alias de recurso `my-resource-alias` e o app `my-app`:

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

Listar chaves de recursos de instância de recurso ou de alias de recurso

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID da instância de recurso</dd>
  <dt>--instance-name</dt>
  <dd>Nome da instância de recurso</dd>
  <dt>--alias-id</dt>
  <dd>ID do alias do recurso</dd>
  <dt>--alias-name</dt>
  <dd>Nome do alias do recurso</dd>
</dl>

<strong>Exemplos</strong>:
liste as chaves de recursos da instância de recurso `my-resource-instance`:

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

Mostrar detalhes de uma chave de recursos

```
bluemix resource key KEY_NAME [--id]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nome da chave</dd>
  <dt>--id</dt>
  <dd>Exibir o ID de chave de recursos</dd>
</dl>

<strong>Exemplos</strong>:
mostre detalhes das chaves de recursos `my-resource-key`:

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

Criar uma chave de recursos

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>NOME</dt>
  <dd>Nome da chave</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nome da função de usuário</dd>
  <dt>--instance-id</dt>
  <dd>ID da instância de recurso</dd>
  <dt>--instance-name</dt>
  <dd>Nome da instância de recurso</dd>
  <dt>--alias-id</dt>
  <dd>ID do alias do recurso</dd>
  <dt>--alias-name</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>-service-id-name</dt>
  <dd>Nome do ID de serviço ao qual a função pertence</dd>
  <dt>-f, --force</dt>
  <dd>Forçar a criação sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
crie uma chave de recurso chamada `my-resource-key` com a função `Administrator` para a instância de recurso `my-resource-instance`:

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

Excluir uma chave de recursos

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nome da chave</dd>
  <dt>-f, --force</dt>
  <dd>Forçar exclusão sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
exclua a chave de recursos `my-resource-key`:

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

Listar aliases para uma instância de recurso

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID da instância de recurso pertencente.</dd>
  <dt>--instance-name</dt>
  <dd>Nome da instância de recurso pertence.</dd>
</dl>

<strong>Exemplos</strong>:
liste os aliases de recurso para a instância de recurso `my-resource-instance`:
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

Mostrar detalhes de um alias do recurso

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>--id</dt>
  <dd>Exibir somente o ID do alias de recurso especificado. Todas as outras saídas para o alias são suprimidas.</dd>
</dl>

<strong>Exemplos</strong>:
mostre detalhes do alias de recurso `my-resource-alias`:
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

Criar um alias de uma instância de recurso

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>--instance-id</dt>
  <dd>ID da instância de recurso pertencente.</dd>
  <dt>--instance-name</dt>
  <dd>Nome da instância de recurso pertence.</dd>
  <dt>-s</dt>
  <dd>Nome do espaço em que o alias foi criado. O padrão é o espaço atual.</dd>
  <dt>-t, --tags</dt>
  <dd>Lista de marcações.</dd>
  <dt>-p, --parameters</dt>
  <dd>Arquivo JSON ou sequência JSON de parâmetros.</dd>
</dl>

<strong>Exemplos</strong>:
crie um alias de recurso chamado `my-resource-alias` da instância de recurso `my-resource-instance`:
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

Atualizar um alias do recurso

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>-n, --name</dt>
  <dd>Novo nome do alias do recurso.</dd>
  <dt>-t, --tags</dt>
  <dd>Lista de marcações.</dd>
  <dt>-p, --parameters</dt>
  <dd>Arquivo JSON ou sequência JSON de parâmetros.</dd>
  <dt>-f, --force</dt>
  <dd>Forçar atualização sem confirmação do usuário.</dd>
</dl>

<strong>Exemplos</strong>:
atualize o alias de recurso `my-resource-alias`, mude seu nome para `new-resource-alias`:

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

Excluir um alias do recurso

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>ALIAS_NAME (necessário)</dt>
  <dd>Nome do alias do recurso</dd>
  <dt>-f, --force</dt>
  <dd>Forçar exclusão sem confirmação</dd>
</dl>

<strong>Exemplos</strong>:
exclua o alias de recurso `my-resource-alias`:

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

Procurar entradas no catálogo

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-q, --query</dt>
  <dd>Procurar a palavra-chave</dd>
  <dt>-r, --region</dt>
  <dd>Especificar a região geográfica na qual procurar. Atualmente, apenas "us-south" e "united-kingdom" são suportados</dd>
  <dt>-k, --kind</dt>
  <dd>Filtrar pelo tipo de recursos. Atualmente, apenas "service-cf", "iaas", "runtime", "template" e "dashboard" são suportados</dd>
  <dt>-p, --price</dt>
  <dd>Filtrar pelo preço. Atualmente, apenas "free", "paygo", "bluemix-subscription" são suportados</dd>
  <dt>-t, --tag</dt>
  <dd>Filtrar pela tag.</dd>
  <dt>-sort-by</dt>
  <dd>Propriedade pela qual classificar</dd>
  <dt>-reverse</dt>
  <dd>Se a ordem de classificação deve ser revertida</dd>
  <dt>-json</dt>
  <dd>Resposta JSON original da saída</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Procure o serviço `Automation test`:

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

Obter uma entrada no catálogo

```
bluemix catalog entry [-i ID] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>O ID da entrada no catálogo.</dd>
  <dt>-children</dt>
  <dd>Obter todos os filhos da entrada no catálogo</dd>
  <dt>-json</dt>
  <dd>Resposta JSON original da saída</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Obtenha a entrada com ID `a0ef1-d3b4j0`:

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
Criar uma nova entrada no catálogo (administrador do catálogo de uma conta somente)

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-p, --parent</dt>
  <dd>ID-pai do objeto</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido contendo parâmetros de configuração específicos do catálogo, fornecido sequencialmente ou em um arquivo. Para obter uma lista de parâmetros de configuração suportados, veja a documentação para a entrada no catálogo específica.</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Crie o recurso do arquivo JSON com o ID pai `a0ef1-d3b4j0`:

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
Atualizar uma entrada no catálogo existente (administrador do catálogo ou editor de uma conta somente)

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>O ID da entrada no catálogo que está sendo atualizada.</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido contendo parâmetros de configuração específicos do catálogo, fornecido sequencialmente ou em um arquivo. Para obter uma lista de parâmetros de configuração suportados, veja a documentação para a entrada no catálogo específica.</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Atualize o recurso `j402-dnf1i` do arquivo JSON:

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
Obter a visibilidade de uma entrada no catálogo (administrador do catálogo de uma conta somente)

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>O ID da entrada no catálogo.</dd>
  <dt>-json</dt>
  <dd>Resposta JSON original da saída</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Obtenha visibilidade do recurso `j402-dnf1i` no escopo global:

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
Atualizar a visibilidade de uma entrada no catálogo existente (administrador do catálogo de uma conta somente)

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>O ID da entrada no catálogo que está sendo atualizada.</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido contendo parâmetros de configuração específicos do catálogo, fornecido sequencialmente ou em um arquivo. Para obter uma lista de parâmetros de configuração suportados, veja a documentação para a entrada no catálogo específica.</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Configure a visibilidade do recurso `j402-dnf1i` no arquivo JSON:

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
Listar ofertas de serviços no mercado de trabalho

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
<dl>
  <dt>-cf</dt>
  <dd>Mostrar serviços do Cloud Foundry somente</dd>
  <dt>-rc</dt>
  <dd>Mostrar serviços compatíveis com RC somente</dd>
  <dt>-global</dt>
  <dd>Operar no escopo global</dd>
</dl>

<strong>Exemplos</strong>:

Mostre ofertas de serviço no escopo global:

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

Visualize os modelos de modelo no Bluemix.

```
bluemix catalog templates [-d]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

   <dl>
   <dt>-d (opcional)</dt>
   <dd>Se a opção <i>-d</i> for especificada, a descrição de cada modelo também será exibida. Caso contrário, somente o ID e o nome de cada modelo serão mostrados.</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

Visualize as informações detalhadas de um modelo de modelo especificado.

```
bluemix catalog template TEMPLATE_ID
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:
   <dl>
   <dt>TEMPLATE_ID (necessário)</dt>
   <dd>O ID do modelo de modelo. Use <i>modelos bluemix</i> para visualizar todos os IDs dos modelos.</dd>
   </dl>


<strong>Exemplos</strong>:

Visualize detalhes do modelo `mobileBackendStarter`:

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

Crie um aplicativo cf que seja baseado no modelo especificado com a URL e descrição especificadas. Por padrão, o novo app é iniciado automaticamente.

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>Pré-requisitos</strong>: Terminal, Login, Destino

<strong>Opções de comando</strong>:
   <dl>
   <dt>TEMPLATE_ID (necessário)</dt>
   <dd>O modelo no qual o aplicativo será baseado quando for criado. Use <i>bluemix templates</i> para ver todos os IDs dos modelos.</dd>
   <dt>CF_APP_NAME (necessário)</dt>
   <dd>O nome do aplicativo cf a ser criado.</dd>
   <dt>-u <i>URL</i> (opcional)</dt>
   <dd>A rota do aplicativo. Se não especificada, a rota será configurada pelo Bluemix automaticamente com base em seu nome de app e domínio padrão.</dd>
   <dt>-d <i>DESCRIPTION</i> (opcional)</dt>
   <dd>Descrição do aplicativo.</dd>
   <dt>--no-start (opcional)</dt>
   <dd>Não inicie o aplicativo automaticamente após ele ser criado. Se não especificado, o aplicativo será iniciado automaticamente após ser criado.</dd>
   </dl>


<strong>Exemplos</strong>:

Crie um aplicativo cf `my-app` baseado no modelo `javaHelloWorld`:

```
bluemix catalog template-run javaHelloWorld my-app
```

Crie um aplicativo `my-ruby-app` baseado no modelo `rubyHelloWorld`
com a rota `myrubyapp.chinabluemix.net` e a descrição `My first ruby app on
{{site.data.keyword.Bluemix_notm}}.`:

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

Crie um aplicativo `my-python-app` baseado no modelo `pythonHelloWorld` sem início automático:

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

Mostrar o uso mensal e os custos de sua conta.

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

<dl>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Exibir dados para mês e especificando data usando o formato AAAA-MM. Se não especificado, o uso do mês atual será mostrado.</dd>
  <dt>--json (opcional)</dt>
  <dd>Exibir o resultado de uso em formato JSON.</dd>
</dl>

<strong>Exemplos</strong>:

Mostrar o uso da minha conta e relatório de custo em 06/2016:

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

Mostrar detalhes de uso mensal de uma organização. Essa operação pode ser executada somente por um gerente de faturamento da organização.

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

<dl>
  <dt>ORG_NAME (necessário)</dt>
  <dd>Nome da organização.</dd>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Exibir dados para mês e data especificada usando o formato AAAA-MM. Se não especificado, o uso do mês atual será mostrado.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nome da região que hospeda a organização. Se configurado como 'all', o uso da organização em todas as regiões será mostrado.</dd>
  <dt>--json (opcional)</dt>
  <dd>Exibir o resultado de uso em formato JSON.</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

Mostrar o resumo de uso mensal para organizações na minha conta.

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Pré-requisitos</strong>: Terminal, Login

<strong>Opções de comando</strong>:

<dl>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Exibir dados para mês e data especificada usando o formato AAAA-MM. Se não especificado, o uso do mês atual será mostrado.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nome da região que hospeda as organizações. Se configurado como 'all', o resumo de uso das organizações em todas as regiões será mostrado.</dd>
  <dt>--json (opcional)</dt>
  <dd>Exibir o resultado de uso em formato JSON.</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

Liste todos os repositórios de plug-in que estão registrados na CLI do {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repos
```

<strong>Pré-requisitos</strong>: Nenhum


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

Inclua um novo repositório de plug-in na CLI do {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>REPO_NAME (necessário)</dt>
   <dd>O nome do repositório a ser incluído. É possível definir seu próprio nome para cada repositório.</dd>
   <dt>REPO_URL (necessário)</dt>
   <dd>A URL do repositório a ser incluído. A URL do repositório deve conter o protocolo (por exemplo, http://plugins.ng.bluemix.net em vez de plugins.ng.bluemix.net). http://plugins.ng.bluemix.net é o repositório de plug-in oficial da CLI do Bluemix.</dd>
    </dl>


<strong>Exemplos</strong>:

Inclua o repositório de plug-in oficial da CLI do Bluemix CLI como `bluemix-repo`:

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

Remova um repositório de plug-in da CLI do {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-remove REPO_NAME
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
   <dl>
   <dt>REPO_NAME (necessário)</dt>
   <dd>O nome do repositório a ser removido.</dd>
   </dl>

<strong>Exemplos</strong>:

Remova o repositório `bluemix-repo` da CLI do {{site.data.keyword.Bluemix_notm}}:

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

Liste todos os plug-ins disponíveis em todos os repositórios incluídos ou um repositório específico.

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>Liste somente os plug-ins no repositório especificado.</dd>
   </dl>

<strong>Exemplos</strong>:

Liste todos os plug-ins em todos os repositórios incluídos:

```
bluemix plugin repo-plugins
```

Liste todos os plug-ins no repositório `bluemix-repo`:

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

Mostrar os detalhes de um plug-in no repositório.

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>O nome do repositório. Se nenhum repositório for especificado, o comando usará o plug-in padrão repository.å</dd>
   </dl>

<strong>Exemplos</strong>:

Liste detalhes do plug-in "IBM-Containers" no repositório "sample-repo":

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

Listar detalhes do plug-in "IBM-Containers" no repositório padrão

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

Liste todos os plug-ins instalados na CLI do {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin list
```

<strong>Pré-requisitos</strong>: Nenhum

## bluemix plugin show
{: #bluemix_plugin_show}

Mostrar detalhes de um plug-in instalado

```
bluemix plugin show PLUGIN-NAME
```

<strong>Pré-requisitos</strong>: Nenhum


## bluemix plugin install
{: #bluemix_plugin_install}

Instale a versão específica de plug-in na CLI do {{site.data.keyword.Bluemix_notm}} a partir do caminho ou repositório especificado.

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME (obrigatório)</dt>
   <dd>Se -r <i>REPO_NAME</i> não for especificado, o plug-in será instalado a partir do caminho local especificado ou da URL remota.</dd>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>O nome do repositório no qual o binário do plug-in está localizado. Se nenhum repositório for especificado, o comando usará o repositório de plug-in padrão.</dd>
   <dt>-v <i>VERSION</i> (opcional)</dt>
   <dd>A versão do plug-in a ser instalado. Se ela não for fornecida, a versão mais recente do plug-in será instalada. Essa opção é válida somente quando você instala o plug-in a partir do repositório.</dd>
    </dl>

<strong>Exemplos</strong>:

Instale um plug-in a partir do arquivo local:

```
bluemix plugin install /downloads/new_plugin
```

Instale um plug-in a partir da URL remota:

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

Instale o plug-in `IBM-Containers` da versão mais recente do repositório `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
Instale o plug-in `IBM-Containers` com a versão `0.5.800` do repositório `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

Faça upgrade do plug-in de um repositório

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>Nome do plug-in a ser atualizado. Se não especificado, o comando verificará os upgrades de todos os plug-ins instalados.</dd>
 <dt>-r REPO_NAME</dt>
 <dd>O nome do repositório no qual o binário do plug-in está localizado. Se não especificado, o comando usará o repositório de plug-in padrão.</dd>
 <dt>-v <i>VERSION</i> (opcional)</dt>
 <dd>A versão do plug-in para a qual ele será atualizado. Se não fornecida, atualize o plug-in para a versão mais recente disponível.</dd>
 <dt>--all</dt>
 <dd>Atualizar todos os plug-ins disponíveis</dd>
</dl>

<strong>Exemplos</strong>:

Procure todos os upgrades disponíveis no repositório de plug-in "My-Repo":

```
bluemix plugin update -r My-Repo
```

Faça upgrade do plug-in "plugin-echo" no repositório "My-Repo" para o mais recente:

```
bluemix plugin update -r My-Repo plugin-echo
```

Atualize o plug-in "plugin-echo" no repositório "My-Repo" para a versão "1.0.1":

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

Desinstale o plug-in especificado a partir da CLI do {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>Pré-requisitos</strong>: Nenhum

<strong>Opções de comando</strong>:

   <dl>
   <dt>PLUGIN_NAME (necessário)</dt>
   <dd>O nome do plug-in a ser desinstalado.</dd>
    </dl>

<strong>Exemplos</strong>:

Desinstale o plug-in `IBM-Containers` que foi instalado anteriormente:

```
bluemix plugin uninstall IBM-Containers
```

