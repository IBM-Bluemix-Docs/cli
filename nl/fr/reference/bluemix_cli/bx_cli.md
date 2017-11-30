---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Commandes {{site.data.keyword.Bluemix_notm}} (bx)
{: #bluemix_cli}

Version : 0.6.1

L'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} fournit un ensemble de commandes qui sont regroupées par espace de nom pour que les utilisateurs puissent interagir avec {{site.data.keyword.Bluemix_notm}}. 

A compter de la version 0.5.0, le client de ligne de commande {{site.data.keyword.Bluemix_notm}} inclut un client de ligne de commande Cloud Foundry dans son installation. Si vous disposez de votre propre installation d'interface CLI cf, n'utilisez pas en même temps les commandes CLI {{site.data.keyword.Bluemix_notm}} `bx [command]` et les commandes CLI Cloud Foundry `cf [command]` de votre installation dans le même contexte. A la place, exécutez `bluemix cf [command]` si vous souhaitez utiliser l'interface CLI cf pour gérer des ressources Cloud Foundry dans le contexte CLI {{site.data.keyword.Bluemix_notm}}.  De plus, `bluemix cf api/login/logout/target` n'est pas admis, utilisez `bluemix api/login/logout/target` à la place.

Les listes ci-dessous répertorient la syntaxe des commandes prises en charge par l'interface CLI {{site.data.keyword.Bluemix_notm}}, en indiquant leurs noms, leurs arguments, leurs options, leurs prérequis, leurs descriptions, et des exemples.
{:shortdesc}

**Remarque :** la zone *Prérequis* répertorie les actions qui sont requises avant l'utilisation de la commande. Les commandes pour lesquelles aucune action n'est requise indiquent **Aucun**. Sinon, les prérequis peuvent inclure une ou plusieurs des actions suivantes :

<dl>
<dt>Noeud final</dt>
<dd>Un noeud final d'API doit être défini via <code>bluemix api</code> avant l'utilisation de la commande.</dd>
<dt>Connexion</dt>
<dd>La connexion avec la commande <code>bluemix login</code> est requise avant l'utilisation de cette commande.
Si vous vous connectez avec un ID fédéré, utilisez l'option '--sso' pour vous authentifier avec un code d'accès unique ou utilisez l'option '--apikey' pour vous authentifier avec une clé d'API. Dans la console {{site.data.keyword.Bluemix_notm}}, sélectionnez **Gérer** &gt; **Sécurité** &gt; **Clés d'API Bluemix** pour créer des clés d'API.
</dd>
<dt>Cible</dt>
<dd>La commande <code>bluemix target</code> doit être utilisée pour définir une organisation et un espace avant l'utilisation de cette commande.</dd>
<dt>Docker</dt>
<dd>L'interface de ligne de commande Docker (docker) doit être installée pour que vous puissiez exécuter cette commande.</dd>
</dl>

**Remarque :** vous pouvez utiliser le format abrégé
des commandes Bluemix. Par exemple, `bx api` est la forme
abrégée de `bluemix api`.

Utilisez les index des tableaux suivants pour examiner les commandes Bluemix fréquemment utilisées.

## Commandes générales Bluemix 
{: #bx_commands_index}

<table summary="Commandes générales Bluemix.">
<caption>Tableau 1. Commandes générales Bluemix</caption>
 <thead>
 <th colspan="5">Commandes générales Bluemix</th>
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
 
 ## Commandes de gestion et de configuration des services {{site.data.keyword.BluSoftlayer_notm}}
  {: #bx_commands_softlayer}
  
Les commandes de gestion de {{site.data.keyword.BluSoftlayer_notm}}} ont été fusionnées dans l'interface de ligne de commande Bluemix. Pour plus d'informations sur l'utilisation de l'interface de ligne de commande Bluemix dans le but de configurer et gérer des services {{site.data.keyword.BluSoftlayer_notm}}, voir :  [Commandes {{site.data.keyword.BluSoftlayer_notm}} de l'interface de ligne de commande Bluemix (bluemix sl)](/docs/cli/reference/softlayer/index.md#softlayer_cli).
 
 ## Commandes de gestion des comptes, des organisations et des rôles
 {: #bx_commands_account}

<table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des comptes, des organisations, des espaces et des rôles.">
<caption>Tableau 2. Commandes de gestion des comptes, des organisations, des espaces et des rôles</caption>
 <thead>
 <th colspan="5">Commandes de gestion des comptes, des organisations, des espaces et des rôles</th>
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


 ## Commandes de gestion des groupes de ressources et des ressources
{: #bx_commands_resource}

<table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des groupes de ressources et des ressources.">
  <caption>Tableau 3. Commandes de gestion des groupes de ressources et des ressources</caption>
  <thead>
    <th colspan="5">Commandes de gestion des groupes de ressources et des ressources</th>
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

 
 ## Commandes de gestion des clés d'API et des règles
 {: #bx_commands_iam}
 <table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des clés d'API et des règles.">
 <caption>Tableau 3. Commandes de gestion des clés d'API et des règles</caption>
  <thead>
  <th colspan="5">Commandes de gestion des clés d'API et des règles</th>
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
 
 ## Commandes de gestion des applications CF et des domaines, routes et certificats liés aux applications
 {: #bx_commands_apps}

<table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des applications CF et des domaines, des routes et des certificats liés aux applications.">
<caption>Tableau 4. Commandes de gestion des applications CF et des domaines, des routes et des certificats liés aux applications</caption>
 <thead>
 <th colspan="5">Commandes de gestion des applications CF et des domaines, des routes et des certificats liés aux applications</th>
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
 
 ## Commandes pour la gestion de services Bluemix
 {: #bx_commands_services}

<table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des services Bluemix.">
<caption>Tableau 5. Commandes de gestion des services Bluemix</caption>
 <thead>
 <th colspan="5">Commandes de gestion des services Bluemix</th>
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

 
 ## Commandes de gestion des paramètres de catalogue, de plug-in et de facturation
 {: #bx_commands_settings}

<table summary="Commandes Bluemix que vous pouvez utiliser pour gérer des paramètres de catalogue, de plug-in, de facturation et de sécurité Bluemix.">
<caption>Tableau 6. Commandes de gestion des paramètres de catalogue, de plug-in, de facturation et de sécurité Bluemix</caption>
 <thead>
 <th colspan="5">Commandes de gestion des paramètres de catalogue, de plug-in, de facturation et de sécurité Bluemix</th>
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
Affichez l'aide générale pour les commandes intégrées de premier niveau et les espaces de nom pris en charge de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}, ou l'aide d'une commande intégrée ou d'un espace de nom spécifique.

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>COMMAND|NAMESPACE (facultatif))</dt>
   <dd>Commande ou espace de nom pour lequel afficher l'aide. Si la commande ou l'espace de nom n'est pas spécifié, l'aide générale de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} est affichée.</dd>
   </dl>



<strong>Exemples</strong> :

Affichez l'aide générale pour l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} :

```
bluemix help
```

Affichez l'aide pour la commande `info` :

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
Définissez ou affichez le noeud final d'API {{site.data.keyword.Bluemix_notm}}.

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
   <dl>
   <dt>API_ENDPOINT (facultatif)</dt>
   <dd>Noeud final d'API ciblé. Par exemple, `https://api.chinabluemix.net`. Si l'option *NOEUD_FINAL_API* et l'option `--unset` sont toutes les deux spécifiées, le noeud final d'API en cours est affiché.</dd>
   <dt>--unset (facultatif)</dt>
   <dd>Supprimer le paramètre de noeud final d'API.</dd>
   <dt>--skip-ssl-validation (facultatif)</dt>
   <dd>Ignorer la validation SSL des demandes HTTP.</dd>
   </dl>
<strong>Exemples</strong> :

Définissez le noeud final d'API api.chinabluemix.net :

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

Affichez le noeud final d'API en cours :

```
bluemix api
```

Annulez la définition du noeud final d'API :

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


Ecrivez les valeurs par défaut dans le fichier de configuration.

```
bluemix config --http-timeout TIMEOUT_IN_SECONDS | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDS</i></dt>
   <dd>Délai d'attente pour les demandes HTTP. La valeur par défaut est 60 secondes.</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>Consigne la trace des demandes HTTP sur le terminal ou dans le fichier spécifié.</dd>
   <dt>--color true|false</dt>
   <dd>Active ou désactive la sortie en couleurs. Elle est activée par défaut.</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>Définit un environnement local par défaut. Si LOCALE a pour valeur <i>CLEAR</i>, l'environnement local précédent est supprimé.</dd>
   <dt>--check-version true|false</dt>
   <dd>Active ou désactive la vérification de la version de l'interface de ligne de commande.</dd>
   </dl>

Une seule de ces options peut être indiquée à la fois.

<strong>Exemples</strong> :

Définissez le délai d'attente des demandes HTTP à 30 secondes :

```
bluemix config --http-timeout 30
```

Activez la sortie de trace pour les demandes HTTP :

```
bluemix config --trace true
```

Consigne la trace des demandes HTTP dans le fichier spécifié */home/usera/my_trace*:

```
bluemix config --trace /home/usera/my_trace
```

Désactivez la sortie couleur :

```
bluemix config --color false
```

Définissez l'environnement local zh_Hans :

```
bluemix config --locale zh_Hans
```

Effacez les paramètres d'environnement local :

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

Affichez les informations {{site.data.keyword.Bluemix_notm}} de base, notamment la région en cours, la version du contrôleur de cloud et certains noeuds finaux utiles tels que les noeuds finaux pour la connexion et l'échange de jeton d'accès.

```
bluemix info
```

<strong>Prérequis</strong> : Noeud final


## bluemix cf
{: #bluemix_cf}

Appeler l'interface CLI CF imbriquée

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
<dl>
  <dt>-q, --quiet</dt>
  <dd>Désactiver le message "Appel de commande cf..."</dd>
</dl>

<strong>Exemples</strong> :

Liste d'applications CF :

```
bluemix cf apps
```

Liste de services CF sans le message "Appel de commande cf...":

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

Connectez l'utilisateur. 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>Prérequis</strong> : Aucun

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>Options de commande</strong> :
<dl>
  <dt> -a <i>API_ENDPOINT</i> (facultatif)</dt>
  <dd> Noeud final de l'API (par exemple : api.ng.bluemix.net)</dd>
  <dt> --apikey <i>API_KEY ou @API_KEY_FILE_PATH</i>
  <dd> Contenu de clé d'API ou chemin d'un fichier de clés d'API indiqué par @</dd>
  <dt> --sso (facultatif) </dt>
  <dd> Utiliser un code d'accès unique pour se connecter </dd>
  <dt> -u <i>USERNAME</i> (facultatif)</dt>
  <dd> Nom d'utilisateur</dd>
  <dt> -p <i>PASSWORD</i> (facultatif)</dt>
  <dd> Mot de passe</dd>
  <dt> -c <i>ACCOUNT_ID</i> (facultatif) </dt>
  <dd> ID du compte cible</dd>
  <dt> -o <i>ORG_NAME</i> (facultatif) </dt>
  <dd> Nom de l'organisation cible </dd>
  <dt> -s <i>SPACE_NAME</i> (facultatif) </dt>
  <dd> Nom de l'espace cible</dd>
  <dt> --skip-ssl-validation (facultatif) </dt>
  <dd> Ignorer la validation SSL des demandes HTTP. Cette option n'est pas recommandée.</dd>
</dl>

<strong>Exemples</strong> :

#### Connexion en mode interactif

```
bluemix login
```

Connectez-vous avec un nom d'utilisateur et un mot de passe, puis définissez un compte, une organisation et un espace cible :

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

Connectez-vous avec un code d'accès unique et définissez un compte, une organisation et un espace cible

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

Connectez-vous avec une clé d'API et définissez des cibles :

#### Un compte est associé à une clé d'API

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### Aucun compte n'est associé à une clé d'API

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>Remarque :</strong> si un compte est associé à la clé d'API, le passage à un autre compte n'est pas autorisé.

#### Utiliser un code d'accès unique

```
bluemix login -u UserID --sso
```

L'interface de ligne de commande fournira ensuite un lien d'URL et demandera un code d'accès :
```
One Time Code (Get one at https://URL_Link_To_Obtain_Passcode):
```

Ouvrez le lien dans un navigateur et laissez-vous guider pour obtenir le code secret. Entrez le code d'accès qui vous a été fourni dans la console. Vous devriez pouvoir vous connecter.

## bluemix logout
{: #bluemix_logout}

Déconnectez l'utilisateur.

```
bluemix logout
```

<strong>Prérequis</strong> : Aucun

## bluemix regions
{: #bluemix_regions}

Affichez les informations pour toutes les régions dans {{site.data.keyword.Bluemix_notm}}.

```
bluemix regions
```

<strong>Prérequis</strong> : Noeud final


## bluemix target
{: #bluemix_target}


Définissez ou affichez le compte, la région, l'organisation ou l'espace cible :

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>-r <i>REGION_NAME</i> (facultatif)</dt>
   <dd>Nom de la région vers laquelle commuter, par exemple 'us-south' ou 'eu-gb'.</dd>
   <dt>-c <i>ACCOUNT_ID</i> (facultatif)</dt>
   <dd>ID du compte à cibler.</dd>
   <dt>--cf</dt>
   <dd>Sélectionner l'organisation et l'espace cible de manière interactive</dd>
   <dt>-o <i>ORG_NAME</i> (facultatif)</dt>
   <dd>Nom de l'organisation à cibler.</dd>
   <dt>-s <i>SPACE_NAME</i> (facultatif)</dt>
   <dd>Nom de l'espace à cibler.</dd>
   </dl>
Si aucune de ces options n'est spécifiée, le compte, la région, l'organisation et l'espace en cours s'affichent.

<strong>Exemples</strong> :

Définissez le compte, l'organisation et l'espace en cours :

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

Basculez vers une nouvelle région :

```
bluemix target -r eu-gb
```

Affichez le compte, la région, l'organisation et l'espace en cours :

```
bluemix target
```

### bluemix update
{: #bluemix_update}

Mettez à jour l'interface de ligne de commande vers la version la plus récente.

```
bluemix update
```

<strong>Prérequis</strong> : Aucun

### bluemix account orgs
{: #bluemix_account_orgs}

Répertorier toutes les organisations

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>-r <i>REGION</i> (facultatif)</dt>
   <dd>Spécifie la région pour laquelle afficher les informations de l'organisation. Si vous spécifiez 'all', toutes les
organisations de toutes les régions sont répertoriées.</dd>
   <dt>--guid (facultatif)</dt>
   <dd>Affiche l'identificateur global unique (GUID) des organisations.</dd>
   </dl>

<strong>Exemples</strong> :

Répertorier toutes les organisations dans la région `us-south` en affichant leur identificateur global unique

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

Affiche des informations sur l'organisation spécifiée.

```
bluemix account org ORG_NAME [--guid]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation.</dd>
   <dt>--guid (facultatif)</dt>
   <dd>Affiche l'identificateur global unique (GUID) de l'organisation.</dd>
   </dl>

<strong>Exemples</strong> :

Afficher les informations de l'organisation `IBM` en indiquant son identificateur global unique (GUID)

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

Crée une nouvelle organisation. Cette opération ne peut être effectuée que par un propriétaire de compte.

```
bluemix account org-create ORG_NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation à créer.</dd>
   </dl>

<strong>Exemples</strong> :

Création d'une organisation nommée `IBM`.

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

Répliquez une organisation de la région en cours dans une autre région.

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation existante à répliquer.</dd>
   <dt>REGION_NAME (obligatoire)</dt>
   <dd>Nom de la région hébergeant l'organisation répliquée.</dd>
   </dl>

<strong>Exemples</strong> :

Réplication de l'organisation `mon_org` dans la région `eu-gb`:

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

Attribue un nouveau nom à une organisation. Cette opération ne peut être réalisée que par un responsable de l'organisation.

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>OLD_ORG_NAME (obligatoire)</dt>
   <dd>Ancien nom de l'organisation qui sera renommée.</dd>
   <dt>NEW_ORG_NAME (obligatoire)</dt>
   <dd>Nouveau nom à affecter à l'organisation.</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

Cette commande possède la même fonction et les mêmes options que la commande `cf spaces`.


## bluemix account space
{: #bluemix_account_space}

Cette commande possède la même fonction et les mêmes options que la commande `cf space`.


## bluemix account space-create
{: #bluemix_account_space_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-space`.


## bluemix account space-rename
{: #bluemix_account_space_rename}


Cette commande possède la même fonction et les mêmes options que la commande `cf rename-space`.


## bluemix account space-delete
{: #bluemix_account_space_delete}


Cette commande possède la même fonction et les mêmes options que la commande `cf delete-space`.

## bluemix account org-users
{: #bluemix_account_org_users}

Affiche les utilisateurs dans l'organisation spécifiée, par rôle.

```
bluemix account org-users ORG_NAME [-a]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>ORG_NAME (obligatoire)</dt>
<dd>Nom de l'organisation.</dd>
<dt>-a (facultatif)</dt>
<dd>Recense tous les utilisateurs de l'organisation spécifiés, sans les regrouper par rôle.</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

Ajouter un utilisateur à une organisation (un responsable d'organisation est requis).

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

Retirer un utilisateur d'une organisation (responsable d'organisation ou utilisateur/utilisatrice proprement dit(e))

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>Options de commande</strong> :
<dl>
<dt>--force, -f</dt>
<dd>Force une suppression sans demander de confirmation.</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

Extraire tous les rôles d'organisation de l'utilisateur en cours

```
bluemix account org-roles
```

<strong>Prérequis</strong> : Noeud final, Connexion

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

Affecte un rôle de l'organisation à un utilisateur. Cette opération ne peut être réalisée que par un responsable de l'organisation.

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
  <dl>
   <dt>USER_NAME (obligatoire)</dt>
   <dd>Nom de l'utilisateur à affecter.</dd>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation à laquelle l'utilisateur est affecté.</dd>
   <dt>ORG_ROLE (obligatoire)</dt>
   <dd>Nom du rôle d'organisation auquel cet utilisateur est affecté. Par exemple :
   <ul>
   <li>OrgManager : ce rôle peut inviter et gérer des utilisateurs, sélectionner et changer de plan, et définir des plafonds de dépense.</li>
   <li>BillingManager : ce rôle peut créer et gérer le compte de facturation et les informations de paiement.</li>
   <li>OrgAuditor : ce rôle dispose d'un accès en lecture seule aux informations de l'organisation et aux rapports.</li>
   </ul>
   </dd>
  </dl>

<strong>Exemples</strong> :

Affecter l'utilisatrice `Mary` à l'organisation `IBM` sous le rôle `OrgManager` :

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**Remarque **: vous pouvez définir des rôles d'organisation ou d'espace via l'interface CLI, mais pour les autres autorisations, il vous utiliser l'interface utilisateur. Pour plus d'informations, voir [Octroi d'un accès utilisateur](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

Supprime l'affectation d'un rôle d'organisation à un utilisateur. Cette opération ne peut être réalisée que par un responsable de l'organisation.

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>USER_NAME (obligatoire)</dt>
   <dd>Nom de l'utilisateur à supprimer.</dd>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation dans laquelle supprimer cet utilisateur.</dd>
   <dt>ORG_ROLE (obligatoire)</dt>
   <dd>Nom du rôle d'organisation dans lequel supprimer cet utilisateur. Par exemple :
   <ul>
   <li>OrgManager : ce rôle peut inviter et gérer des utilisateurs, sélectionner et changer de plan, et définir des plafonds de dépense.</li>
   <li>BillingManager : ce rôle peut créer et gérer le compte de facturation et les informations de paiement.</li>
   <li>OrgAuditor : ce rôle dispose d'un accès en lecture seule aux informations de l'organisation et aux rapports.</li>
   </ul>
   </dd>
    </dl>

<strong>Exemples</strong> :

Retirer l'utilisatrice `Mary` de l'organisation `IBM` sous le rôle `OrgManager` :

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

Affichage des utilisateurs, par rôle, dans l'espace spécifié.

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation.</dd>
   <dt>SPACE_NAME (obligatoire)</dt>
   <dd>Nom de l'espace.</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

Affecte un rôle d'espace à un utilisateur. Cette opération ne peut être réalisée que par un gestionnaire d'espace.

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

   <dl>
   <dt>USER_NAME (obligatoire)</dt>
   <dd>Nom de l'utilisateur à affecter.</dd>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation à laquelle l'utilisateur est affecté.</dd>
   <dt>SPACE_NAME (obligatoire)</dt>
   <dd>Nom de l'espace auquel affecter cet utilisateur.</dd>
   <dt>SPACE_ROLE (obligatoire)</dt>
   <dd>Nom du rôle d'espace auquel affecter cet utilisateur. Par exemple :
   <ul>
   <li>SpaceManager: ce rôle peut inviter et gérer des utilisateurs, et activer des fonctions dans un espace spécifique.</li>
   <li>SpaceDeveloper : ce rôle peut créer et gérer des applications et des services, et consulter les journaux et les rapports.</li>
   <li>SpaceAuditor : ce rôle peut consulter les journaux, les rapports, et les paramètres de l'espace.</li>
   </ul></dd>
    </dl>

<strong>Exemples</strong> :

Affecter l'utilisatrice `Mary` à l'organisation `IBM` et à l'espace `Cloud` sous le rôle `SpaceManager` :

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

Suppression de l'affectation d'un rôle d'espace à un utilisateur. Cette opération ne peut être réalisée que par un gestionnaire d'espace.

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

   <dl>
   <dt>USER_NAME (obligatoire)</dt>
   <dd>Nom de l'utilisateur à supprimer.</dd>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation dans laquelle supprimer cet utilisateur.</dd>
   <dt>SPACE_NAME (obligatoire)</dt>
   <dd>Nom de l'espace dans lequel supprimer cet utilisateur.</dd>
   <dt>SPACE_ROLE (obligatoire)</dt>
   <dd>Nom du rôle d'espace dans lequel supprimer cet utilisateur. Par exemple :
   <ul>
   <li>SpaceManager: ce rôle peut inviter et gérer des utilisateurs, et activer des fonctions dans un espace spécifique.</li>
   <li>SpaceDeveloper : ce rôle peut créer et gérer des applications et des services, et consulter les journaux et les rapports.</li>
   <li>SpaceAuditor : ce rôle peut consulter les journaux, les rapports, et les paramètres de l'espace.</li>
   </ul></dd>
    </dl>


<strong>Exemples</strong> :

Retirer l'utilisatrice `Mary` de l'organisation `IBM` et de l'espace `Cloud` sous le rôle `SpaceManager` :

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

Afficher la liste de tous les comptes de l'utilisateur en cours

```
bluemix account list
```

<strong>Prérequis</strong> : Noeud final, Connexion


## bluemix account org-account
{: #bluemix_account_org_account}

Afficher le compte de l'organisation spécifiée (utilisateur d'organisation requis).

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
  <dt>--guid (facultatif)</dt>
  <dd>Affiche uniquement l'ID de compte</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

Affiche les utilisateurs associés au compte. Cette opération ne peut être effectuée que par le propriétaire de compte.

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

Supprimer un utilisateur dans le compte en cours (propriétaire de compte seulement).

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>USERNAME (obligatoire)</dt>
<dd>Nom d'utilisateur</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>ID compte. Si ce paramètre n'est pas spécifié, le compte en cours est pris par défaut.</dd>
<dt>--force, -f (facultatif)</dt>
<dd>Force une suppression sans demander de confirmation.</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

Invite un utilisateur à joindre le compte avec un rôle d'organisation et un rôle d'espace déjà définis. Cette opération ne peut être effectuée que par le propriétaire de compte.

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
   <dt>USER_NAME (obligatoire)</dt>
   <dd>Nom de l'utilisateur à inviter.</dd>
   <dt>ORG_NAME (obligatoire)</dt>
   <dd>Nom de l'organisation dans laquelle cet utilisateur est invité.</dd>
   <dt>ORG_ROLE (obligatoire)</dt>
   <dd>Nom du rôle d'organisation pour lequel cet utilisateur est invité. Par exemple :
   <ul>
  <li>OrgManager : ce rôle peut inviter et gérer des utilisateurs, sélectionner et changer de plan, et définir des plafonds de dépense.</li>
  <li>BillingManager : ce rôle peut créer et gérer le compte de facturation et les informations de paiement.</li>
  <li>OrgAuditor : ce rôle dispose d'un accès en lecture seule aux informations de l'organisation et aux rapports.</li>
  </ul> </dd>
   <dt>SPACE_NAME (obligatoire)</dt>
   <dd>Nom de l'espace pour lequel cet utilisateur est invité.</dd>
   <dt>SPACE_ROLE (obligatoire)</dt>
   <dd>Nom de l'espace pour lequel cet utilisateur est invité. Nom du rôle d'espace pour lequel cet utilisateur est invité. Par exemple :
   <ul>
<li>SpaceManager: ce rôle peut inviter et gérer des utilisateurs, et activer des fonctions dans un espace spécifique.</li>
<li>SpaceDeveloper : ce rôle peut créer et gérer des applications et des services, et consulter les journaux et les rapports.</li>
<li>SpaceAuditor : ce rôle peut consulter les journaux, les rapports, et les paramètres de l'espace.</li>
</ul>
</dd>
</dl>

<strong>Exemples</strong> :

Inviter l'utilisatrice `Mary` dans l'organisation `IBM` sous le rôle `OrgManager` et dans l'espace   `Cloud` sous le rôle `SpaceAuditor` :

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**Remarque **: vous pouvez définir des rôles d'organisation ou d'espace lors de l'invitation par le biais de l'interface CLI, mais pour les autres autorisations, il vous faut utiliser l'interface utilisateur. Pour plus d'informations, voir [Octroi d'un accès utilisateur](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

Renvoyer l'invitation à un utilisateur (gestionnaire d'organisation ou propriétaire de compte requis).

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

Répertorier tous les ID de service

```
bluemix iam service-ids --uuid
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-uuid</dt>
  <dd>Afficher l'identificateur unique universel des ID de service uniquement</dd>
</dl>

<strong>Exemples</strong> :
Répertorier les identificateurs uniques universels de tous les ID de service sous le compte en cours

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

Afficher les détails d'un ID de service

```
bluemix iam service-id NAME [--uuid]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du service</dd>
  <dt>-uuid</dt>
  <dd>Afficher l'identificateur unique universel de l'ID de service</dd>
</dl>

<strong>Exemples</strong> :

Afficher les détails de l'ID de service `sample-test`

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

Créer un ID de service

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du service</dd>
  <dt>-d, --description</dt>
  <dd>Description de l'ID de service</dd>
</dl>

<strong>Exemples</strong> :

Créer un ID de service avec le nom `sample-test` et la description `hello, world!`

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
Mettre à jour un ID de service

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du service</dd>
  <dt>-n, --name</dt>
  <dd>Nouveau nom du service</dd>
  <dt>-d, --description</dt>
  <dd>Nouvelle description du service</dd>
  <dt>-v, --version</dt>
  <dd>Version de l'ID de service</dd>
  <dt>-f, --force</dt>
  <dd>Mettre à jour sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Renommer l'ID de service `sample-test` en `sample-test-2` sans demander de confirmation

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

Mettre à jour la description of service `sample-test` version `1-0jn39fbefew`

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

Supprimer un ID de service

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du service</dd>
  <dt>-f, --force</dt>
  <dd>Supprimer sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Supprimer l'ID de service `sample-teset` sans demander de confirmation

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

Répertorier toutes les clés d'API de la plateforme Bluemix

```
bluemix iam api-keys
```

<strong>Prérequis</strong> : Noeud final, Connexion

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

Créer une nouvelle clé d'API de plateforme Bluemix.

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>NAME (obligatoire)</dt>
<dd>Nom de la clé d'API à créer.</dd>
<dt>-d <i>DESCRIPTION</i> (facultatif)</dt>
<dd>Description de la clé d'API</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>Sauvegarder les informations de clé d'API dans le fichier spécifié. Si cette option n'est pas spécifiée, le contenu JSON s'affiche.</dd>
</dl>

<strong>Exemples</strong> :

Créer une clé d'API et de la sauvegarder dans un fichier

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Mettre à jour une clé d'API de plateforme Bluemix

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>NAME (obligatoire)</dt>
<dd>Ancien nom de la clé d'API qui doit être mise à jour</dd>
<dt>-n <i>NAME</i> (facultatif)</dt>
<dd>Nouveau nom de la clé d'API</dd>
<dt>-d <i>DESCRIPTION</i> (facultatif)</dt>
<dd>Nouvelle description de la clé d'API</dd>
</dl>

<strong>Exemples</strong> :

Mettre à jour la description d'une clé d'API :

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Supprimer une clé d'API de plateforme Bluemix

```
bluemix iam api-key-delete NAME [-f]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>NAME (obligatoire)</dt>
<dd>Nom de la clé d'API à supprimer.</dd>
<dt>-f (facultatif)</dt>
<dd>Force une suppression sans demander de confirmation.</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

Répertorier toutes les clés d'API de service

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
</dl>

<strong>Exemples</strong> :

Afficher les clés d'API de service liées au nom de ressource de cloud de service `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

Répertorier les détails d'une clé d'API de service

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-uuid</dt>
  <dd>Afficher l'identificateur unique universel de la clé d'API de service</dd>
</dl>

<strong>Exemples</strong> :

Afficher les détails de la clé d'API de service `sample-key` liée au nom de ressource de cloud de service`crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

Créer une clé d'API de service

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-d, --description</dt>
  <dd>Description de la clé d'API</dd>
  <dt>-f, --file</dt>
  <dd>Sauvegarder les informations de clé d'API dans le fichier spécifié. Si cette option n'est pas spécifiée, le contenu JSON s'affiche.</dd>
</dl>

<strong>Exemples</strong> :

Créer une clé d'API de service `sample-key` liée au nom de ressource de cloud de service `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

Mettre à jour une clé d'API de service

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-n, --name</dt>
  <dd>Nouveau nom de la clé d'API de service</dd>
  <dt>-d, --description</dt>
  <dd>Nouvelle description de la clé d'API de service</dd>
  <dt>-v, --version</dt>
  <dd>Version de la clé d'API de service</dd>
  <dt>-f, --force</dt>
  <dd>Mettre à jour sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Renommer la clé d'API de service `sample-key` en `new-sample-key` :

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

Supprimer une clé d'API de service

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-f, --force</dt>
  <dd>Supprimer sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Supprimer la clé d'API de service `sample-key` :

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

Afficher les règles de l'utilisateur `name@example.com` :

```
bluemix iam user-policies name@example.com
```

<strong>Prérequis</strong> : Noeud final, Connexion, Compte ciblé

<strong>Options de commande</strong> :
<dl>
<dt>USER_NAME (obligatoire)</dt>
<dd>Nom de l'utilisateur auquel les règles appartiennent</dd>
</dl>

<strong>Exemples</strong> :

Afficher les règles de l'utilisateur `name@example.com` :

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

Afficher les détails d'une règle utilisateur

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>Prérequis</strong> : Noeud final, Connexion, Compte ciblé

<strong>Options de commande</strong> :
<dl>
<dt>USER_NAME (obligatoire)</dt>
<dd>Nom de l'utilisateur auquel la règle appartient</dd>
<dt>POLICY_ID (obligatoire)</dt>
<dd>ID de la règle</dd>
</dl>

<strong>Exemples</strong> :

Afficher la règle `0bb730daa` de l'utilisateur `name@example.com` :

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

Créer une règle utilisateur

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>Prérequis</strong> : Noeud final, Connexion, Compte ciblé

<strong>Options de commande</strong> :
<dl>
<dt>USER_NAME (obligatoire)</dt>
<dd>Nom de l'utilisateur auquel la règle appartient</dd>
<dt>-f, --file <i>FILE</i> (facultatif)</dt>
<dd>Fichier JSON de définition de police</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (facultatif)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (facultatif)</dt>
<dd>Nom de service de la définition de règles. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--service-instance <i>SERVICE_INSTANCE</i> (facultatif)</dt>
<dd>Instance de service de la définition de règles. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--region <i>REGION</i> (facultatif)</dt>
<dd>Région de la définition de règles. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (facultatif)</dt>
<dd>Type de ressource de la définition de règles. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (facultatif)</dt>
<dd>Ressource de la définition de règles. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (facultatif)</dt>
<dd>Nom du groupe de ressources. Exclusif avec les indicateurs '-f, --file', '--resource' et '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (facultatif)</dt>
<dd>ID du groupe de ressources. Exclusif avec les indicateurs '-f, --file', '--resource' et '--resource-group-name'.</dd>
  <dd>Noms de rôle de la définition de règle. Pour les rôles pris en charge d'un service spécifique, exécutez 'bluemix iam roles --service SERVICE_NAME'. Cette option exclut '-f, --file'.</dd>
</dl>

<strong>Exemples</strong> :

Créer une règle utilisateur pour l'utilisateur `name@example.com` à partir du fichier JSON de règles `policy.json` :

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

Accorder le rôle `Administrator` à `name@example.com` pour toutes les ressources `sample-service` :

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

Accorder le rôle `Editor` à `name@example.com` pour la ressource `key123` de l'exemple d'instance de service`ServiceId-ade78e9f` dans la région `us-south` :

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Accorder le rôle `Operator` à `name@example.com` pour le groupe de ressources portant l'ID `dda27e49d2a1efca58083a01dfde18f6` :

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Accorder le rôle `Viewer` à `name@example.com` pour les membres du groupe de ressources `sample-resource-group` :

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

Accorder le rôle `Viewer` à `name@example.com` pour les membres du groupe de ressources portant l'ID `dda27e49d2a1efca58083a01dfde18f6` :

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

Mettre à jour une règle utilisateur

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>Prérequis</strong> : Noeud final, Connexion, Compte ciblé

<strong>Options de commande</strong> :
<dt>USER_NAME (obligatoire)</dt>
<dd>Nom de l'utilisateur auquel la règle appartient</dd>
<dt>POLICY_ID (obligatoire)</dt>
<dd>ID de la règle à mettre à jour</dd>
<dt>-v, --version <i>VERSION</i> (facultatif)</dt>
<dd>Version de règle existante</dd>
<dt>-f, --file <i>FILE</i> (facultatif)</dt>
<dd>Fichier JSON de définition de règle</dd>
<dt>-f, --file <i>FILE</i> (facultatif)</dt>
<dd>Fichier JSON de définition de règle</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (facultatif)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (facultatif)</dt>
<dd>Nom de service de la définition de règle. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--service-instance <i>SERVICE_INSTANCE</i> (facultatif)</dt>
<dd>Instance de service de la définition de règle. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--region <i>REGION</i> (facultatif)</dt>
<dd>Région de la définition de règle. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (facultatif)</dt>
<dd>Type de ressource de la définition de règle. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (facultatif)</dt>
<dd>Ressource de la définition de règle. Exclusif avec l'indicateur '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (facultatif)</dt>
<dd>Nom du groupe de ressources. Exclusif avec les indicateurs '-f, --file', '--resource' et '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (facultatif)</dt>
<dd>ID du groupe de ressources. Exclusif avec les indicateurs '-f, --file', '--resource' et '--resource-group-name'.</dd>
  <dd>Noms de rôle de la définition de règle. Pour les rôles pris en charge d'un service spécifique, exécutez 'bluemix iam roles --service SERVICE_NAME'. Cette option exclut '-f, --file'.</dd>
</dl>

<strong>Exemples</strong> :

Mettre à jour une règle utilisateur avec celle définie dans le fichier JSON

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

Mettre à jour une règle utilisateur afin d'accorder le rôle `Administrator` à `name@example.com` pour toutes les ressources `sample-service` :

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 Mettre à jour une règle utilisateur afin d'accorder le rôle `Editor` à `name@example.com` pour la ressource `key123` de l'exemple d'instance de service `ServiceId-ade78e9f` dans la région `us-south` :

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Mettre à jour une règle utilisateur afin d'accorder le rôle `Operator` à `name@example.com` pour le groupe de ressources portant l'ID `dda27e49d2a1efca58083a01dfde18f6` :

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Mettre à jour une règle utilisateur afin d'accorder le rôle `Viewer` à `name@example.com` pour les membres du groupe de ressources `sample-resource-group` :

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

Mettre à jour une règle utilisateur afin d'accorder le rôle `Viewer` à `name@example.com` pour les membres du groupe de ressources portant l'ID `dda27e49d2a1efca58083a01dfde18f6` :

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

Répertorier toutes les règles de service du service spécifié

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>SERVICE_ID_NAME (obligatoire)</dt>
  <dd>Nom d'ID de service</dd>
  <dt>-json</dt>
  <dd>Afficher la règle au format JSON</dd>
  <dt>-f, --force</dt>
  <dd>Afficher les règles de service sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Répertorier les règles du service `test` :

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

Afficher les détails d'une règle de service

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>SERVICE_ID_NAME (obligatoire)</dt>
  <dd>Nom d'ID de service</dd>
  <dt>POLICY_ID (obligatoire)</dt>
  <dd>ID de la règle de service<dd>
  <dt>-json</dt>
  <dd>Afficher la règle au format JSON</dd>
  <dt>-f, --force</dt>
  <dd>Afficher la règle de service sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Afficher la règle `140798e2-8ea7db3` du service `test` :

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

Créer une règle de service

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>SERVICE_ID_NAME (obligatoire)</dt>
  <dd>Nom d'ID de service</dd>
  <dt>-f, --file</dt>
  <dd>Fichier JSON de définition de règle. Exclut les indicateurs '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' et '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Noms de rôle de la définition de règle. Pour les rôles pris en charge d'un service spécifique, exécutez 'bluemix iam roles --service SERVICE_NAME'. Cette option exclut '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nom de service de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Instance de service de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Région de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Type de ressource de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Ressource de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Créer la règle de service sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Créer une règle de service à partir du fichier JSON pour le service `test` :

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

Mettre à jour une règle de service

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>SERVICE_ID_NAME (obligatoire)</dt>
  <dd>Nom d'ID de service</dd>
  <dt>POLICY_ID (obligatoire)</dt>
  <dd>ID de la règle de service<dd>
  <dt>-v, --version</dt>
  <dd>Version de la règle de service</dd>
  <dt>-f, --file</dt>
  <dd>Fichier JSON de définition de règle. Exclut les indicateurs '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' et '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Noms de rôle de la définition de règle. Pour les rôles pris en charge d'un service spécifique, exécutez 'bluemix iam roles --service SERVICE_NAME'. Cette option exclut '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nom de service de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Instance de service de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Région de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Type de ressource de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Ressource de la définition de règle. Exclut l'indicateur '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Mettre à jour la règle de service sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Mettre à jour la règle de service `140798e2-8ea7db3` à partir du fichier JSON pour le service `test` :

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

Supprimer une règle de service

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>SERVICE_ID_NAME (obligatoire)</dt>
  <dd>Nom d'ID de service</dd>
  <dt>POLICY_ID (obligatoire)</dt>
  <dd>ID de la règle de service<dd>
  <dt>-f, --force</dt>
  <dd>Supprimer sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Supprimer la règle `140798e2-8ea7db3` du service `test`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

Répertorier les groupes de ressources

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>--default</dt>
  <dd>Obtenir le groupe par défaut du compte en cours</dd>
  <dt>-r, --resource</dt>
  <dd>ID de la ressource membre</dd>
  <dt>-o, --resource-origin</dt>
  <dd>Origine de la ressource membre. Valeurs admises : 'CF_ORG', 'IMS_ACCOUNT'.</dd>
</dl>

<strong>Exemples</strong> :

Répertorier tous les groupes de ressources sous le compte actuellement ciblé :

```
bluemix resource groups
```

Répertorier le groupe par défaut du compte actuellement ciblé :

```
bluemix resource groups --default
```

Répertorier les groupes de ressources mappés à une organisation CloudFoundry

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

Afficher les détails d'un groupe de ressources

```
bluemix resource group NAME [--id]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du groupe de ressources</dd>
  <dt>--id</dt>
  <dd>Afficher l'ID uniquement</dd>
</dl>

<strong>Exemples</strong> :

Afficher le groupe de ressources `example-group` :

```
bluemix resource group example-group
```

Afficher uniquement le groupe de ressources `example-group` :

```
bluemix resource group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

Mettre à jour un groupe de ressources existant

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du groupe de ressources cible</dd>
  <dt>-n, --name</dt>
  <dd>Nouveau nom du groupe de ressources</dd>
  <dt>-q, --quota</dt>
  <dd>Nom de la nouvelle définition de quota</dd>
  <dt>-f</dt>
  <dd>Forcer la mise à jour sans confirmation</dd>
</dl>

<strong>Exemples</strong> :

Renommer le groupe de ressources `example-group` en `trial-group` :

```
bluemix resource group-update example-group -n trial-group
```

Modifier le quota du groupe de ressources `example-group` et le remplacer par `free` :

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

Répertorier toutes les définitions de quota

```
bluemix resource quotas
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
</dl>

<strong>Exemples</strong> :

Répertorier toutes les définitions de quota :

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

Afficher les détails d'une définition de quota

```
bluemix resource quota NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom du quota</dd>
</dl>

<strong>Exemples</strong> :
Afficher les détails du quota `free` :

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

Cette commande possède la même fonction et les mêmes options que la commande `cf push`.


## bluemix app list
{: #bluemix_app_list}

Cette commande possède la même fonction et les mêmes options que la commande `cf apps`.


## bluemix app show
{: #bluemix_app_show}

Cette commande possède la même fonction et les mêmes options que la commande `cf app`.


## bluemix app delete
{: #bluemix_app_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete`.


## bluemix app rename
{: #bluemix_app_rename}

Cette commande possède la même fonction et les mêmes options que la commande `cf rename`.


## bluemix app start
{: #bluemix_app_start}

Cette commande possède la même fonction et les mêmes options que la commande `cf start`.


## bluemix app stop
{: #bluemix_app_stop}

Cette commande possède la même fonction et les mêmes options que la commande `cf stop`.


## bluemix app restart
{: #bluemix_app_restart}

Cette commande possède la même fonction et les mêmes options que la commande `cf restart`.


## bluemix app restage
{: #bluemix_app_restage}


Cette commande possède la même fonction et les mêmes options que la commande `cf restage`.


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


Cette commande possède la même fonction et les mêmes options que la commande `cf restart-app-instance`.


## bluemix app events
{: #bluemix_app_events}

Cette commande possède la même fonction et les mêmes options que la commande `cf events`.


## bluemix app files
{: #bluemix_app_files}

Cette commande possède la même fonction et les mêmes options que la commande `cf files`.


## bluemix app logs
{: #bluemix_app_logs}

Cette commande possède la même fonction et les mêmes options que la commande `cf logs`.


## bluemix app env
{: #bluemix_app_env}

Cette commande possède la même fonction et les mêmes options que la commande `cf env`.


## bluemix app env-set
{: #bluemix_app_env_set}

Cette commande possède la même fonction et les mêmes options que la commande `cf set-env`.


## bluemix app env-unset
{: #bluemix_app_env_unset}

Cette commande possède la même fonction et les mêmes options que la commande `cf unset-env`.


## bluemix app stacks
{: #bluemix_app_stacks}

Cette commande possède la même fonction et les mêmes options que la commande `cf stacks`.


## bluemix app stack-show
{: #bluemix_app_stack_show}

Cette commande possède la même fonction et les mêmes options que la commande `cf stack`.


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-app-manifest`.

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

Affichez les informations de certificat d'un domaine.

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
<dl>
<dt>DOMAIN_NAME (obligatoire)</dt>
<dd>Domaine hébergeant le certificat.</dd>
</dl>


<strong>Exemples</strong> :

Affichage des informations de certificat du domaine `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

Ajoutez un certificat au domaine indiqué dans l'organisation en cours.

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
   <dl>
   <dt>DOMAIN (obligatoire)</dt>
   <dd>Domaine auquel ajouter le certificat.</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i> (obligatoire)</dt>
   <dd>Chemin du fichier de clé privée.</dd>
   <dt>-c <i>CERT_FILE</i> (obligatoire)</dt>
   <dd>Chemin du fichier de certificat.</dd>
   <dt>-p <i>PASSWORD</i> (facultatif)</dt>
   <dd>Mot de passe du certificat.</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i> (facultatif)</dt>
   <dd>Chemin du fichier de certificat intermédiaire.</dd>
   <dt>-t <i>TRUST_STORE_FILE</i> (facultatif)</dt>
   <dd>Fichier de clés certifiées.</dd>
   </dl>


<strong>Exemples</strong> :

Ajoutez un certificat au domaine `ibmcxo-eventconnect.com` :

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

Supprimez un certificat du domaine spécifié dans l'organisation en cours.

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :

   <dl>
   <dt>DOMAIN (obligatoire)</dt>
   <dd>Domaine duquel supprimer le certificat.</dd>
   <dt>-f (facultatif)</dt>
   <dd>Force une suppression sans demander de confirmation.</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

Cette commande possède la même fonction et les mêmes options que la commande `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-shared-domain`.

## bluemix app routes
{: #bluemix_app_routes}

Cette commande possède la même fonction et les mêmes options que la commande `cf routes`.


## bluemix app route-check
{: #bluemix_app_route_check}

Cette commande possède la même fonction et les mêmes options que la commande `cf check-route`.


## bluemix app route-map
{: #bluemix_app_route_map}

Mappez une route à une application cf ou un groupe de conteneurs existant associé au domaine et au nom d'hôte spécifiés.

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (obligatoire)</dt>
   <dd>Nom de l'application cf ou du groupe de conteneur à mapper à une route.</dd>
   <dt>DOMAIN (obligatoire)</dt>
   <dd>Domaine de la route. Par exemple, mychinabluemix.net ou chinabluemix.net. </dd>
   <dt>-n <i>HOST_NAME</i> (facultatif)</dt>
   <dd>Nom d'hôte de la route. S'il n'est pas spécifié, le nom d'hôte est le nom de l'application ou le nom du groupe de conteneurs par défaut.</dd>
   </dl>

<strong>Exemples</strong> :

Mappez une route à `mon-app` avec le domaine spécifié :

```
bluemix app route-map my-app mychinabluemix.net
```

Mappez une route à 'mon-groupe-conteneurs' avec le domaine et le nom d'hôte spécifiés :

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

Supprimez le mappage de la route spécifiée à une application cf ou un groupe de conteneurs existant.

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (obligatoire)</dt>
   <dd>Nom de l'application cf ou du groupe de conteneurs.</dd>
   <dt>DOMAIN (obligatoire)</dt>
   <dd>Domaine de la route (par exemple, mychinabluemix.net ou chinabluemix.net).</dd>
   <dt>-n <i>HOST_NAME</i> (facultatif)</dt>
   <dd>Nom d'hôte de la route. S'il n'est pas spécifié, le nom d'hôte est le nom de l'application ou le nom du groupe de conteneurs par défaut.</dd>
   </dl>

<strong>Exemples</strong> :

Supprimez le mappage de la route `mon-app.mychinabluemix.net` de `mon-app` :

```
bluemix app route-unmap my-app mychianbluemix.net
```

Supprimez le mappage de la route `abc.chinabluexmix.net` de `mon-groupe-conteneurs` :

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-route`.


## bluemix app route-delete
{: #bluemix_app_route_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-route`.


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-orphaned-routes`.


## bluemix app domains
{: #bluemix_app_domains}

Cette commande possède la même fonction et les mêmes options que la commande `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-shared-domain`.


## bluemix service offerings
{: #bluemix_service_offerings}


Cette commande possède la même fonction et les mêmes options que la commande `cf marketplace`.


## bluemix service list
{: #bluemix_service_list}

Cette commande possède la même fonction et les mêmes options que la commande `cf services`.


## bluemix service show
{: #bluemix_service_show}

Cette commande possède la même fonction et les mêmes options que la commande `cf service`.


## bluemix service create
{: #bluemix_service_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-service`.


## bluemix service update
{: #bluemix_service_update}

Cette commande possède la même fonction et les mêmes options que la commande `cf update-service`.


## bluemix service delete
{: #bluemix_service_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-service`.


## bluemix service rename
{: #bluemix_service_rename}

Cette commande possède la même fonction et les mêmes options que la commande `cf rename-service`.


## bluemix service bind
{: #bluemix_service_bind}

Cette commande possède la même fonction et les mêmes options que la commande `cf bind-service`.


## bluemix service unbind
{: #bluemix_service_unbind}

Cette commande possède la même fonction et les mêmes options que la commande `cf unbind-service`.


## bluemix service key-create
{: #bluemix_service_key_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-service-key`.


## bluemix service key-delete
{: #bluemix_service_key_delete}

Cette commande possède la même fonction et les mêmes options que la commande `cf delete-service-key`.


## bluemix service keys
{: #bluemix_service_keys}

Cette commande possède la même fonction et les mêmes options que la commande `cf service-keys`.


## bluemix service key-show
{: #bluemix_service_key_show}

Cette commande possède la même fonction et les mêmes options que la commande `cf service-key`.


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

Cette commande possède la même fonction et les mêmes options que la commande `cf create-user-provided-service`.


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

Cette commande possède la même fonction et les mêmes options que la commande `cf update-user-provided-service`.


## bluemix resource instances
{: #bluemix_resource_instances}

Répertorier les instances de ressource

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>--resource-name</dt>
  <dd>Nom de la ressource membre</dd>
  <dt>-r, --region</dt>
  <dd>Filtre par ID de région, par défaut la région en cours si rien n'est spécifié, '-r, --region all' pour afficher les instances de ressource de toutes les régions</dd>
  <dt>--long</dt>
  <dd>Afficher des zones supplémentaires dans la sortie</dd>
</dl>

<strong>Exemples</strong> :

Répertorier les instances de la ressource `test-resource` :

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

Afficher les détails d'une instance de ressource

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom de l'instance de ressource</dd>
  <dt>-r, --region</dt>
  <dd>Filtre par ID de région, par défaut la région en cours si rien n'est spécifié, '-r, --region all' pour afficher les instances de ressource de toutes les régions</dd>
  <dt>--id</dt>
  <dd>Afficher l'ID de l'instance de ressource</dd>
</dl>

<strong>Exemples</strong> :
Afficher les détails de l'instance de ressource `my-resource-instance` :

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

Créer une instance de ressource

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME (obligatoire)</dt>
  <dd>Nom de l'instance de ressource</dd>
  <dt>RESOURCE_NAME ou RESOURCE_ID (obligatoire)</dt>
  <dd>Nom ou ID de la ressource</dd>
  <dt>RESOURCE_PLAN_NAME ou RESOURCE_PLAN_ID (obligatoire)</dt>
  <dd>Nom ou ID du plan de ressources</dd>
  <dt>-r, --region</dt>
  <dd>Région dans laquelle créer l'instance de ressource, il s'agit par défaut de la région en cours si rien n'est spécifié</dd>
  <dt>-t, --tags</dt>
  <dd>Etiquettes</dd>
  <dt>-p, --parameters</dt>
  <dd>Fichier JSON ou chaîne de paramètres JSON pour la création de l'instance de ressource</dd>
</dl>

<strong>Exemples</strong> :
Créer une instance de ressource nommée `my-resource-instance` en utilisant le plan de ressources `test-resource-plan` de la ressource `test-resource` :

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

Mettre à jour une instance de ressource

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>RESOURCE_INSTANCE_NAME (obligatoire)</dt>
  <dd>Nom de l'instance de ressource</dd>
  <dt>-n, --name</dt>
  <dd>Nouveau nom de l'instance de ressource</dd>
  <dt>-t, --tags</dt>
  <dd>Nouvelles étiquettes</dd>
  <dt>--resource-plan-id</dt>
  <dd>Nouvel ID du plan de ressources</dd>
  <dt>--update-time</dt>
  <dd>Durée en secondes depuis l'époque de la prise d'effet attendue de l'enregistrement payant</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la mise à jour sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Mettre à jour l'instance de ressource `my-resource-instance` et remplacer son nom par `new-resource-instance` :

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

Supprimer une instance de ressource

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-f, --force</dt>
  <dd>Forcer la suppression sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Supprimer l'instance de ressource `my-resource-instance` :

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

Afficher les liaisons vers l'alias de ressource

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>RESOURCE_ALIAS (obligatoire)</dt>
  <dd>Nom d'alias de ressource</dd>
</dl>

<strong>Exemples</strong> :
Afficher les liaisons de ressources à l'alias de ressource `my-resource-alias` :

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

Afficher les détails d'une liaison de ressource

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>ALIAS_NAME (obligatoire)</dt>
  <dd>Nom d'alias de ressource</dd>
  <dt>APP_NAME</dt>
  <dd>Nom d'application CloudFoundry</dd>
  <dt>--id</dt>
  <dd>Seul l'ID s'affiche. Toute autre sortie de la liaison de ressource est supprimée.</dd>
</dl>

<strong>Exemples</strong> :
Afficher les détails de liaison de ressource entre l'alias de ressource `my-resource-alias` et l'application `my-app` :

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

Créer une liaison de ressource

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>RESOURCE_ALIAS_NAME (obligatoire)</dt>
  <dd>Nom d'alias de ressource</dd>
  <dt>APP_NAME</dt>
  <dd>Nom d'application CloudFoundry</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nom du rôle utilisateur</dd>
  <dt>--service-id-name</dt>
  <dd>Nom de l'ID de service auquel le rôle appartient</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la création sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Créer une liaison de ressource entre l'alias de ressource `my-resource-alias` et l'application `my-app` avec le rôle`Administrator` :

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

Supprimer une liaison de ressource

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
<dl>
  <dt>RESOURCE_ALIAS_NAME (obligatoire)</dt>
  <dd>Nom d'alias de ressource</dd>
  <dt>APP_NAME</dt>
  <dd>Nom d'application CloudFoundry</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la suppression sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Supprimer la liaison de ressource entre l'alias de ressource `my-resource-alias` et l'application `my-app` :

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

Répertorier les clés de ressource de l'instance de ressource ou de l'alias de ressource

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>--instance-id</dt>
  <dd>ID d'instance de ressource</dd>
  <dt>--instance-name</dt>
  <dd>Nom d'instance de ressource</dd>
  <dt>--alias-id</dt>
  <dd>ID d'alias de la ressource</dd>
  <dt>--alias-name</dt>
  <dd>Nom d'alias de la ressource</dd>
</dl>

<strong>Exemples</strong> :
Répertorier les clés de ressource de l'instance de ressource `my-resource-instance` :

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

Afficher les détails d'une clé de ressource

```
bluemix resource key KEY_NAME [--id]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nom de la clé</dd>
  <dt>--id</dt>
  <dd>Afficher l'ID de la clé de ressource</dd>
</dl>

<strong>Exemples</strong> :
Afficher les détails de la clé de ressource `my-resource-key` :

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

Créer une clé de ressource

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>NAME</dt>
  <dd>Nom de la clé</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nom du rôle utilisateur</dd>
  <dt>--instance-id</dt>
  <dd>ID d'instance de ressource</dd>
  <dt>--instance-name</dt>
  <dd>Nom d'instance de ressource</dd>
  <dt>--alias-id</dt>
  <dd>ID d'alias de la ressource</dd>
  <dt>--alias-name</dt>
  <dd>Nom d'alias de la ressource</dd>
  <dt>-service-id-name</dt>
  <dd>Nom de l'ID de service auquel le rôle appartient</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la création sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Créer une clé de ressource nommée `my-resource-key` avec le rôle `Administrator` pour l'instance de ressource`my-resource-instance` :

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

Supprimer une clé de ressource

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nom de la clé</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la suppression sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Supprimer la clé de ressource `my-resource-key` :

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

Répertorier les alias d'une instance de ressource

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>--instance-id</dt>
  <dd>ID de l'instance de ressource membre</dd>
  <dt>--instance-name</dt>
  <dd>Nom de l'instance de ressource membre.</dd>
</dl>

<strong>Exemples</strong> :
Répertorier les alias de ressource pour l'instance de ressource `my-resource-instance` :
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

Afficher les détails d'un alias de ressource

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>ALIAS_NAME (obligatoire)</dt>
  <dd>Nom de l'alias de ressource</dd>
  <dt>--id</dt>
  <dd>Seul l'ID de l'alias de la ressource donnée s'affiche. Toute autre sortie de l'alias est supprimée.</dd>
</dl>

<strong>Exemples</strong> :
Afficher les détails de l'alias de ressource `my-resource-alias` :
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

Créer un alias d'une instance de ressource

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>ALIAS_NAME (obligatoire)</dt>
  <dd>Nom de l'alias de ressource</dd>
  <dt>--instance-id</dt>
  <dd>ID de l'instance de ressource membre</dd>
  <dt>--instance-name</dt>
  <dd>Nom de l'instance de ressource membre.</dd>
  <dt>-s</dt>
  <dd>Nom de l'espace dans lequel l'alias est créé. Il s'agit de l'espace en cours par défaut.</dd>
  <dt>-t, --tags</dt>
  <dd>Liste d'étiquettes.</dd>
  <dt>-p, --parameters</dt>
  <dd>Fichier JSON ou chaîne JSON de paramètres.</dd>
</dl>

<strong>Exemples</strong> :
Créer un alias de ressource nommé `my-resource-alias` de l'instance de ressource `my-resource-instance` :
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

Mettre à jour un alias de ressource

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>ALIAS_NAME (obligatoire)</dt>
  <dd>Nom de l'alias de ressource</dd>
  <dt>-n, --name</dt>
  <dd>Nouveau nom de l'alias de ressource.</dd>
  <dt>-t, --tags</dt>
  <dd>Liste d'étiquettes.</dd>
  <dt>-p, --parameters</dt>
  <dd>Fichier JSON ou chaîne JSON de paramètres.</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la mise à jour sans confirmation de l'utilisateur</dd>
</dl>

<strong>Exemples</strong> :
Mettre à jour un alias de ressource `my-resource-alias` et remplacer son nom par `new-resource-alias` :

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

Supprimer un alias de ressource

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>ALIAS_NAME (obligatoire)</dt>
  <dd>Nom de l'alias de ressource</dd>
  <dt>-f, --force</dt>
  <dd>Forcer la suppression sans confirmation</dd>
</dl>

<strong>Exemples</strong> :
Supprimer l'alias de ressource `my-resource-alias` :

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

Effectuer des recherches dans des entrées de catalogue

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-q, --query</dt>
  <dd>Rechercher le mot clé</dd>
  <dt>-r, --region</dt>
  <dd>Spécifier la région géographique dans laquelle effectuer la recherche. Actuellement, seules les régions "us-south" et "united-kingdom" sont prises en charge.</dd>
  <dt>-k, --kind</dt>
  <dd>Filtrer par type de ressource. Actuellement, seules les options "service-cf", "iaas", "runtime", "template" et "dashboard" sont prises en charge.</dd>
  <dt>-p, --price</dt>
  <dd>Filtrer par prix. Actuellement, seuls les options "free", "paygo", "bluemix-subscription" sont prises en charge.</dd>
  <dt>-t, --tag</dt>
  <dd>Filtrer par étiquette.</dd>
  <dt>-sort-by</dt>
  <dd>Propriétés de tri</dd>
  <dt>-reverse</dt>
  <dd>Inverser l'ordre de tri</dd>
  <dt>-json</dt>
  <dd>Imprimer la réponse JSON d'origine</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Effectuer une recherche dans le service `Automation test` :

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

Obtenir une entrée de catalogue

```
bluemix catalog entry [-i ID] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-i, --id</dt>
  <dd>ID de l'entrée de catalogue</dd>
  <dt>-children</dt>
  <dd>Obtenir tous les enfants de l'entrée de catalogue</dd>
  <dt>-json</dt>
  <dd>Imprimer la réponse JSON d'origine</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Obtenir l'entrée portant l'ID `a0ef1-d3b4j0` :

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
Créer une nouvelle entrée de catalogue (administrateur de catalogue d'un compte uniquement)

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-p, --parent</dt>
  <dd>ID parent de l'objet</dd>
  <dt>-c</dt>
  <dd>Objet JSON valide contenant des paramètres de configuration spécifiques au catalogue, fournis en ligne ou dans un fichier. Pour obtenir la liste des paramètres de configuration pris en charge, voir la documentation de l'entrée de catalogue concernée.</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Créer une ressource à partir du fichier JSON portant l'ID parent `a0ef1-d3b4j0` :

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
Mettre à jour une entrée de catalogue existante (administrateur ou éditeur de catalogue d'un compte uniquement)

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-i, --id</dt>
  <dd>ID de l'entrée de catalogue qui fait l'objet d'une mise à jour.</dd>
  <dt>-c</dt>
  <dd>Objet JSON valide contenant des paramètres de configuration spécifiques au catalogue, fournis en ligne ou dans un fichier. Pour obtenir la liste des paramètres de configuration pris en charge, voir la documentation de l'entrée de catalogue concernée.</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Mettre à jour la ressource `j402-dnf1i` à partir d'un fichier JSON :

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
Obtenir la visibilité pour une entrée de catalogue (administrateur de catalogue d'un compte uniquement)

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-i, --id</dt>
  <dd>ID de l'entrée de catalogue</dd>
  <dt>-json</dt>
  <dd>Imprimer la réponse JSON d'origine</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Obtenir la visibilité de la ressource `j402-dnf1i` dans une portée globale :

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
Mettre à jour la visibilité d'une entrée de catalogue existante (administrateur de catalogue d'un compte uniquement)

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-i, --id</dt>
  <dd>ID de l'entrée de catalogue qui fait l'objet d'une mise à jour.</dd>
  <dt>-c</dt>
  <dd>Objet JSON valide contenant des paramètres de configuration spécifiques au catalogue, fournis en ligne ou dans un fichier. Pour obtenir la liste des paramètres de configuration pris en charge, voir la documentation de l'entrée de catalogue concernée.</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Définir la visibilité de la ressource `j402-dnf1i` à partir d'un fichier JSON :

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
Répertorier les offres de services de la place du marché

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
<dl>
  <dt>-cf</dt>
  <dd>Afficher les services Cloud Foundry uniquement</dd>
  <dt>-rc</dt>
  <dd>Afficher les services RC compatibles uniquement</dd>
  <dt>-global</dt>
  <dd>Exploiter dans une portée globale</dd>
</dl>

<strong>Exemples</strong> :

Afficher les offres de services dans une portée globale :

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

Affichez les modèles de conteneur boilerplate dans Bluemix.

```
bluemix catalog templates [-d]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

   <dl>
   <dt>-d (facultatif)</dt>
   <dd>Si l'option <i>-d</i> est spécifiée, la description de chaque modèle est également affichée. Sinon, seul l'ID et le nom des modèles sont affichés.</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

Affichez les informations détaillées d'un modèle de conteneur boilerplate spécifié.

```
bluemix catalog template TEMPLATE_ID
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :
   <dl>
   <dt>TEMPLATE_ID (obligatoire)</dt>
   <dd>ID du modèle de conteneur boilerplate. Utilisez <i>bluemix templates</i> pour afficher tous les ID de modèles.</dd>
   </dl>


<strong>Exemples</strong> :

Affichez les détails du modèle `mobileBackendStarter` :

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

Créez une application cf reposant sur le modèle spécifié avec l'adresse URL et la description indiquées. Par défaut, la nouvelle application est démarrée automatiquement.

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>Prérequis</strong> : Noeud final, Connexion, Cible

<strong>Options de commande</strong> :
   <dl>
   <dt>TEMPLATE_ID (obligatoire)</dt>
   <dd>Modèle sur lequel sera basée l'application lors de sa création. Utilisez <i>bluemix templates</i> pour voir tous les ID des modèles.</dd>
   <dt>CF_APP_NAME (obligatoire)</dt>
   <dd>Nom de l'application cf à créer.</dd>
   <dt>-u <i>URL</i> (facultatif)</dt>
   <dd>Route de l'application. Si elle n'est pas spécifiée, la route est définie automatiquement par Bluemix d'après le nom de votre application et le domaine par défaut.</dd>
   <dt>-d <i>DESCRIPTION</i> (facultatif)</dt>
   <dd>Description de l'application.</dd>
   <dt>--no-start (facultatif)</dt>
   <dd>Indique de ne pas démarrer automatiquement l'application après sa création. Si cette option n'est pas spécifiée, l'application est démarrée automatiquement après sa création.</dd>
   </dl>


<strong>Exemples</strong> :

Créez l'application cf `mon-app` d'après le modèle `javaHelloWorld` :

```
bluemix catalog template-run javaHelloWorld mon-app
```

Créez une application `my-ruby-app` d'après le modèle `rubyHelloWorld` avec la route
`myrubyapp.chinabluemix.net` et la description `Ma première application Ruby dans {{site.data.keyword.Bluemix_notm}}.`:

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "Ma première application Ruby dans {{site.data.keyword.Bluemix_notm}}."
```

Créez l'application `mon-app-python` d'après le modèle `pythonHelloWorld` sans démarrage automatique :

```
bluemix catalog template-run pythonHelloWorld mon-app-python --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

Affichez l'utilisation mensuelle et les coûts liés à votre compte.

```
bluemix billing account-usage [-d YYYY-MM] [--json]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

<dl>
  <dt>-d MONTH_DATE (facultatif)</dt>
  <dd>Afficher les données relatives au mois et à la date spécifiées en utilisant le format AAAA-MM. Si ces données ne sont pas spécifiées, l'utilisation du mois en cours est affichée.</dd>
  <dt>--json (facultatif)</dt>
  <dd>Afficher le résultat de l'utilisation au format JSON.</dd>
</dl>

<strong>Exemples</strong> :

Affichage du rapport d'utilisation et des coûts de mon compte pour 2016-06 :

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

Affichez les détails de l'utilisation mensuelle d'une organisation. Cette opération ne peut être réalisée que par un responsable de la facturation de l'organisation.

```
bluemix billing org-usage ORG_NAME [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

<dl>
  <dt>ORG_NAME (obligatoire)</dt>
  <dd>Nom de l'organisation.</dd>
  <dt>-d MONTH_DATE (facultatif)</dt>
  <dd>Afficher les données relatives au mois et à la date spécifiés en utilisant le format AAAA-MM. Si ces données ne sont pas spécifiées, l'utilisation du mois en cours est affichée.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nom de la région qui héberge l'organisation. Si ce paramètre a pour valeur 'all', l'utilisation de l'organisation dans toutes les régions est affichée.</dd>
  <dt>--json (facultatif)</dt>
  <dd>Afficher le résultat de l'utilisation au format JSON.</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

Affichez un récapitulatif d'utilisation mensuelle pour les organisations dans mon compte.

```
bluemix billing orgs-usage-summary [-d YYYY-MM] [-r REGION_NAME] [--json]
```

<strong>Prérequis</strong> : Noeud final, Connexion

<strong>Options de commande</strong> :

<dl>
  <dt>-d MONTH_DATE (facultatif)</dt>
  <dd>Afficher les données relatives au mois et à la date spécifiés en utilisant le format AAAA-MM. Si ces données ne sont pas spécifiées, l'utilisation du mois en cours est affichée.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nom de la région qui héberge les organisations. Si ce paramètre a pour valeur 'all', le récapitulatif d'utilisation des organisations dans toutes les régions est affiché.</dd>
  <dt>--json (facultatif)</dt>
  <dd>Afficher le résultat de l'utilisation au format JSON.</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

Répertoriez tous les référentiels de plug-in qui sont enregistrés dans l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repos
```

<strong>Prérequis</strong> : Aucun


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

Ajoutez un nouveau référentiel de plug-in à l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>REPO_NAME (obligatoire)</dt>
   <dd>Nom du référentiel à ajouter. Vous pouvez définir votre propre nom pour chaque référentiel.</dd>
   <dt>REPO_URL (obligatoire)</dt>
   <dd>URL du référentiel à ajouter. Elle doit contenir le protocole (par exemple http://plugins.ng.bluemix.net au lieu de plugins.ng.bluemix.net). http://plugins.ng.bluemix.net est le référentiel de plug-in officiel de l'interface de ligne de commande (CLI) Bluemix.</dd>
    </dl>


<strong>Exemples</strong> :

Ajoutez le référentiel de plug-in officiel de l'interface de ligne de commande Bluemix sous la forme `référentiel-bluemix` :

```
bluemix plugin repo-add référentiel-bluemix http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

Retirez un référentiel de plug-in de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-remove REPO_NAME
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
   <dl>
   <dt>REPO_NAME (obligatoire)</dt>
   <dd>Nom du référentiel à supprimer.</dd>
   </dl>

<strong>Exemples</strong> :

Supprimez `référentiel-bluemix` de l'interface de ligne de commande (CLI) {{site.data.keyword.Bluemix_notm}} :

```
bluemix plugin repo-remove référentiel-bluemix
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

Répertoriez tous les plug-in disponibles dans tous les référentiels ajoutés ou dans un référentiel spécifique.

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>-r <i>REPO_NAME</i> (facultatif)</dt>
   <dd>Recense uniquement les plug-in dans le référentiel spécifié.</dd>
   </dl>

<strong>Exemples</strong> :

Répertoriez tous les plug-in dans tous les référentiels ajoutés :

```
bluemix plugin repo-plugins
```

Répertoriez tous les plug-in du référentiel `référentiel-bluemix` :

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

Afficher les détails d'un plug-in dans le référentiel

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>-r <i>REPO_NAME</i> (facultatif)</dt>
   <dd>Nom du référentiel. Si aucun référentiel n'est spécifié, la commande utilise le référentiel de plug-in par défaut.</dd>
   </dl>

<strong>Exemples</strong> :

Afficher les détails du plug-in "IBM-Containers" dans le référentiel "sample-repo" :

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

Afficher les détails du plug-in "IBM-Containers" dans le référentiel par défaut

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

Répertoriez tous les plug-in installés dans l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin list
```

<strong>Prérequis</strong> : Aucun

## bluemix plugin show
{: #bluemix_plugin_show}

Afficher les détails d'un plug-in installé

```
bluemix plugin show PLUGIN-NAME
```

<strong>Prérequis</strong> : Aucun


## bluemix plugin install
{: #bluemix_plugin_install}

Installez la version de plug-in spécifique dans l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}} à partir du chemin ou du référentiel spécifié.

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME (obligatoire)</dt>
   <dd>Si -r <i>REPO_NAME</i> n'est pas spécifié, le plug-in est installé depuis le chemin local spécifié ou depuis l'URL distante.</dd>
   <dt>-r <i>REPO_NAME</i> (facultatif)</dt>
   <dd>Nom du référentiel hébergeant le fichier binaire du plug-in. Si aucun référentiel n'est spécifié, la commande utilise le référentiel de plug-in par défaut.</dd>
   <dt>-v <i>VERSION</i> (facultatif)</dt>
   <dd>Version du plug-in à installer. Si elle n'est pas fournie, la dernière version du plug-in est installée. Cette option n'est valide que si vous installez le plug-in à partir du référentiel.</dd>
    </dl>

<strong>Exemples</strong> :

Installez un plug-in depuis le fichier local :

```
bluemix plugin install /downloads/new_plugin
```

Installez un plug-in depuis l'adresse URL distante :

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

Installez la dernière version du plug-in `IBM-Containers` à partir du référentiel `référentiel-bluemix` :

```
bluemix plugin install IBM-Containers -r référentiel-bluemix
```
Installez le plug-in `IBM-Containers` avec la version `0.5.800` à partir du référentiel `référentiel-bluemix` :

```
bluemix plugin install IBM-Containers -r référentiel-bluemix -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

Mettez à niveau le plug-in à partir d'un référentiel

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>Nom du plug-in à mettre à jour. Si ce paramètre n'est pas spécifié, la commande recherche des mises à niveau pour tous les plug-ins installés.</dd>
 <dt>-r REPO_NAME</dt>
 <dd>Nom du référentiel hébergeant le fichier binaire du plug-in. Si ce paramètre n'est pas spécifié, la commande utilise le référentiel de plug-in par défaut.</dd>
 <dt>-v <i>VERSION</i> (facultatif)</dt>
 <dd>Version cible du plug-in pour la mise à jour. Si cette option n'est pas spécifiée, mettez à jour le plugin vers la dernière version disponible.</dd>
 <dt>--all</dt>
 <dd>Mettre à jour tous les plug-in disponibles</dd>
</dl>

<strong>Exemples</strong> :

Recherchez tous les plug-ins disponibles pour la mise à niveau dans le référentiel "My-Repo" :

```
bluemix plugin update -r My-Repo
```

Mettez à niveau le plug-in "plugin-echo" dans le référentiel "My-Repo" vers la dernière version :

```
bluemix plugin update -r My-Repo plugin-echo
```

Mettez à niveau le plug-in "plugin-echo" dans le référentiel "My-Repo" vers la version "1.0.1" :

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

Désinstallez le plug-in spécifié de l'interface de ligne de commande {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>Prérequis</strong> : Aucun

<strong>Options de commande</strong> :

   <dl>
   <dt>PLUGIN_NAME (obligatoire)</dt>
   <dd>Nom du plug-in à désinstaller.</dd>
    </dl>

<strong>Exemples</strong> :

Désinstallez le plug-in `IBM-Containers` installé précédemment :

```
bluemix plugin uninstall IBM-Containers
```

