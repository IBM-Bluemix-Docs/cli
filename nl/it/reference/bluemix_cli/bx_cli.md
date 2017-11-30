---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Comandi {{site.data.keyword.Bluemix_notm}} (bx)
{: #bluemix_cli}

Versione: 0.6.1

L'interfaccia di riga comando (CLI) {{site.data.keyword.Bluemix_notm}} fornisce una serie di comandi che vengono raggruppati in base allo spazio dei nomi per consentire agli utenti di interagire con {{site.data.keyword.Bluemix_notm}}. 

A partire dalla versione 0.5.0, il client riga di comando {{site.data.keyword.Bluemix_notm}} include un client riga di comando Cloud Foundry nella sua installazione. Se hai una tua CLI cf installata, non utilizzare sia i comandi della CLI {{site.data.keyword.Bluemix_notm}} `bx [comando]` che i comandi della CLI Cloud Foundry `cf [comando]`
della tua installazione nello stesso contesto. Utilizza invece `bluemix cf [comando]` se vuoi utilizzare la CLI cf per gestire le risorse Cloud Foundry nel contesto della CLI {{site.data.keyword.Bluemix_notm}}.  Inoltre, `bluemix cf api/login/logout/target` non è consentito e devi utilizzare invece `bluemix api/login/logout/target`.

Viene qui di seguito elencato in modo dettagliato l'utilizzo dei comandi supportati dalla CLI {{site.data.keyword.Bluemix_notm}}, compresi i loro nomi, argomenti, opzioni, prerequisiti, descrizioni ed esempi.
{:shortdesc}

**Nota:** i *Prerequisiti* elencano quali azioni sono richieste prima di utilizzare il comando. I comandi che non hanno azioni prerequisite elencano **Nessuno**. Altrimenti, i prerequisiti possono includere una o più delle seguenti azioni:

<dl>
<dt>Endpoint</dt>
<dd>Un endpoint API deve essere impostato mediante <code>bluemix api</code> prima di utilizzare il comando.</dd>
<dt>Accesso</dt>
<dd>L'accesso utilizzando il comando <code>bluemix login</code> è richiesto prima di utilizzare questo comando.
Se stai eseguendo l'accesso con l'ID federato, utilizza l'opzione '--sso' per autenticarti con il passcode monouso o utilizza '--apikey' per autenticarti con la chiave API. Vai alla console {{site.data.keyword.Bluemix_notm}} **Gestisci** &gt; **Sicurezza** &gt; **Chiavi API Bluemix** per creare le chiavi API.
</dd>
<dt>Destinazione</dt>
<dd>Il comando <code>bluemix target</code> deve essere utilizzato per impostare un'organizzazione e uno spazio prima di utilizzare questo comando.</dd>
<dt>Docker</dt>
<dd>Per poter eseguire questo comando, è necessario che la CLI Docker (docker) sia installata.</dd>
</dl>

**Nota:** puoi utilizzare il formato breve dei comandi bluemix; ad esempio `bx api` è l'abbreviazione di `bluemix api`.

Utilizza gli indici delle seguenti tabelle per fare riferimento ai comandi bluemix più utilizzati.

## Comandi bluemix generali 
{: #bx_commands_index}

<table summary="Comandi bluemix generali.">
<caption>Tabella 1. Comandi bluemix generali</caption>
 <thead>
 <th colspan="5">Comandi bluemix generali</th>
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
 
 ## Comandi per la gestione e configurazione dei servizi {{site.data.keyword.BluSoftlayer_notm}}
  {: #bx_commands_softlayer}
  
I comandi per la gestione di {{site.data.keyword.BluSoftlayer_notm}}} sono stati inglobati nella CLI Bluemix. Per ulteriori informazioni sull'utilizzo della CLI Bluemix per configurare e gestire i servizi {{site.data.keyword.BluSoftlayer_notm}}, vedi: [Comandi della CLI Bluemix {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl)](/docs/cli/reference/softlayer/index.md#softlayer_cli).
 
 ## Comandi per la gestione di account, organizzazioni e ruoli
 {: #bx_commands_account}

<table summary="Comandi Bluemix che puoi utilizzare per gestire account, organizzazioni, spazi e ruoli.">
<caption>Tabella 2. Comandi per gestire account, organizzazioni, spazi e ruoli</caption>
 <thead>
 <th colspan="5">Comandi per gestire account, organizzazioni, spazi e ruoli</th>
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


 ## Comandi per gestire i gruppi di risorse e le risorse
{: #bx_commands_resource}

<table summary="Comandi Bluemix che puoi utilizzare per gestire i gruppi di risorse e le risorse.">
  <caption>Tabella 3. Comandi per gestire i gruppi di risorse e le risorse</caption>
  <thead>
    <th colspan="5">Comandi per gestire i gruppi di risorse e le risorse</th>
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

 
 ## Comandi per gestire le politiche e le chiavi API
 {: #bx_commands_iam}
 <table summary="Comandi Bluemix che puoi utilizzare per gestire le politiche e le chiavi API.">
 <caption>Tabella 3. Comandi per gestire le politiche e le chiavi API</caption>
  <thead>
  <th colspan="5">Comandi per gestire le politiche e le chiavi API</th>
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
 
 ## Comandi per la gestione di applicazioni cf e di domini, rotte e certificati relativi all'applicazione
 {: #bx_commands_apps}

<table summary="comandi bluemix che puoi utilizzare per gestire le applicazioni cf e i domini, le rotte e i certificati relativi all'applicazione.">
<caption>Tabella 4. Comandi per gestire le applicazioni cf e i domini, le rotte e i certificati correlati alle applicazioni</caption>
 <thead>
 <th colspan="5">Comandi per gestire le applicazioni cf e i domini, le rotte e i certificati correlati alle applicazioni</th>
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
 
 ## Comandi per la gestione dei servizi Bluemix
 {: #bx_commands_services}

<table summary="Comandi bluemix che puoi utilizzare per la gestione dei servizi Bluemix.">
<caption>Tabella 5. Comandi per la gestione dei servizi Bluemix</caption>
 <thead>
 <th colspan="5">Comandi per la gestione dei servizi Bluemix</th>
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

 
 ## Comandi per la gestione delle impostazioni di fatturazione, plug-in e catalogo
 {: #bx_commands_settings}

<table summary="comandi bluemix che puoi utilizzare per gestire il catalogo, i plug-in, la fatturazione e le impostazioni di sicurezza Bluemix.">
<caption>Tabella 6. Comandi per la gestione delle impostazioni di sicurezza, dei plug-in, della fatturazione e del catalogo Bluemix</caption>
 <thead>
 <th colspan="5">Comandi per la gestione delle impostazioni di sicurezza, dei plug-in, della fatturazione e del catalogo Bluemix</th>
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
Visualizza la guida generale per i comandi integrati di primo livello e gli spazi dei nomi supportati della CLI {{site.data.keyword.Bluemix_notm}} oppure la guida per un comando o uno spazio dei nomi integrati specifici.

```
bluemix help [COMANDO|SPAZIONOMI]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>COMANDO|SPAZIONOMI (facoltativo)</dt>
   <dd>Il comando o lo spazio dei nomi per cui viene visualizzata la guida. Se non viene specificata, viene visualizzata la guida generale per la CLI {{site.data.keyword.Bluemix_notm}}.</dd>
   </dl>



<strong>Esempi</strong>:

Visualizza la guida generale per la CLI {{site.data.keyword.Bluemix_notm}}:

```
bluemix help
```

Visualizza la guida per il comando `info`:

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
Imposta o visualizza l'endpoint API {{site.data.keyword.Bluemix_notm}}.

```
bluemix api [ENDPOINT_API] [--unset] [--skip-ssl-validation]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
   <dl>
   <dt>ENDPOINT_API (facoltativo)</dt>
   <dd>L'endpoint API di destinazione, ad esempio `https://api.chinabluemix.net`. Se non vengono specificate entrambe le opzioni *ENDPOINT_API* e `--unset`, viene visualizzato l'endpoint API corrente.</dd>
   <dt>--unset (facoltativo)</dt>
   <dd>Rimuove l'impostazione di endpoint API.</dd>
   <dt>--skip-ssl-validation (facoltativo)</dt>
   <dd>Tralascia la convalida SSL delle richieste HTTP.</dd>
   </dl>
<strong>Esempi</strong>:

Imposta l'endpoint API su api.chinabluemix.net:

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

Visualizza l'endpoint API corrente:

```
bluemix api
```

Annulla l'impostazione dell'endpoint API:

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


Scrive i valori predefiniti nel file di configurazione.

```
bluemix config --http-timeout TIMEOUT_IN_SECONDI | --trace (true|false|path/to/file) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
   <dl>
   <dt>--http-timeout <i>TIMEOUT_IN_SECONDI</i></dt>
   <dd>Il valore di timeout per le richieste HTTP. Il valore predefinito è 60 secondi.</dd>
   <dt>--trace true|false|<i>percorso-al-file</i></dt>
   <dd>Traccia le richieste HTTP nel terminale o file specificato.</dd>
   <dt>--color true|false</dt>
   <dd>Abilita o disabilita l'output a colori. L'output a colori è abilitato per impostazione predefinita.</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>Imposta una locale predefinita. Se LOCALE è <i>CLEAR</i>, la locale precedente viene eliminata.</dd>
   <dt>--check-version true|false</dt>
   <dd>Abilita o disabilita il controllo della versione della CLI.</dd>
   </dl>

È possibile specificare solo una di queste opzioni alla volta.

<strong>Esempi</strong>:

Imposta il timeout della richiesta HTTP su 30 secondi:

```
bluemix config --http-timeout 30
```

Abilita l'output di traccia per le richieste HTTP:

```
bluemix config --trace true
```

Traccia le richieste HTTP in un file specificato */home/usera/my_trace*:

```
bluemix config --trace /home/usera/my_trace
```

Disabilita l'output a colori:

```
bluemix config --color false
```

Imposta la locale su zh_Hans:

```
bluemix config --locale zh_Hans
```

Cancella le impostazioni della locale:

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

Visualizza le informazioni su {{site.data.keyword.Bluemix_notm}} di base, compresi la regione corrente, la versione controller cloud e alcuni utili endpoint, quali gli endpoint per l'accesso e per lo scambio di token di accesso.

```
bluemix info
```

<strong>Prerequisiti</strong>:  Endpoint


## bluemix cf
{: #bluemix_cf}

Richiama la CLI CF integrata

```
bluemix [-q, --quiet] cf COMANDO...
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
<dl>
  <dt>-q, --quiet</dt>
  <dd>Disattiva il messaggio "Richiamo di comando cf..."</dd>
</dl>

<strong>Esempi</strong>:

Elenca le applicazioni cf:

```
bluemix cf apps
```

Elenca i servizi cf senza messaggio "Richiamo di comando cf...":

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

Esegue l'accesso dell'utente. 

```
bluemix login [-a ENDPOINT_API] [--sso] [-u NOMEUTENTE] [-p PASSWORD] [--apikey CHIAVE | @FILE_CHIAVI] [-c ID_ACCOUNT] [-o ORGANIZZAZIONE] [-s SPAZIO]
```

<strong>Prerequisiti</strong>:  Nessuno

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>Opzioni comando</strong>:
<dl>
  <dt> -a <i>ENDPOINT_API</i> (facoltativo)</dt>
  <dd> Endpoint API (ad esempio: api.ng.bluemix.net)</dd>
  <dt> --apikey <i>CHIAVE_API o @PERCORSO_FILE_CHIAVI_API</i>
  <dd> Contenuto della chiave API o percorso del file della chiave API indicato da @</dd>
  <dt> --sso (facoltativo) </dt>
  <dd> Utilizza un passcode monouso per effettuare l'accesso </dd>
  <dt> -u <i>NOMEUTENTE</i> (facoltativo)</dt>
  <dd> Nome utente</dd>
  <dt> -p <i>PASSWORD</i> (facoltativo)</dt>
  <dd> Password</dd>
  <dt> -c <i>ID_ACCOUNT</i> (facoltativo) </dt>
  <dd> ID dell'account di destinazione</dd>
  <dt> -o <i>NOME_ORGANIZZAZIONE</i> (facoltativo) </dt>
  <dd> Nome dell'organizzazione di destinazione </dd>
  <dt> -s <i>NOME_SPAZIO</i> (facoltativo) </dt>
  <dd> Nome dello spazio di destinazione</dd>
  <dt> --skip-ssl-validation (facoltativo) </dt>
  <dd> Tralascia la convalida SSL delle richieste HTTP. Questa opzione non è consigliata.</dd>
</dl>

<strong>Esempi</strong>:

#### Accesso interattivo

```
bluemix login
```

Accesso con nome utente e password e imposta l'account, l'organizzazione e lo spazio di destinazione:

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

Accesso con il passcode monouso e imposta l'account, l'organizzazione e lo spazio di destinazione

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

Accesso con la chiave API e imposta le destinazioni:

#### La chiave API ha un account associato

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### La chiave API non ha un account associato

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>Nota:</strong> se la chiave API ha un account associato, il passaggio a un altro account non è consentito.

#### Utilizza un passcode monouso

```
bluemix login -u IDUtente --sso
```

La CLI fornirà un link all'URL e richiederà il passcode:
```
Codice monouso (Ottienine uno in https://Link_URL_per_ottenere_il_passcode):
```

Apri il link in un browser per ottenere il passcode. Digita il passcode fornito nella console e dovresti essere in grado di accedere.

## bluemix logout
{: #bluemix_logout}

Disconnette l'utente.

```
bluemix logout
```

<strong>Prerequisiti</strong>:  Nessuno

## bluemix regions
{: #bluemix_regions}

Visualizza le informazioni per tutte le regioni su {{site.data.keyword.Bluemix_notm}}.

```
bluemix regions
```

<strong>Prerequisiti</strong>:  Endpoint


## bluemix target
{: #bluemix_target}


Imposta o visualizza l'account, la regione, l'organizzazione o lo spazio di destinazione.

```
bluemix target [-r NOME_REGIONE] [-c ID_ACCOUNT] [--cf] [-o ORGANIZZAZIONE] [-s SPAZIO]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>-r <i>NOME_REGIONE</i> (facoltativo)</dt>
   <dd>Nome della regione a cui essere passati, come 'us-south' o 'eu-gb'.</dd>
   <dt>-c <i>ID_ACCOUNT</i> (facoltativo)</dt>
   <dd>L'ID dell'account di destinazione.</dd>
   <dt>--cf</dt>
   <dd>Seleziona interattivamente l'organizzazione e lo spazio di destinazione</dd>
   <dt>-o <i>NOME_ORGANIZZAZIONE</i> (facoltativo)</dt>
   <dd>Il nome dell'organizzazione di destinazione.</dd>
   <dt>-s <i>NOME_SPAZIO</i> (facoltativo)</dt>
   <dd>Il nome dello spazio di destinazione.</dd>
   </dl>
Se nessuna delle opzioni viene specificata, vengono visualizzati l'account, la regione, l'organizzazione e lo spazio correnti.

<strong>Esempi</strong>:

Imposta l'account, l'organizzazione e lo spazio correnti:

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

Passa a una nuova regione:

```
bluemix target -r eu-gb
```

Visualizza l'account, la regione, l'organizzazione e lo spazio correnti:

```
bluemix target
```

### bluemix update
{: #bluemix_update}

Aggiorna la CLI alla versione più recente.

```
bluemix update
```

<strong>Prerequisiti</strong>:  Nessuno

### bluemix account orgs
{: #bluemix_account_orgs}

Elenca tutte le organizzazioni

```
bluemix account orgs [-r REGIONE] [--guid]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>-r <i>REGIONE</i> (facoltativo)</dt>
   <dd>Regione per cui vengono visualizzare le informazioni sull'organizzazione. Se impostato su 'all', vengono elencate tutte le organizzazioni in tutte le regioni.</dd>
   <dt>--guid (facoltativo)</dt>
   <dd>Visualizza il GUID delle organizzazioni.</dd>
   </dl>

<strong>Esempi</strong>:

Elenca tutte le organizzazioni della regione: `us-south` con il GUID visualizzato

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

Visualizza le informazioni per l'organizzazione specificata.

```
bluemix account org NOME_ORGANIZZAZIONE [--guid]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione.</dd>
   <dt>--guid (facoltativo)</dt>
   <dd>Visualizza il GUID dell'organizzazione.</dd>
   </dl>

<strong>Esempi</strong>:

Mostra le informazioni dell'organizzazione `IBM` con il GUID visualizzato

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

Crea una nuova organizzazione. Questa operazione può essere eseguita solo dal proprietario dell'account.

```
bluemix account org-create NOME_ORGANIZZAZIONE
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione in fase di creazione.</dd>
   </dl>

<strong>Esempi</strong>:

Crea un'organizzazione denominata `IBM`.

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

Replica un'organizzazione dalla regione corrente in un'altra regione.

```
bluemix account org-replicate NOME_ORGANIZZAZIONE NOME_REGIONE
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione esistente che deve essere replicata.</dd>
   <dt>NOME_REGIONE (obbligatorio)</dt>
   <dd>Il nome della regione che ospita l'organizzazione replicata.</dd>
   </dl>

<strong>Esempi</strong>:

Replica l'organizzazione `myorg` nella regione `eu-gb`:

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

Rinomina un'organizzazione. Questa operazione può essere eseguita solo da un gestore organizzazione.

```
bluemix account org-rename VECCHIO_NOME_ORGANIZZAZIONE NUOVO_NOME_ORGANIZZAZIONE
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_ORGANIZZAZIONE_PRECEDENTE (obbligatorio)</dt>
   <dd>Il vecchio nome dell'organizzazione da rinominare.</dd>
   <dt>NUOVO_NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nuovo nome con cui viene rinominata l'organizzazione.</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf spaces`.


## bluemix account space
{: #bluemix_account_space}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf space`.


## bluemix account space-create
{: #bluemix_account_space_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-space`.


## bluemix account space-rename
{: #bluemix_account_space_rename}


Questo comando ha la stessa funzione e le stesse opzioni del comando `cf rename-space`.


## bluemix account space-delete
{: #bluemix_account_space_delete}


Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-space`.

## bluemix account org-users
{: #bluemix_account_org_users}

Visualizza gli utenti nell'organizzazione specificata per il ruolo.

```
bluemix account org-users NOME_ORGANIZZAZIONE [-a]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
<dd>Il nome dell'organizzazione.</dd>
<dt>-a (facoltativo)</dt>
<dd>Elenca tutti gli utenti dell'organizzazione specificata, non raggruppati per ruolo.</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

Aggiunge un utente nell'organizzazione (è richiesto il gestore organizzazione).

```
 bluemix account org-user-add NOME_UTENTE ORGANIZZAZIONE
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

Rimuove un utente dall'organizzazione (gestore organizzazione o solo l'utente)

```
   bluemix account org-user-remove NOME_UTENTE ORGANIZZAZIONE [-f, --force]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--force, -f</dt>
<dd>Forza l'eliminazione senza conferma.</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

Ottiene tutti i ruoli organizzazione dell'utente corrente

```
bluemix account org-roles
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

Assegna un ruolo dell'organizzazione ad un utente. Questa operazione può essere eseguita solo da un gestore organizzazione.

```
bluemix account org-role-set NOME_UTENTE NOME_ORGANIZZAZIONE RUOLO_ORGANIZZAZIONE
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
  <dl>
   <dt>NOME_UTENTE (obbligatorio)</dt>
   <dd>Il nome dell'utente in fase di assegnazione.</dd>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione a cui viene assegnato l'utente.</dd>
   <dt>RUOLO_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome del ruolo organizzazione a cui viene assegnato l'utente. Ad esempio:
   <ul>
   <li>OrgManager: questo ruolo può invitare e gestire utenti, selezionare e modificare piani e impostare limiti di spesa.</li>
   <li>BillingManager: questo ruolo può creare e gestire l'account di fatturazione e le informazioni sul pagamento.</li>
   <li>OrgAuditor: questo ruolo dispone di un accesso in sola lettura a report e informazioni sull'organizzazione.</li>
   </ul>
   </dd>
  </dl>

<strong>Esempi</strong>:

Assegna l'utente `Mary` all'organizzazione `IBM` con il ruolo `OrgManager`:

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: puoi impostare i ruoli org/space utilizzando la CLI ma, se vuoi impostare le altre autorizzazioni, devi utilizzare l'IU. Per ulteriori dettagli, vedi [Assegnazione dell'accesso utente](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

Rimuove un ruolo dell'organizzazione da un utente. Questa operazione può essere eseguita solo da un gestore organizzazione.

```
bluemix account org-role-unset NOME_UTENTE NOME_ORGANIZZAZIONE RUOLO_ORGANIZZAZIONE
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_UTENTE (obbligatorio)</dt>
   <dd>Il nome dell'utente in fase di eliminazione.</dd>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione da cui viene eliminato l'utente.</dd>
   <dt>RUOLO_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome del ruolo organizzazione da cui viene eliminato l'utente. Ad esempio:
   <ul>
   <li>OrgManager: questo ruolo può invitare e gestire utenti, selezionare e modificare piani e impostare limiti di spesa.</li>
   <li>BillingManager: questo ruolo può creare e gestire l'account di fatturazione e le informazioni sul pagamento.</li>
   <li>OrgAuditor: questo ruolo dispone di un accesso in sola lettura a report e informazioni sull'organizzazione.</li>
   </ul>
   </dd>
    </dl>

<strong>Esempi</strong>:

Rimuove l'utente `Mary` dall'organizzazione `IBM` con il ruolo `OrgManager`:

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

Visualizza gli utenti nello spazio specificato per il ruolo.

```
bluemix account space-users NOME_ORGANIZZAZIONE NOME_SPAZIO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione.</dd>
   <dt>NOME_SPAZIO (obbligatorio)</dt>
   <dd>Il nome dello spazio.</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

Assegna un ruolo dello spazio ad un utente. Questa operazione può essere eseguita solo da un gestore spazio.

```
bluemix account space-role-set NOME_UTENTE NOME_ORGANIZZAZIONE NOME_SPAZIO RUOLO_SPAZIO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_UTENTE (obbligatorio)</dt>
   <dd>Il nome dell'utente in fase di assegnazione.</dd>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione a cui viene assegnato l'utente.</dd>
   <dt>NOME_SPAZIO (obbligatorio)</dt>
   <dd>Il nome dello spazio a cui è assegnato l'utente.</dd>
   <dt>RUOLO_SPAZIO (obbligatorio)</dt>
   <dd>Il nome del ruolo spazio a cui è assegnato l'utente. Ad esempio:
   <ul>
   <li>SpaceManager: questo ruolo può invitare e gestire utenti e attivare funzioni per un dato spazio.</li>
   <li>SpaceDeveloper: questo ruolo può creare e gestire applicazioni e servizi e visualizzare log e report.</li>
   <li>SpaceAuditor: questo ruolo può visualizzare log, report e impostazioni per lo spazio.</li>
   </ul></dd>
    </dl>

<strong>Esempi</strong>:

Assegna l'utente `Mary` all'organizzazione `IBM` e allo spazio `Cloud` con il ruolo `SpaceManager`:

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

Rimuove un ruolo dello spazio da un utente. Questa operazione può essere eseguita solo da un gestore spazio.

```
bluemix account space-role-unset NOME_UTENTE NOME_ORGANIZZAZIONE NOME_SPAZIO RUOLO_SPAZIO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_UTENTE (obbligatorio)</dt>
   <dd>Il nome dell'utente in fase di eliminazione.</dd>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione da cui viene eliminato l'utente.</dd>
   <dt>NOME_SPAZIO (obbligatorio)</dt>
   <dd>Il nome dello spazio da cui viene eliminato l'utente.</dd>
   <dt>RUOLO_SPAZIO (obbligatorio)</dt>
   <dd>Il nome del ruolo spazio da cui viene eliminato l'utente. Ad esempio:
   <ul>
   <li>SpaceManager: questo ruolo può invitare e gestire utenti e attivare funzioni per un dato spazio.</li>
   <li>SpaceDeveloper: questo ruolo può creare e gestire applicazioni e servizi e visualizzare log e report.</li>
   <li>SpaceAuditor: questo ruolo può visualizzare log, report e impostazioni per lo spazio.</li>
   </ul></dd>
    </dl>


<strong>Esempi</strong>:

Rimuove l'utente `Mary` dall'organizzazione `IBM` e dall spazio `Cloud` con il ruolo `SpaceManager`:

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

Elenca tutti gli account dell'utente corrente

```
bluemix account list
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso


## bluemix account org-account
{: #bluemix_account_org_account}

Visualizza l'account dell'organizzazione specificata (utente dell'organizzazione obbligatorio)

```
bluemix account org-account NOME_ORGANIZZAZIONE [--guid]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
  <dt>--guid (facoltativo)</dt>
  <dd>Visualizza solo l'ID account</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

Visualizza gli utenti associati con l'account. Questa operazione può essere eseguita solo dal proprietario dell'account.

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

Elimina un utente dall'account corrente (solo il proprietario dell'account)

```
bluemix account user-delete NOMEUTENTE [-c ID_ACCOUNT] [-f]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOMEUTENTE (obbligatorio)</dt>
<dd>Nome utente</dd>
<dt>-c ID_ACCOUNT</dt>
<dd>ID account. Se non specificato, il valore predefinito è l'account corrente.</dd>
<dt>--force, -f (facoltativo)</dt>
<dd>Forza l'eliminazione senza conferma.</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

Invita un utente nell'account con un'organizzazione e un ruolo spazio già impostati. Questa operazione può essere eseguita solo dal proprietario dell'account.

```
bluemix account user-invite NOME_UTENTE NOME_ORGANIZZAZIONE RUOLO_ORGANIZZAZIONE NOME_SPAZIO RUOLO_SPAZIO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
   <dt>NOME_UTENTE (obbligatorio)</dt>
   <dd>Il nome dell'utente invitato.</dd>
   <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome dell'organizzazione in cui viene invitato l'utente.</dd>
   <dt>RUOLO_ORGANIZZAZIONE (obbligatorio)</dt>
   <dd>Il nome del ruolo organizzazione in cui viene invitato l'utente. Ad esempio:
   <ul>
  <li>OrgManager: questo ruolo può invitare e gestire utenti, selezionare e modificare piani e impostare limiti di spesa.</li>
  <li>BillingManager: questo ruolo può creare e gestire l'account di fatturazione e le informazioni sul pagamento.</li>
  <li>OrgAuditor: questo ruolo dispone di un accesso in sola lettura a report e informazioni sull'organizzazione.</li>
  </ul> </dd>
   <dt>NOME_SPAZIO (obbligatorio)</dt>
   <dd>Il nome dello spazio in cui viene invitato l'utente.</dd>
   <dt>RUOLO_SPAZIO (obbligatorio)</dt>
   <dd>Il nome dello spazio in cui viene invitato l'utente. Il nome del ruolo spazio in cui viene invitato l'utente. Ad esempio:
   <ul>
<li>SpaceManager: questo ruolo può invitare e gestire utenti e attivare funzioni per un dato spazio.</li>
<li>SpaceDeveloper: questo ruolo può creare e gestire applicazioni e servizi e visualizzare log e report.</li>
<li>SpaceAuditor: questo ruolo può visualizzare log, report e impostazioni per lo spazio.</li>
</ul>
</dd>
</dl>

<strong>Esempi</strong>:

Invita l'utente `Mary` nell'organizzazione `IBM` con il ruolo `OrgManager` e lo spazio `Cloud` con il ruolo `SpaceAuditor`:

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: puoi impostare i ruoli org/space durante l'invito utilizzando la CLI ma, se vuoi impostare le altre autorizzazioni, devi utilizzare l'IU. Per ulteriori dettagli, vedi [Assegnazione dell'accesso utente](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

Invia di nuovo l'invito a un utente (è richiesto il gestore organizzazione o il proprietario account)

```
bluemix account user-reinvite EMAIL_UTENTE NOME_ORGANIZZAZIONE
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

Elenca tutti gli ID servizio

```
bluemix iam service-ids --uuid
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Mostra l'UUID solo degli ID servizio</dd>
</dl>

<strong>Esempi</strong>:
elenca l'UUID di tutti gli ID servizio sotto l'account corrente

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

Visualizza i dettagli di un ID servizio

```
bluemix iam service-id NOME [--uuid]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del servizio</dd>
  <dt>-uuid</dt>
  <dd>Visualizza l'UUID dell'ID servizio</dd>
</dl>

<strong>Esempi</strong>:

Mostra i dettagli dell'ID servizio `sample-test`

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

Crea un ID servizio

```
bluemix iam service-id-create NOME [-d, --description DESCRIZIONE]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del servizio</dd>
  <dt>-d, --description</dt>
  <dd>Descrizione dell'ID servizio</dd>
</dl>

<strong>Esempi</strong>:

Crea un ID servizio con il nome servizio `sample-test` e la descrizione `hello, world!`

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
Aggiorna un ID servizio

```
bluemix iam service-id-update NOME [-n, --name NUOVO_NOME] [-d, --description DESCRIZIONE] [-v, --version VERSIONE] [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del servizio</dd>
  <dt>-n, --name</dt>
  <dd>Nuovo nome del servizio</dd>
  <dt>-d, --description</dt>
  <dd>Nuova descrizione del servizio</dd>
  <dt>-v, --version</dt>
  <dd>Versione dell'ID servizio</dd>
  <dt>-f, --force</dt>
  <dd>Aggiorna senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Rinomina l'ID servizio `sample-test` come `sample-test-2` senza conferma

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

Aggiorna la descrizione del servizio `sample-test` versione `1-0jn39fbefew`

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

Elimina un ID servizio

```
bluemix iam service-id-delete NOME [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del servizio</dd>
  <dt>-f, --force</dt>
  <dd>Elimina senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Elimina l'ID servizio `sample-teset` senza conferma

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

Elenca tutte le chiavi API della piattaforma Bluemix

```
bluemix iam api-keys
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

Crea una nuova chiave API della piattaforma Bluemix

```
bluemix iam api-key-create NOME [-d DESCRIZIONE] [-f, --file FILE]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME (obbligatorio)</dt>
<dd>Nome della chiave API da creare.</dd>
<dt>-d <i>DESCRIZIONE</i> (facoltativo)</dt>
<dd>Descrizione della chiave API</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>Salva le informazioni della chiave API nel file specificato. Se non impostato, verrà visualizzato il contenuto JSON.</dd>
</dl>

<strong>Esempi</strong>:

Crea una chiave API e salva in un file

```
bluemix iam api-key-create MyKey -d "questa è la mia chiave API" -f file_chiave
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Aggiorna una chiave API della piattaforma Bluemix

```
bluemix iam api-key-update NOME [-n NOME] [-d DESCRIZIONE]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME (obbligatorio)</dt>
<dd>Il vecchio nome della chiave API da aggiornare.</dd>
<dt>-n <i>NOME</i> (facoltativo)</dt>
<dd>Il nuovo nome della chiave API</dd>
<dt>-d <i>DESCRIZIONE</i> (facoltativo)</dt>
<dd>La nuova descrizione della chiave API</dd>
</dl>

<strong>Esempi</strong>:

Aggiorna la descrizione di una chiave API:

```
bluemix iam api-key-update MyKey -d "la nuova descrizione della mia chiave"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Elimina una chiave API della piattaforma Bluemix

```
bluemix iam api-key-delete NOME [-f]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME (obbligatorio)</dt>
<dd>Nome della chiave API da eliminare.</dd>
<dt>-f (facoltativo)</dt>
<dd>Forza l'eliminazione senza conferma.</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

Elenca tutte le chiavi API di servizio

```
bluemix iam service-api-keys ASSOCIATE_A 
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
</dl>

<strong>Esempi</strong>:

Elenca le chiavi API di servizio associate al CRN di servizio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

Elenca i dettagli di una chiave API di servizio

```
bluemix iam service-api-key NOME ASSOCIATA_A [--uuid]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Visualizza l'UUID della chiave API di servizio</dd>
</dl>

<strong>Esempi</strong>:

Mostra i dettagli della chiave API di servizio `sample-key` associata al CRN di servizio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

Crea una chiave API di servizio

```
bluemix iam service-api-key-create NOME ASSOCIATA_A [-d, --description DESCRIZIONE] [-f, --file FILE]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-d, --description</dt>
  <dd>Descrizione della chiave API</dd>
  <dt>-f, --file</dt>
  <dd>Salva le informazioni della chiave API nel file specificato. Se non impostato, verrà visualizzato il contenuto JSON.</dd>
</dl>

<strong>Esempi</strong>:

Crea una chiave API di servizio `sample-key` associata al CRN di servizio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da` :

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

Aggiorna una chiave API di servizio

```
bluemix iam service-api-key-update NOME ASSOCIATA_A  [-n, --name NUOVO_NOME] [-d, --description DESCRIZIONE] [-v, --version VERSIONE] [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-n, --name</dt>
  <dd>Nuovo nome della chiave API di servizio</dd>
  <dt>-d, --description</dt>
  <dd>Nuova descrizione della chiave API di servizio</dd>
  <dt>-v, --version</dt>
  <dd>Versione della chiave API di servizio</dd>
  <dt>-f, --force</dt>
  <dd>Aggiorna senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Rinomina la chiave API di servizio `sample-key` come `new-sample-key` :

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

Elimina una chiave API di servizio

```
bluemix iam service-api-key-delete NOME ASSOCIATA_A [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Elimina senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Elimina la chiave API di servizio `sample-key` :

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

Elenca le politiche dell'utente `name@example.com`:

```
bluemix iam user-policies name@example.com
```

<strong>Prerequisiti</strong>: Endpoint, Accesso, Account di destinazione

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME_UTENTE (obbligatorio)</dt>
<dd>Nome utente a cui appartengono le politiche</dd>
</dl>

<strong>Esempi</strong>:

Elenca le politiche dell'utente `name@example.com`:

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

Visualizza i dettagli di una politica utente

```
bluemix iam user-policy NOME_UTENTE ID_POLITICA
```

<strong>Prerequisiti</strong>: Endpoint, Accesso, Account di destinazione

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME_UTENTE (obbligatorio)</dt>
<dd>Nome utente a cui appartiene la politica</dd>
<dt>ID_POLITICA (obbligatorio)</dt>
<dd>ID della politica</dd>
</dl>

<strong>Esempi</strong>:

Elenca la politica `0bb730daa` dell'utente `name@example.com`:

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

Crea una politica utente

```
bluemix iam user-policy-create NOME_UTENTE {-f, --file FILE_JSON | --roles NOME_RUOLO1,NOME_RUOLO2... [--service-name NOME_SERVIZIO] [--service-instance ISTANZA_SERVIZIO] [--region REGIONE] [--resource-type TIPO_RISORSA] [--resource RISORSA] [--resource-group-name NOME_GRUPP_RISORSE] [--resouce-group-id ID_GRUPPO_RISORSE]}
```

<strong>Prerequisiti</strong>: Endpoint, Accesso, Account di destinazione

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME_UTENTE (obbligatorio)</dt>
<dd>Nome utente a cui appartiene la politica</dd>
<dt>-f, --file <i>FILE</i> (facoltativo)</dt>
<dd>File JSON della definizione della politica</dd>
<dt>--roles <i>NOME_RUOLO1,NOME_RUOLO2...</i> (facoltativo)</dt>
<dt>--service-name <i>NOME_SERVIZIO</i> (facoltativo)</dt>
<dd>Nome del servizio della definizione della politica, che è esclusivo con l'indicatore '-f, --file'.</dd>
<dt>--serivce-instance <i>ISTANZA_SERVIZIO</i> (facoltativo)</dt>
<dd>Istanza del servizio della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--region <i>REGIONE</i> (facoltativo)</dt>
<dd>Regione della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--resource-type <i>TIPO_RISORSA</i> (facoltativo)</dt>
<dd>Tipo di risorsa della definizione della politica, che è esclusivo con l'indicatore '-f, --file'.</dd>
<dt>--resource <i>RISORSA</i> (facoltativo)</dt>
<dd>Risorsa della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--resource-group-name <i>NOME_GRUPPO_RISORSE</i> (facoltativo)</dt>
<dd>Nome del gruppo di risorse, che è esclusivo con gli indicatori '-f, --file', '--resource' e '--resource-group-id'.</dd>
<dt>--resource-group-id <i>ID_GRUPPO_RISORSE</i> (facoltativo)</dt>
<dd>ID del gruppo di risorse, che è esclusivo con gli indicatori '-f, --file', '--resource' e '--resource-group-name'.</dd>
  <dd>Nomi dei ruoli della definizione della politica. Per i ruoli supportati di uno specifico servizio, esegui 'bluemix iam roles --service NOME_SERVIZIO'. Questa opzione è esclusiva con '-f, --file'.</dd>
</dl>

<strong>Esempi</strong>:

Crea la politica utente per l'utente `name@example.com` dal file JSON di politiche `policy.json`:

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

Dai a `name@example.com` il ruolo di amministratore (`Administrator`) per tutte le risorse `sample-service`:

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

Dai a `name@example.com` il ruolo di editor (`Editor`) per la risorsa `key123` dell'istanza del servizio di esempio `ServiceId-ade78e9f` nella regione `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Dai a `name@example.com` il ruolo di operatore (`Operator`) per il gruppo di risorse con ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Dai a `name@example.com` il ruolo di visualizzatore (`Viewer`) per i membri del gruppo di risorse `sample-resource-group`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

Dai a `name@example.com` il ruolo di visualizzatore (`Viewer`) per i membri del gruppo di risorse con ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

Aggiorna una politica utente

```
bluemix iam user-policy-update NOME_UTENTE ID_POLITICA [-v, --version VERSIONE] {-f, --file FILE_JSON | [--roles NOME_RUOLO1,NOME_RUOLO2...] [--service-name NOME_SERVIZIO] [--service-instance ISTANZA_SERVIZIO] [--region REGIONE] [--resource-type TIPO_RISORSA] [--resource RISORSA] [--resource-group-name NOME_GRUPPO_RISORSE] [--resource-group-id ID_GRUPPO_RISORSE]}
```

<strong>Prerequisiti</strong>: Endpoint, Accesso, Account di destinazione

<strong>Opzioni comando</strong>:
<dt>NOME_UTENTE (obbligatorio)</dt>
<dd>Nome utente a cui appartiene la politica</dd>
<dt>ID_POLITICA (obbligatorio)</dt>
<dd>ID della politica da aggiornare</dd>
<dt>-v, --version <i>VERSIONE</i> (facoltativo)</dt>
<dd>Versione della politica esistente</dd>
<dt>-f, --file <i>FILE</i> (facoltativo)</dt>
<dd>File JSON della definizione della politica</dd>
<dt>-f, --file <i>FILE</i> (facoltativo)</dt>
<dd>File JSON della definizione della politica</dd>
<dt>--roles <i>NOME_RUOLO1,NOME_RUOLO2...</i> (facoltativo)</dt>
<dt>--service-name <i>NOME_SERVIZIO</i> (facoltativo)</dt>
<dd>Nome del servizio della definizione della politica, che è esclusivo con l'indicatore '-f, --file'.</dd>
<dt>--serivce-instance <i>ISTANZA_SERVIZIO</i> (facoltativo)</dt>
<dd>Istanza del servizio della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--region <i>REGIONE</i> (facoltativo)</dt>
<dd>Regione della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--resource-type <i>TIPO_RISORSA</i> (facoltativo)</dt>
<dd>Tipo di risorsa della definizione della politica, che è esclusivo con l'indicatore '-f, --file'.</dd>
<dt>--resource <i>RISORSA</i> (facoltativo)</dt>
<dd>Risorsa della definizione della politica, che è esclusiva con l'indicatore '-f, --file'.</dd>
<dt>--resource-group-name <i>NOME_GRUPPO_RISORSE</i> (facoltativo)</dt>
<dd>Nome del gruppo di risorse, che è esclusivo con gli indicatori '-f, --file', '--resource' e '--resource-group-id'.</dd>
<dt>--resource-group-id <i>ID_GRUPPO_RISORSE</i> (facoltativo)</dt>
<dd>ID del gruppo di risorse, che è esclusivo con gli indicatori '-f, --file', '--resource' e '--resource-group-name'.</dd>
  <dd>Nomi dei ruoli della definizione della politica. Per i ruoli supportati di uno specifico servizio, esegui 'bluemix iam roles --service NOME_SERVIZIO'. Questa opzione è esclusiva con '-f, --file'.</dd>
</dl>

<strong>Esempi</strong>:

Aggiorna la politica utente con quella nel file JSON

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

Aggiorna la politica utente per dare a `name@example.com` il ruolo di amministratore (`Administrator`) per tutte le risorse `sample-service`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 Aggiorna la politica utente per dare a `name@example.com` il ruolo di editor (`Editor`) per la risorsa `key123` dell'istanza del servizio di esempio `ServiceId-ade78e9f` nella regione `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Aggiorna la politica utente per dare a `name@example.com` il ruolo di operatore (`Operator`) per il gruppo di risorse con ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Aggiorna la politica utente per dare a `name@example.com` il ruolo di visualizzatore (`Viewer`) per i membri del gruppo di risorse `sample-resource-group`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

Aggiorna la politica utente per dare a `name@example.com` il ruolo di visualizzatore (`Viewer`) per i membri del gruppo di risorse con ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

Elenca tutte le politiche di servizio del servizio specificato

```
bluemix iam service-policies NOME_ID_SERVIZIO [--json] [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ID_SERVIZIO (obbligatorio)</dt>
  <dd>Nome dell'ID servizio</dd>
  <dt>-json</dt>
  <dd>Visualizza la politica in formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Visualizza le politiche di servizio senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Elenca le politiche del servizio `test`:

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

Visualizza i dettagli di una politica di servizio

```
bluemix iam service-policy NOME_ID_SERVIZIO ID_POLITICA [--json] [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ID_SERVIZIO (obbligatorio)</dt>
  <dd>Nome dell'ID servizio</dd>
  <dt>ID_POLITICA (obbligatorio)</dt>
  <dd>ID della politica di servizio<dd>
  <dt>-json</dt>
  <dd>Visualizza la politica in formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Visualizza la politica di servizio senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Mostra la politica `140798e2-8ea7db3` del servizio `test`:

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

Crea una politica di servizio

```
bluemix iam service-policy-create NOME_ID_SERVIZIO {-f, --file FILE_JSON | -r, --roles NOME_RUOLO1,NOME_RUOLO2... [--service-name NOME_SERVIZIO] [--service-instance ISTANZA_SERVIZIO] [--region REGIONE] [--resource-type TIPO_RISORSA] [--resource RISORSA]} [-F, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ID_SERVIZIO (obbligatorio)</dt>
  <dd>Nome dell'ID servizio</dd>
  <dt>-f, --file</dt>
  <dd>File JSON della definizione della politica. È esclusivo con gli indicatori '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' e  '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Nomi dei ruoli della definizione della politica. Per i ruoli supportati di uno specifico servizio, esegui 'bluemix iam roles --service NOME_SERVIZIO'. Questa opzione è esclusiva con '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nome del servizio della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Istanza del servizio della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Regione della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo di risorsa della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Risorsa della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Crea politica di servizio senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Crea la politica di servizio dal file JSON per il servizio `test`:

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

Aggiorna una politica di servizio

```
bluemix iam service-policy-update NOME_ID_SERVIZIO ID_POLITICA [-v, --version VERSIONE] {-f, --file FILE_JSON | [-r, --roles NOME_RUOLO1,NOME_RUOLO2...] [--service-name NOME_SERVIZIO] [--service-instance ISTANZA_SERVIZIO] [--region REGIONE] [--resource-type TIPO_RISORSA] [--resource RISORSA]} [-F, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ID_SERVIZIO (obbligatorio)</dt>
  <dd>Nome dell'ID servizio</dd>
  <dt>ID_POLITICA (obbligatorio)</dt>
  <dd>ID della politica di servizio<dd>
  <dt>-v, --version</dt>
  <dd>Versione della politica di servizio</dd>
  <dt>-f, --file</dt>
  <dd>File JSON della definizione della politica. È esclusivo con gli indicatori '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' e  '--resource'.</dd>
  <dt>-r, --roles</dt>
  <dd>Nomi dei ruoli della definizione della politica. Per i ruoli supportati di uno specifico servizio, esegui 'bluemix iam roles --service NOME_SERVIZIO'. Questa opzione è esclusiva con '-f, --file'.</dd>
  <dt>-service-name</dt>
  <dd>Nome del servizio della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-service-instance</dt>
  <dd>Istanza del servizio della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-region</dt>
  <dd>Regione della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo di risorsa della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-resource</dt>
  <dd>Risorsa della definizione della politica. È esclusivo con l'indicatore '-f, --file'.</dd>
  <dt>-F, --force</dt>
  <dd>Aggiorna la politica di servizio senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Aggiorna la politica di servizio `140798e2-8ea7db3` dal file JSON per il servizio `test`:

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

Elimina una politica di servizio

```
bluemix iam service-policy-delete NOME_ID_SERVIZIO ID_POLITICA [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ID_SERVIZIO (obbligatorio)</dt>
  <dd>Nome dell'ID servizio</dd>
  <dt>ID_POLITICA (obbligatorio)</dt>
  <dd>ID della politica di servizio<dd>
  <dt>-f, --force</dt>
  <dd>Elimina senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Elimina la politica `140798e2-8ea7db3` del servizio `test`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

Elenca i gruppi di risorse

```
bluemix resource groups [--default | (-r, --resource ID_RISORSA -o, --resource-origin ORIGINE_RISORSA)]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>--default</dt>
  <dd>Ottieni il gruppo predefinito dell'account corrente</dd>
  <dt>-r, --resource</dt>
  <dd>ID della risorsa di appartenenza</dd>
  <dt>-o, --resource-origin</dt>
  <dd>Origine della risorsa di appartenenza. Valori accettati: 'CF_ORG', 'IMS_ACCOUNT'.</dd>
</dl>

<strong>Esempi</strong>:

Elenca tutti i gruppi di risorse nell'attuale account di destinazione:

```
bluemix resource groups
```

Elenca il gruppo predefinito dell'attuale account di destinazione:

```
bluemix resource groups --default
```

Elenco i gruppi di risorse che sono un'associazione di un'organizzazione CloudFoundry

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

Mostra i dettagli di un gruppo di risorse

```
bluemix resource group NOME [--id]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del gruppo di risorse</dd>
  <dt>--id</dt>
  <dd>Mostra solo l'ID</dd>
</dl>

<strong>Esempi</strong>:

Mostra il gruppo di risorse `example-group`:

```
bluemix resource group example-group
```

Mostra solo l'ID del gruppo di risorse `example-group`:

```
bluemix resource group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

Aggiorna un gruppo di risorse esistente

```
bluemix resource group-update NOME [-n, --name NUOVO_NOME] [-q, --quota NUOVO_NOME_QUOTA]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome del gruppo di risorse di destinazione</dd>
  <dt>-n, --name</dt>
  <dd>Nuovo nome del gruppo di risorse</dd>
  <dt>-q, --quota</dt>
  <dd>Nome della nuova definizione di quota</dd>
  <dt>-f</dt>
  <dd>Forza l'aggiornamento senza conferma</dd>
</dl>

<strong>Esempi</strong>:

Rinomina il gruppo di risorse `example-group` come `trial-group`:

```
bluemix resource group-update example-group -n trial-group
```

Modifica la quota del gruppo di risorse `example-group` come `free`:

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

Elenca tutte le definizioni di quota

```
bluemix resource quotas
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
</dl>

<strong>Esempi</strong>:

Elenca tutte le definizioni di quota:

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

Mostra i dettagli di una definizione di quota

```
bluemix resource quota NOME
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome della quota</dd>
</dl>

<strong>Esempi</strong>:
mostra i dettagli della quota `free`:

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf push`.


## bluemix app list
{: #bluemix_app_list}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf apps`.


## bluemix app show
{: #bluemix_app_show}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf app`.


## bluemix app delete
{: #bluemix_app_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete`.


## bluemix app rename
{: #bluemix_app_rename}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf rename`.


## bluemix app start
{: #bluemix_app_start}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf start`.


## bluemix app stop
{: #bluemix_app_stop}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf stop`.


## bluemix app restart
{: #bluemix_app_restart}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf restart`.


## bluemix app restage
{: #bluemix_app_restage}


Questo comando ha la stessa funzione e le stesse opzioni del comando `cf restage`.


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


Questo comando ha la stessa funzione e le stesse opzioni del comando `cf restart-app-instance`.


## bluemix app events
{: #bluemix_app_events}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf events`.


## bluemix app files
{: #bluemix_app_files}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf files`.


## bluemix app logs
{: #bluemix_app_logs}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf logs`.


## bluemix app env
{: #bluemix_app_env}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf env`.


## bluemix app env-set
{: #bluemix_app_env_set}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf set-env`.


## bluemix app env-unset
{: #bluemix_app_env_unset}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf unset-env`.


## bluemix app stacks
{: #bluemix_app_stacks}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf stacks`.


## bluemix app stack-show
{: #bluemix_app_stack_show}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf stack`.


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-app-manifest`.

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

Elenca le informazioni sul certificato di un dominio.

```
bluemix app domain-cert NOME_DOMINIO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
<dl>
<dt>NOME_DOMINIO (obbligatorio)</dt>
<dd>Il dominio che ospita il certificato.</dd>
</dl>


<strong>Esempi</strong>:

Visualizza le informazioni sul certificato del dominio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

Aggiunge un certificato al dominio specificato nell'organizzazione corrente.

```
bluemix app domain-cert-add DOMINIO -k FILE_CHIAVE PRIVATA -c FILE_CERTIFICATO [-p PASSWORD] [-i FILE_CERTIFICATO_INTERMEDIO] [-t FILE_TRUSTSTORE]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
   <dl>
   <dt>DOMINIO (obbligatorio)</dt>
   <dd>Il dominio a cui viene aggiunto il certificato.</dd>
   <dt>-k <i>FILE_CHIAVE PRIVATA</i> (obbligatorio)</dt>
   <dd>Il percorso del file della chiave privata.</dd>
   <dt>-c <i>FILE_CERTIFICATO</i> (obbligatorio)</dt>
   <dd>Il percorso del file del certificato.</dd>
   <dt>-p <i>PASSWORD</i> (facoltativo)</dt>
   <dd>La password per il certificato.</dd>
   <dt>-i <i>FILE_CERTIFICATO_INTERMEDIO</i> (optional)</dt>
   <dd>Il percorso del file di certificato intermedio.</dd>
   <dt>-t <i>FILE_TRUSTSTORE</i> (facoltativo)</dt>
   <dd>Il file truststore.</dd>
   </dl>


<strong>Esempi</strong>:

Aggiunge un certificato al dominio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

Rimuove un certificato dal dominio specificato nell'organizzazione corrente.

```
bluemix app domain-cert-remove DOMINIO [-f]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:

   <dl>
   <dt>DOMINIO (obbligatorio)</dt>
   <dd>Il dominio da cui rimuovere il certificato.</dd>
   <dt>-f (facoltativo)</dt>
   <dd>Forza l'eliminazione senza conferma.</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-shared-domain`.

## bluemix app routes
{: #bluemix_app_routes}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf routes`.


## bluemix app route-check
{: #bluemix_app_route_check}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf check-route`.


## bluemix app route-map
{: #bluemix_app_route_map}

Associa una rotta a un'applicazione cf o a un gruppo di contenitori esistenti che hanno il dominio e il nome host specificati.

```
bluemix app route-map NOME_APPLICAZIONE_CF|NOME_GRUPPO_CONTENITORE  DOMINIO  [-n NOME_HOST]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_APPLICAZIONE_CF|NOME_GRUPPO_CONTENITORI (obbligatorio)</dt>
   <dd>Il nome dell'applicazione cf o del gruppo di contenitori da associare a una rotta.</dd>
   <dt>DOMINIO (obbligatorio)</dt>
   <dd>Il dominio della rotta. Ad esempio, mychinabluemix.net o chinabluemix.net. </dd>
   <dt>-n <i>NOME_HOST</i> (facoltativo)</dt>
   <dd>Il nome host della rotta. Se non viene fornito, il nome host è impostato sul nome applicazione o sul nome gruppo di contenitori per impostazione predefinita.</dd>
   </dl>

<strong>Esempi</strong>:

Associa una rotta `my-app` con il dominio specificato:

```
bluemix app route-map my-app mychinabluemix.net
```

Associa una rotta a 'my-container-group' con il dominio e il nome host specificati:

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

Annulla l'associazione della rotta specificata a un'applicazione cf o a un gruppo di contenitori esistenti.

```
bluemix app route-unmap NOME_APPLICAZIONE_CF|NOME_GRUPPO_CONTENITORE  DOMINIO  [-n NOME_HOST]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_APPLICAZIONE_CF|NOME_GRUPPO_CONTENITORI (obbligatorio)</dt>
   <dd>Il nome dell'applicazione cf o del gruppo di contenitori.</dd>
   <dt>DOMINIO (obbligatorio)</dt>
   <dd>Il dominio della rotta (ad esempio, mychinabluemix.net o chinabluemix.net).</dd>
   <dt>-n <i>NOME_HOST</i> (facoltativo)</dt>
   <dd>Il nome host della rotta. Se non viene fornito, il nome host è impostato sul nome applicazione o sul nome gruppo di contenitori per impostazione predefinita.</dd>
   </dl>

<strong>Esempi</strong>:

Annulla l'associazione di `my-app.mychinabluemix.net` da `my-app`:

```
bluemix app route-unmap my-app mychianbluemix.net
```

Annulla l'associazione di `abc.chinabluexmix.net` da `my-container-group`:

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-route`.


## bluemix app route-delete
{: #bluemix_app_route_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-route`.


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-orphaned-routes`.


## bluemix app domains
{: #bluemix_app_domains}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-shared-domain`.


## bluemix service offerings
{: #bluemix_service_offerings}


Questo comando ha la stessa funzione e le stesse opzioni del comando `cf marketplace`.


## bluemix service list
{: #bluemix_service_list}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf services`.


## bluemix service show
{: #bluemix_service_show}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf service`.


## bluemix service create
{: #bluemix_service_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-service`.


## bluemix service update
{: #bluemix_service_update}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf update-service`.


## bluemix service delete
{: #bluemix_service_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-service`.


## bluemix service rename
{: #bluemix_service_rename}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf rename-service`.


## bluemix service bind
{: #bluemix_service_bind}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf bind-service`.


## bluemix service unbind
{: #bluemix_service_unbind}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf unbind-service`.


## bluemix service key-create
{: #bluemix_service_key_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-service-key`.


## bluemix service key-delete
{: #bluemix_service_key_delete}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf delete-service-key`.


## bluemix service keys
{: #bluemix_service_keys}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf service-keys`.


## bluemix service key-show
{: #bluemix_service_key_show}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf service-key`.


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf create-user-provided-service`.


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

Questo comando ha la stessa funzione e le stesse opzioni del comando `cf update-user-provided-service`.


## bluemix resource instances
{: #bluemix_resource_instances}

Elenca le istanze della risorsa

```
bluemix resource instances [--resource-name NOME_RISORSA] [-r, --region ID_REGIONE] [--long]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>--resource-name</dt>
  <dd>Nome della risorsa di appartenenza</dd>
  <dt>-r, --region</dt>
  <dd>Filtra in base all'ID regione; se non viene specificato, il valore predefinito è la regione corrente; '-r, --region all' per visualizzare le istanze della risorsa in tutte le regioni</dd>
  <dt>--long</dt>
  <dd>Mostra dei campi aggiuntivi nell'output</dd>
</dl>

<strong>Esempi</strong>:

Elenca le istanze della risorsa `test-resource`:

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

Mostra i dettagli di una istanza della risorsa

```
bluemix resource instance NOME [-r, --region REGIONE] [--id]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome dell'istanza della risorsa</dd>
  <dt>-r, --region</dt>
  <dd>Filtra in base all'ID regione; se non viene specificato, il valore predefinito è la regione corrente; '-r, --region all' per visualizzare le istanze della risorsa in tutte le regioni</dd>
  <dt>--id</dt>
  <dd>Visualizza l'ID dell'istanza della risorsa</dd>
</dl>

<strong>Esempi</strong>:
mostra i dettagli dell'istanza della risorsa `my-resource-instance`:

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

Crea un'istanza della risorsa

```
bluemix resource instance-create NOME NOME_RISORSA|ID_RISORSA NOME_PIANO_RISORSE|ID_PIANO_RISORSE [-r, --region REGIONE] [-t, --tags TAG] [-p, --parameters @FILE_JSON | STRINGA_JSON ]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME (obbligatorio)</dt>
  <dd>Nome dell'istanza della risorsa</dd>
  <dt>NOME_RISORSA o ID_RISORSA (obbligatorio)</dt>
  <dd>Nome o ID della risorsa</dd>
  <dt>NOME_PIANO_RISORSE o ID_PIANO_RISORSE (obbligatorio)</dt>
  <dd>Nome o ID del piano risorse</dd>
  <dt>-r, --region</dt>
  <dd>Regione per creare l'istanza della risorsa; se non viene specificato, viene utilizzata per impostazione predefinita la regione corrente</dd>
  <dt>-t, --tags</dt>
  <dd>Tag</dd>
  <dt>-p, --parameters</dt>
  <dd>File JSON o stringa JSON di parametri per creare l'istanza della risorsa</dd>
</dl>

<strong>Esempi</strong>:
crea una istanza della risorsa denominata `my-resource-instance` utilizzando il piano risorse `test-resource-plan` della risorsa `test-resource`:

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

Aggiorna l'istanza della risorsa

```
bluemix resource instance-update NOME_ISTANZA_RISORSA [-n, --name NUOVO_NOME] [-t, --tags TAG] [--resource-plan-id ID_PIANO_RISORSE] [--update-time TEMPO_AGGIORNAMENTO] [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ISTANZA_RISORSA (obbligatorio)</dt>
  <dd>Nome dell'istanza della risorsa</dd>
  <dt>-n, --name</dt>
  <dd>Nuovo nome dell'istanza della risorsa</dd>
  <dt>-t, --tags</dt>
  <dd>Nuove tag</dd>
  <dt>--resource-plan-id</dt>
  <dd>Nuovo ID del piano delle risorse</dd>
  <dt>--update-time</dt>
  <dd>Tempo in secondi da quando il record caricabile dovrebbe diventare effettivo</dd>
  <dt>-f, --force</dt>
  <dd>Forza l'aggiornamento senza conferma</dd>
</dl>

<strong>Esempi</strong>:
aggiorna l'istanza della risorsa `my-resource-instance`, modificane il nome in `new-resource-instance`:

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

Elimina l'istanza della risorsa

```
bluemix resource instance-delete NOME [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Forza l'eliminazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
elimina l'istanza della risorsa `my-resource-instance`:

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

Mostra le associazioni all'alias della risorsa

```
bluemix resource bindings ALIAS_RISORSA
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>ALIAS_RISORSA (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
</dl>

<strong>Esempi</strong>:
mostra le associazioni risorsa all'alias della risorsa `my-resource-alias`:

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

Mostra i dettagli di un'associazione risorsa

```
bluemix resource binding NOME_ALIAS NOME_APPLICAZIONE [--id]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>NOME_APPLICAZIONE</dt>
  <dd>Nome applicazione CloudFoundry</dd>
  <dt>--id</dt>
  <dd>Visualizza solo l'ID. Tutto l'altro output per l'associazione risorsa viene eliminato.</dd>
</dl>

<strong>Esempi</strong>:
mostra i dettagli dell'associazione risorsa tra l'alias della risorsa `my-resource-alias` e l'applicazione `my-app`:

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

Crea un'associazione risorsa

```
bluemix resource binding-create NOME_ALIAS_RISORSA NOME_APPLICAZIONE NOME_RUOLO [--service-id-name NOME_ID_SERVIZIO [-f, --force]]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS_RISORSA (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>NOME_APPLICAZIONE</dt>
  <dd>Nome applicazione CloudFoundry</dd>
  <dt>NOME_RUOLO</dt>
  <dd>Nome del ruolo utente</dd>
  <dt>--service-id-name</dt>
  <dd>Nome dell'ID servizio a cui appartiene il ruolo</dd>
  <dt>-f, --force</dt>
  <dd>Forza la creazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
crea un'associazione risorsa tra l'alias risorsa `my-resource-alias` e l'applicazione `my-app` con il ruolo `Administrator`:

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

Elimina un'associazione risorsa

```
bluemix resource binding-delete ALIAS_RISORSA NOME_APPLICAZIONE [-f, --force]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS_RISORSA (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>NOME_APPLICAZIONE</dt>
  <dd>Nome applicazione CloudFoundry</dd>
  <dt>-f, --force</dt>
  <dd>Forza l'eliminazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
elimina l'associazione risorsa tra l'alias della risorsa `my-resource-alias` e l'applicazione `my-app`:

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

Elenca le chiavi risorsa dell'istanza della risorsa o dell'alias della risorsa

```
bluemix resource keys [ --instance-id ID | --instance-name NOME | --alias-id ID | --alias-name NOME ]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID dell'istanza della risorsa</dd>
  <dt>--instance-name</dt>
  <dd>Nome dell'istanza della risorsa</dd>
  <dt>--alias-id</dt>
  <dd>ID dell'alias della risorsa</dd>
  <dt>--alias-name</dt>
  <dd>Nome alias della risorsa</dd>
</dl>

<strong>Esempi</strong>:
elenca le chiavi risorsa dell'istanza della risorsa `my-resource-instance`:

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

Mostra i dettagli di una chiave risorsa

```
bluemix resource key NOME_CHIAVE [--id]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_CHIAVE</dt>
  <dd>Nome della chiave</dd>
  <dt>--id</dt>
  <dd>Visualizza l'ID della chiave risorsa</dd>
</dl>

<strong>Esempi</strong>:
mostra i dettagli della chiave risorsa `my-resource-key`:

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

Crea una chiave risorsa

```
bluemix resource key-create NOME NOME_RUOLO ( --instance-id ID_ISTANZA_RISORSA | --instance-name NOME_ISTANZA_RISORSA | --alias-id ID_ALIAS_RISORSA | --alias-name NOME_ALIAS_RISORSA ) [--service-id-name NOME_ID_SERVIZIO [-f, --force]]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME</dt>
  <dd>Nome della chiave</dd>
  <dt>NOME_RUOLO</dt>
  <dd>Nome del ruolo utente</dd>
  <dt>--instance-id</dt>
  <dd>ID dell'istanza della risorsa</dd>
  <dt>--instance-name</dt>
  <dd>Nome dell'istanza della risorsa</dd>
  <dt>--alias-id</dt>
  <dd>ID dell'alias della risorsa</dd>
  <dt>--alias-name</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>-service-id-name</dt>
  <dd>Nome dell'ID servizio a cui appartiene il ruolo</dd>
  <dt>-f, --force</dt>
  <dd>Forza la creazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
crea una chiave risorsa denominata `my-resource-key` con il ruolo `Administrator` per l'istanza della risorsa `my-resource-instance`:

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

Elimina una chiave risorsa

```
bluemix resource key-delete NOME_CHIAVE [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_CHIAVE</dt>
  <dd>Nome della chiave</dd>
  <dt>-f, --force</dt>
  <dd>Forza l'eliminazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
elimina la chiave risorsa `my-resource-key`:

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

Elenca gli alias per una istanza della risorsa

```
bluemix resource aliases [ --instance-id ID | --instance-name NOME ]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID dell'istanza della risorsa di appartenenza.</dd>
  <dt>--instance-name</dt>
  <dd>Nome dell'istanza della risorsa di appartenenza.</dd>
</dl>

<strong>Esempi</strong>:
elenca gli alias della risorsa per l'istanza della risorsa `my-resource-instance`:
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

Mostra i dettagli di un alias della risorsa

```
bluemix resource alias NOME_ALIAS [--id]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>--id</dt>
  <dd>Visualizza solo l'ID dell'alias della risorsa fornito. Tutto l'altro output per l'alias viene eliminato.</dd>
</dl>

<strong>Esempi</strong>:
mostra i dettagli dell'alias della risorsa `my-resource-alias`:
```
bluemix resource alias my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

Crea un alias di una istanza della risorsa

```
bluemix resource alias-create NOME_ALIAS ( --instance-id ID | --instance-name NOME ) [-s NOME_SPAZIO] [-t, --tags TAG] [-p, --parameters @FILE_JSON | TESTO_JSON]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>--instance-id</dt>
  <dd>ID dell'istanza della risorsa di appartenenza.</dd>
  <dt>--instance-name</dt>
  <dd>Nome dell'istanza della risorsa di appartenenza.</dd>
  <dt>-s</dt>
  <dd>Nome dello spazio in cui l'alias viene creato. Il valore predefinito è lo spazio corrente.</dd>
  <dt>-t, --tags</dt>
  <dd>Elenco delle tag.</dd>
  <dt>-p, --parameters</dt>
  <dd>File JSON o stringa JSON dei parametri.</dd>
</dl>

<strong>Esempi</strong>:
crea un alias della risorsa denominato `my-resource-alias` dell'istanza della risorsa `my-resource-instance`:
```
bluemix resource alias-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

Aggiorna un alias della risorsa

```
bluemix resource alias-update NOME_ALIAS [-n, --name NUOVO_NOME] [-t, --tags TAG] [-p, --parameters @FILE_JSON | STRINGA_JSON ][-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>-n, --name</dt>
  <dd>Nuovo nome dell'alias della risorsa.</dd>
  <dt>-t, --tags</dt>
  <dd>Elenco delle tag.</dd>
  <dt>-p, --parameters</dt>
  <dd>File JSON o stringa JSON dei parametri.</dd>
  <dt>-f, --force</dt>
  <dd>Forza l'aggiornamento senza conferma dell'utente.</dd>
</dl>

<strong>Esempi</strong>:
aggiorna l'alias della risorsa `my-resource-alias`, modificane il nome in `new-resource-alias`:

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

Elimina un alias della risorsa

```
bluemix resource alias-delete NOME_ALIAS [-f, --force]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>NOME_ALIAS (obbligatorio)</dt>
  <dd>Nome alias della risorsa</dd>
  <dt>-f, --force</dt>
  <dd>Forza l'eliminazione senza conferma</dd>
</dl>

<strong>Esempi</strong>:
elimina l'alias della risorsa `my-resource-alias`:

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

Cerca voci del catalogo

```
bluemix catalog search [-q, --query PAROLE_CHIAVE] [-r, --region REGIONE] [-k, --kind TIPO] [-p, --price PREZZO] [-t, --tag TAG] [--sort-by PROPRIETÀ] [--reverse] [--json] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-q, --query</dt>
  <dd>Cerca la parola chiave</dd>
  <dt>-r, --region</dt>
  <dd>Specifica la regione geografica in cui cercare. Attualmente sono supportate solo "us-south" e "united-kingdom"</dd>
  <dt>-k, --kind</dt>
  <dd>Filtra in base al tipo di risorse. Attualmente sono supportati solo "service-cf", "iaas", "runtime", "template" e "dashboard"</dd>
  <dt>-p, --price</dt>
  <dd>Filtra in base al prezzo. Attualmente sono supportati solo "free", "paygo" e "bluemix-subscription"</dd>
  <dt>-t, --tag</dt>
  <dd>Filtra in base alla tag.</dd>
  <dt>-sort-by</dt>
  <dd>Proprietà in base a cui ordinare</dd>
  <dt>-reverse</dt>
  <dd>Indica se invertire la sequenza di ordinamento</dd>
  <dt>-json</dt>
  <dd>Genera in output la risposta JSON originale</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Cerca il servizio `Automation test`:

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

Ottiene una voce di catalogo

```
bluemix catalog entry [-i ID] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>L'ID della voce di catalogo.</dd>
  <dt>-children</dt>
  <dd>Ottieni tutti gli elementi secondari per la voce di catalogo</dd>
  <dt>-json</dt>
  <dd>Genera in output la risposta JSON originale</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Ottieni la voce con ID `a0ef1-d3b4j0`:

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
Crea una nuova voce di catalogo (solo amministratore catalogo di un account)

```
bluemix catalog entry-create [-c PARAMETERI_COME_JSON] [-p, --parent ELEMENTO_PRINCIPALE] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-p, --parent</dt>
  <dd>ID elemento principale dell'oggetto</dd>
  <dt>-c</dt>
  <dd>Oggetto JSON valido che contiene i parametri di configurazione specifici per il catalogo, fornito incorporato o in un file. Per un elenco dei parametri di configurazione supportati, consulta la documentazione per la specifica voce di catalogo.</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Crea risorsa dal file JSON con l'ID di elemento principale `a0ef1-d3b4j0`:

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
Aggiorna una voce di catalogo esistente (solo editor o amministratore di catalogo di un account)

```
bluemix catalog entry-update [-i ID] [-c PARAMETRI_COME_JSON] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>L'ID della voce di catalogo in fase di aggiornamento.</dd>
  <dt>-c</dt>
  <dd>Oggetto JSON valido che contiene i parametri di configurazione specifici per il catalogo, fornito incorporato o in un file. Per un elenco dei parametri di configurazione supportati, consulta la documentazione per la specifica voce di catalogo.</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Aggiorna la risorsa `j402-dnf1i` dal file JSON:

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
Ottieni la visibilità per una voce di catalogo (solo amministratore di catalogo di un account)

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>L'ID della voce di catalogo.</dd>
  <dt>-json</dt>
  <dd>Genera in output la risposta JSON originale</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Ottiene la visibilità della risorsa `j402-dnf1i` in ambito globale:

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
Aggiorna la visibilità di una voce di catalogo esistente (solo amministratore di catalogo di un account)

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETRI_COME_JSON] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>L'ID della voce di catalogo in fase di aggiornamento.</dd>
  <dt>-c</dt>
  <dd>Oggetto JSON valido che contiene i parametri di configurazione specifici per il catalogo, fornito incorporato o in un file. Per un elenco dei parametri di configurazione supportati, consulta la documentazione per la specifica voce di catalogo.</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Imposta la visibilità della risorsa `j402-dnf1i` dal file JSON:

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
Elenca le offerte di servizio nel marketplace

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
<dl>
  <dt>-cf</dt>
  <dd>Mostra solo i servizi Cloud Foundry</dd>
  <dt>-rc</dt>
  <dd>Mostra solo i servizi compatibili con RC</dd>
  <dt>-global</dt>
  <dd>Opera in ambito globale</dd>
</dl>

<strong>Esempi</strong>:

Mostra le offerte del servizio in ambito globale:

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

Visualizza i modelli di contenitore tipo su Bluemix.

```
bluemix catalog templates [-d]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

   <dl>
   <dt>-d (facoltativo)</dt>
   <dd>Se viene specificata l'opzione <i>-d</i>, viene visualizzata anche la descrizione di ciascun modello. Altrimenti, vengono visualizzati solo l'ID e il nome di ciascun modello.</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

Visualizza le informazioni dettagliate di un modello contenitore tipo specificato.

```
bluemix catalog template ID_MODELLO
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:
   <dl>
   <dt>ID_MODELLO (obbligatorio)</dt>
   <dd>L'ID del modello contenitore tipo. Utilizza <i>bluemix template</i> per visualizzare l'ID di tutti i modelli.</dd>
   </dl>


<strong>Esempi</strong>:

Visualizza i dettagli del modello `mobileBackendStarter`:

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

Crea un'applicazione cf basata sul modello specificato con l'URL e la descrizione specificati. Per impostazione predefinita, la nuova applicazione viene avviata automaticamente.

```
bluemix catalog template-run ID_MODELLO NOME_APPLICAZIONE_CF [-u URL] [-d DESCRIZIONE] [--no-start]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso, Destinazione

<strong>Opzioni comando</strong>:
   <dl>
   <dt>ID_MODELLO (obbligatorio)</dt>
   <dd>Il modello su cui verrà basata l'applicazione quando verrà creata. Utilizza <i>bluemix templates</i> per visualizzare l'ID di tutti i modelli.</dd>
   <dt>NOME_APPLICAZIONE_CF (obbligatorio)</dt>
   <dd>Il nome dell'applicazione cf da creare.</dd>
   <dt>-u <i>URL</i> (facoltativo)</dt>
   <dd>La rotta dell'applicazione. Se non specificata, la rotta viene impostata automaticamente da Bluemix, in base al tuo nome applicazione e al tuo dominio predefinito.</dd>
   <dt>-d <i>DESCRIZIONE</i> (facoltativo)</dt>
   <dd>Descrizione dell'applicazione.</dd>
   <dt>--no-start (facoltativo)</dt>
   <dd>Non avviare l'applicazione automaticamente una volta creata. Se non viene specificata, l'applicazione viene avviata automaticamente dopo la sua creazione.</dd>
   </dl>


<strong>Esempi</strong>:

Crea un'applicazione `my-app` basata sul modello `javaHelloWorld`:

```
bluemix catalog template-run javaHelloWorld my-app
```

Crea un'applicazione `my-ruby-app` basata sul modello `rubyHelloWorld` con la rotta `myrubyapp.chinabluemix.net` e la descrizione `La mia prima applicazione ruby su {{site.data.keyword.Bluemix_notm}}.`:

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "La mia prima applicazione ruby su {{site.data.keyword.Bluemix_notm}}."
```

Crea un'applicazione `my-python-app` basata sul modello `pythonHelloWorld` senza l'avvio automatico:

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

Mostra i costi e l'utilizzo mensile del tuo account.

```
bluemix billing account-usage [-d AAAA-MM] [--json]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

<dl>
  <dt>-d DATA_MESE (facoltativo)</dt>
  <dd>Visualizza i dati per il mese e la data specificando l'utilizzo nel formato AAAA-MM. Se non specificato, viene mostrato l'utilizzo del mese corrente.</dd>
  <dt>--json (facoltativo)</dt>
  <dd>Visualizza il risultato di utilizzo nel formato JSON.</dd>
</dl>

<strong>Esempi</strong>:

Mostra il report del costo e l'utilizzo dell'account per 2016-06:

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

Mostra i dettagli dell'utilizzo mensile di un'organizzazione. Questa operazione può essere eseguita solo da un gestore della fatturazione dell'organizzazione.

```
bluemix billing org-usage NOME_ORGANIZZAZIONE [-d AAAA-MM] [-r NOME_REGIONE] [--json]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

<dl>
  <dt>NOME_ORGANIZZAZIONE (obbligatorio)</dt>
  <dd>Nome dell'organizzazione.</dd>
  <dt>-d DATA_MESE (facoltativo)</dt>
  <dd>Visualizza i dati per il mese e la data specificata tramite l'utilizzo nel formato AAAA-MM. Se non specificato, viene mostrato l'utilizzo del mese corrente.</dd>
  <dt>-r NOME_REGIONE</dt>
  <dd>Nome della regione che ospita l'organizzazione. Se impostato su 'all', viene mostrato l'utilizzo dell'organizzazione in tutte le regioni.</dd>
  <dt>--json (facoltativo)</dt>
  <dd>Visualizza il risultato di utilizzo nel formato JSON.</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

Mostra il riepilogo dell'utilizzo mensile per le organizzazioni nel mio account.

```
bluemix billing orgs-usage-summary [-d AAAA-MM] [-r NOME_REGIONE] [--json]
```

<strong>Prerequisiti</strong>:  Endpoint, Accesso

<strong>Opzioni comando</strong>:

<dl>
  <dt>-d DATA_MESE (facoltativo)</dt>
  <dd>Visualizza i dati per il mese e la data specificata tramite l'utilizzo nel formato AAAA-MM. Se non specificato, viene mostrato l'utilizzo del mese corrente.</dd>
  <dt>-r NOME_REGIONE</dt>
  <dd>Nome della regione che ospita le organizzazioni. Se impostato su 'all', viene mostrato il riepilogo dell'utilizzo delle organizzazioni in tutte le regioni.</dd>
  <dt>--json (facoltativo)</dt>
  <dd>Visualizza il risultato di utilizzo nel formato JSON.</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

Elenca i repository di plugin registrati nella CLI {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repos
```

<strong>Prerequisiti</strong>:  Nessuno


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

Aggiunge un nuovo repository di plugin alla CLI {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-add NOME_REPOSITORY URL_REPOSITORY
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_REPOSITORY (obbligatorio)</dt>
   <dd>Il nome del repository da aggiungere. Puoi definire un tuo nome per ciascun repository.</dd>
   <dt>URL_REPOSITORY (obbligatorio)</dt>
   <dd>L'URL del repository da aggiungere. L'URL del repository deve contenere il protocollo (ad esempio, http://plugins.ng.bluemix.net invece di plugins.ng.bluemix.net). http://plugins.ng.bluemix.net è il repository di plugin ufficiale della CLI Bluemix.</dd>
    </dl>


<strong>Esempi</strong>:

Aggiunge il repository di plug-in ufficiale della CLI Bluemix come `bluemix-repo`:

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

Rimuove un repository di plugin dalla CLI {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin repo-remove NOME_REPOSITORY
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
   <dl>
   <dt>NOME_REPOSITORY (obbligatorio)</dt>
   <dd>Il nome del repository da rimuovere.</dd>
   </dl>

<strong>Esempi</strong>:

Rimuove il repository `bluemix-repo` dalla CLI {{site.data.keyword.Bluemix_notm}}:

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

Elenca tutti i plug-in disponibili in tutti i repository aggiunti o in uno specifico repository.

```
bluemix plugin repo-plugins [-r NOME_REPOSITORY]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>-r <i>NOME_REPOSITORY</i> (facoltativo)</dt>
   <dd>Elenca solo i plug-in del repository specificato.</dd>
   </dl>

<strong>Esempi</strong>:

Elenca tutti i plug-in in tutti i repository aggiunti:

```
bluemix plugin repo-plugins
```

Elenca tutti i plug-in nel repository `bluemix-repo`:

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

Mostra i dettagli di un plug-in nel repository.

```
bluemix plugin repo-plugin NOME_PLUGIN [-r NOME_REPOSITORY]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>-r <i>NOME_REPOSITORY</i> (facoltativo)</dt>
   <dd>Il nome del repository. Se non viene specificato alcun repository, il comando utilizza il repository di plug-in predefinito.</dd>
   </dl>

<strong>Esempi</strong>:

Elenca i dettagli del plug-in "IBM-Containers" nel repository "sample-repo":

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

Elenca i dettagli del plug-in "IBM-Containers" nel repository predefinito.

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

Elenca tutti i plug-in installati nella CLI {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin list
```

<strong>Prerequisiti</strong>:  Nessuno

## bluemix plugin show
{: #bluemix_plugin_show}

Visualizza i dettagli di un plugin installato

```
bluemix plugin show NOME-PLUGIN
```

<strong>Prerequisiti</strong>:  Nessuno


## bluemix plugin install
{: #bluemix_plugin_install}

Installa la versione specifica del plugin nella CLI {{site.data.keyword.Bluemix_notm}} dal percorso o repository specificato.

```
bluemix plugin install PERCORSO_PLUGIN|NOME_PLUGIN [-r NOME_REPOSITORY] [-v VERSIONE]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>PERCORSO_PLUGIN|NOME_PLUGIN (obbligatorio)</dt>
   <dd>Se -r <i>NOME_REPOSITORY</i> non viene specificato, il plugin viene installato dal percorso locale o dall'URL remoto specificati.</dd>
   <dt>-r <i>NOME_REPOSITORY</i> (facoltativo)</dt>
   <dd>Il nome del repository in cui si trova il file binario del plugin. Se non viene specificato alcun repository, il comando utilizza il repository di plug-in predefinito.</dd>
   <dt>-v <i>VERSIONE</i> (facoltativo)</dt>
   <dd>La versione del plugin da installare. Se non fornita, viene installata l'ultima versione del plugin. Questa opzione è valida solo quando si installa il plugin dal repository.</dd>
    </dl>

<strong>Esempi</strong>:

Installa un plugin dal file locale:

```
bluemix plugin install /downloads/new_plugin
```

Installa un plugin dall'URL remoto:

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

Installa il plugin `IBM-Containers` dell'ultima versione dal repository `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
Installa il plugin `IBM-Containers` con la versione `0.5.800` dal repository `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

Aggiorna il plug-in da un repository

```
bluemix plugin update [NOME PLUGIN] [-r NOME_REPOSITORY] [-v VERSIONE] [--all]
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:
<dl>
 <dt>NOME PLUGIN</dt>
 <dd>Nome del plugin da aggiornare. Se non specificato, il comando ricerca gli aggiornamenti per tutti i plug-in installati.</dd>
 <dt>-r NOME_REPOSITORY</dt>
 <dd>Il nome del repository in cui si trova il file binario del plugin. Se non specificato, il comando utilizza il repository di plugin predefinito.</dd>
 <dt>-v <i>VERSIONE</i> (facoltativo)</dt>
 <dd>La versione a cui aggiornare il plugin. Se non viene fornita, aggiorna il plugin all'ultima versione disponibile.</dd>
 <dt>--all</dt>
 <dd>Aggiorna tutti i plug-in disponibili.</dd>
</dl>

<strong>Esempi</strong>:

controlla tutti gli aggiornamenti disponibili nel repository di plugin "My-Repo":

```
bluemix plugin update -r My-Repo
```

Aggiorna il plugin "plugin-echo" nel repository "My-Repo" all'ultima versione:

```
bluemix plugin update -r My-Repo plugin-echo
```

Aggiorna il plugin "plugin-echo" nel repository "My-Repo" alla versione "1.0.1":

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

Disinstalla il plugin specificato dalla CLI {{site.data.keyword.Bluemix_notm}}.

```
bluemix plugin uninstall NOME_PLUGIN
```

<strong>Prerequisiti</strong>:  Nessuno

<strong>Opzioni comando</strong>:

   <dl>
   <dt>NOME_PLUGIN (obbligatorio)</dt>
   <dd>Il nome del plugin da disinstallare.</dd>
    </dl>

<strong>Esempi</strong>:

Disinstalla il plugin `IBM-Containers` che era stato precedentemente installato:

```
bluemix plugin uninstall IBM-Containers
```

