---



copyright:

  years: 2015, 2017
lastupdated: "2017-10-06"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Mandatos {{site.data.keyword.Bluemix_notm}} (bx)
{: #bluemix_cli}

Versión: 0.6.1

La interfaz de línea de mandatos (CLI) de {{site.data.keyword.Bluemix_notm}} proporciona un conjunto de mandatos que se agrupan por espacio de nombres para que los usuarios interactúen con {{site.data.keyword.Bluemix_notm}}. 

A partir de la versión 0.5.0, el cliente de línea de mandatos de {{site.data.keyword.Bluemix_notm}} empaqueta un cliente de línea de mandatos de Cloud Foundry en su instalación. Si tiene su propio cf cli instalado, no utilice los mandatos CLI de {{site.data.keyword.Bluemix_notm}} `bx [mandato]` ni los mandatos Cloud Foundry CLI `cf [mandato]` de su propia instalación en el mismo contexto. En su lugar, utilice `bluemix cf [mandato]` si desea utilizar cf cli para gestionar los recursos de Cloud Foundry en el contexto de CLI de {{site.data.keyword.Bluemix_notm}}.  Es más, no se permite `bluemix cf api/login/logout/target`, en su lugar, utilice `bluemix api/login/logout/target`.

A continuación se enumera el uso de los mandatos detallados que están soportados por la CLI de {{site.data.keyword.Bluemix_notm}}, incluidos sus nombres, argumentos, opciones, requisitos previos, descripciones y ejemplos.
{:shortdesc}

**Nota:** *Requisitos previos* lista las acciones que son necesarias antes de utilizar el mandato. Los mandatos que no tienen acciones de requisito previo listan **Ninguno**. De lo contrario, los requisitos previos pueden incluir una o varias de las acciones siguientes:

<dl>
<dt>Punto final</dt>
<dd>Un punto final de API se debe establecer por medio de la <code>bluemix api</code> antes de utilizar el mandato.</dd>
<dt>Login</dt>
<dd>El inicio de sesión que utiliza el mandato <code>bluemix login</code> es necesario antes de utilizar este mandato.
Si inicia sesión con un ID federado, utilice la opción '--sso' para autenticarse con un código de acceso de una sola vez o utilice '--apikey' para realizar la autenticación con una clave de API. Vaya a la consola de {{site.data.keyword.Bluemix_notm}} **Gestionar** &gt; **Seguridad** &gt; **Claves de API de Bluemix ** para crear claves de API.
</dd>
<dt>Target</dt>
<dd>El mandato <code>bluemix target</code> debe utilizarse para establecer un punto de extensión org y un espacio antes de utilizar este mandato.</dd>
<dt>Docker</dt>
<dd>La CLI de Docker CLI (docker) debe estar instalada para poder ejecutar este mandato.</dd>
</dl>

**Nota:** puede utilizar el formato abreviado de los mandatos de bluemix; por ejemplo, `bx api` es la abreviatura de `bluemix api`.

Utilice los índices de las tablas siguientes para consultar los mandatos de Bluemix que se utilizan con mayor frecuencia.

## Mandatos generales bluemix 
{: #bx_commands_index}

<table summary="Mandatos generales bluemix">
<caption>Tabla 1. Mandatos generales de bluemix</caption>
 <thead>
 <th colspan="5">Mandatos generales bluemix</th>
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
 
 ## Mandatos para gestionar servicios {{site.data.keyword.BluSoftlayer_notm}}
  {: #bx_commands_softlayer}
  
Los mandatos para gestionar {{site.data.keyword.BluSoftlayer_notm}}} se han fusionado en la CLI de Bluemix. Para obtener más información sobre la utilización de la CLI de Bluemix CLI configurar y gestionar servicios {{site.data.keyword.BluSoftlayer_notm}}, consulte: mandatos de bluemix de la [CLI de Bluemix {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl)](/docs/cli/reference/softlayer/index.md#softlayer_cli).
 
 ## Mandatos para gestionar cuentas, organizaciones y roles
 {: #bx_commands_account}

<table summary="Mandatos de Bluemix que puede utilizar para gestionar las cuentas, las organizaciones, los espacios y los roles.">
<caption>Tabla 2. Mandatos para gestionar cuentas, organizaciones, espacios y roles</caption>
 <thead>
 <th colspan="5">Mandatos para gestionar cuentas, organizaciones, espacios y roles</th>
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


 ## Mandatos para gestionar grupos de recursos y recursos
{: #bx_commands_resource}

<table summary="Mandato de Bluemix que puede utilizar para gestionar grupos de recursos y recursos.">
  <caption>Tabla 3. Mandatos para gestionar grupos de recursos y recursos</caption>
  <thead>
    <th colspan="5">Mandatos para gestionar grupos de recursos y recursos</th>
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

 
 ## Mandatos para gestionar claves de API y políticas
 {: #bx_commands_iam}
 <table summary="Mandatos de Bluemix que puede utilizar para gestionar claves de API y políticas.">
 <caption>Tabla 3. Mandatos para gestionar claves de API y políticas</caption>
  <thead>
  <th colspan="5">Mandatos para gestionar claves de API y políticas</th>
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
 
 ## Mandatos para gestionar apps cf y dominios, rutas y certificados relacionados con las apps
 {: #bx_commands_apps}

<table summary="mandatos de bluemix que sirven para gestionar apps cf y dominios, rutas y certificados relacionados con las apps.">
<caption>Tabla 4. Mandatos para gestionar apps cf y dominios, rutas y certificados relacionados con las apps</caption>
 <thead>
 <th colspan="5">Mandatos para gestionar apps cf y dominios, rutas y certificados relacionados con las apps</th>
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
 
 ## Mandatos para gestionar servicios Bluemix
 {: #bx_commands_services}

<table summary="Mandatos bluemix que se pueden utilizar para gestionar servicios Bluemix.">
<caption>Tabla 5. Mandatos para gestionar servicios Bluemix</caption>
 <thead>
 <th colspan="5">Mandatos para gestionar servicios Bluemix</th>
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

 
 ## Mandatos para gestionar los valores de catálogo, plug-ins y facturación
 {: #bx_commands_settings}

<table summary="Mandatos bluemix que puede utilizar para gestionar los valores de catálogo, plug-ins, facturación y seguridad de Bluemix.">
<caption>Tabla 6. Mandatos para gestionar los valores de catálogo, plug-ins, facturación y seguridad de Bluemix</caption>
 <thead>
 <th colspan="5">Mandatos para gestionar los valores de catálogo, plug-ins, facturación y seguridad de Bluemix</th>
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
Muestra la ayuda general para mandatos incorporados de primer nivel y espacios de nombres soportados de {{site.data.keyword.Bluemix_notm}} CLI, o la ayuda para un mandato o un espacio de nombres incorporado específico.

```
bluemix help [COMMAND|NAMESPACE]
```

<strong>Requisitos previos</strong>: Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>COMMAND|NAMESPACE (opcional)</dt>
   <dd>Mandato o espacio de nombres para el que se visualiza ayuda. Si no se especifica, se mostrará la ayuda general para {{site.data.keyword.Bluemix_notm}} CLI.</dd>
   </dl>



<strong>Ejemplos</strong>:

Visualiza ayuda general para {{site.data.keyword.Bluemix_notm}} CLI:

```
bluemix help
```

Muestra ayuda para el mandato `info`:

```
bluemix help info
```



## bluemix api
{: #bluemix_api}
Establezca o visualice el punto final de su API de {{site.data.keyword.Bluemix_notm}}.

```
bluemix api [API_ENDPOINT] [--unset] [--skip-ssl-validation]
```

<strong>Requisitos previos</strong>: Ninguno

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>API_ENDPOINT (opcional)</dt>
   <dd>Punto final de API de destino, por ejemplo, `https://api.chinabluemix.net`. Si no se especifican ambas opciones *API_ENDPOINT* y `--unset`, se mostrará el punto final de API actual.</dd>
   <dt>--unset (opcional)</dt>
   <dd>Elimina la configuración del punto final de la API.</dd>
   <dt>--skip-ssl-validation (opcional)</dt>
   <dd>Omite la validación SSL de solicitudes HTTP.</dd>
   </dl>
<strong>Ejemplos</strong>:

Establecer el punto final de la API en api.chinabluemix.net:

```
bluemix api api.chinabluemix.net
```

```
bluemix api https://api.chinabluemix.net --skip-ssl-validation
```

Visualice el punto final de la API actual:

```
bluemix api
```

Desestablecer el punto final de la API:

```
bluemix api --unset
```

## bluemix config
{: #bluemix_config}


Escriba valores predeterminados en el archivo de configuración.

```
bluemix config --http-timeout TIEMPO_ESPERA_EN_SEGUNDOS | --trace (true|false|vía-acceso-archivo) | --color (true|false) | --locale (LOCALE|CLEAR) | --check-version (true|false)
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>--http-timeout <i>TIEMPO_ESPERA_EN_SEGUNDOS</i></dt>
   <dd>Valor de tiempo de espera para solicitudes HTTP. El valor predeterminado es de 60 segundos.</dd>
   <dt>--trace true|false|<i>path-to-file</i></dt>
   <dd>Rastrear solicitudes HTTP al terminal o archivo especificado.</dd>
   <dt>--color true|false</dt>
   <dd>Habilitar o inhabilitar la salida de color. La salida de color está habilitada de forma predeterminada.</dd>
   <dt>--locale <i>LOCALE|CLEAR</i></dt>
   <dd>Establecer un entorno local predeterminado. Si LOCALE es <i>CLEAR</i>, el entorno local anterior se elimina.</dd>
   <dt>--check-version true|false</dt>
   <dd>Habilitar o inhabilitar la comprobación de la versión de la CLI.</dd>
   </dl>

Sólo se puede especificar una de estas opciones a la vez.

<strong>Ejemplos</strong>:

Establezca el tiempo de espera de solicitud HTTP en 30 segundos:

```
bluemix config --http-timeout 30
```

Habilitar la salida de rastreo para las solicitudes HTTP:

```
bluemix config --trace true
```

Rastrear solicitudes HTTP a un archivo determinado */home/usera/my_trace*:

```
bluemix config --trace /home/usera/my_trace
```

Inhabilitar la salida de color:

```
bluemix config --color false
```

Establecer el entorno local en zh_Hans:

```
bluemix config --locale zh_Hans
```

Borrar los valores de entorno local:

```
bluemix config --locale CLEAR
```



## bluemix info
{: #bluemix_info}

Vea la información básica de {{site.data.keyword.Bluemix_notm}}, incluida la región actual, la versión del controlador de nube y algunos puntos finales útiles, como por ejemplo los puntos finales para el inicio de sesión y el intercambio de señales de acceso.

```
bluemix info
```

<strong>Requisitos previos</strong>:  Punto final


## bluemix cf
{: #bluemix_cf}

Invocar CLI CF incluido

```
bluemix [-q, --quiet] cf COMMAND...
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-q, --quiet</dt>
  <dd>Desactivar el mensaje "Invocando el mandato cf..."</dd>
</dl>

<strong>Ejemplos</strong>:

Listar apps cf:

```
bluemix cf apps
```

Listar servicios cf sin el mensaje "Invocando el mandato cf...":

```
bluemix -q cf services
```


## bluemix login
{: #bluemix_login}

Inicio de sesión de usuario. 

```
bluemix login [-a API_ENDPOINT] [--sso] [-u USERNAME] [-p PASSWORD] [--apikey KEY | @KEY_FILE] [-c ACCOUNT_ID] [-o ORG] [-s SPACE]
```

<strong>Requisitos previos</strong>:  Ninguno

<!-- staging comment for Atlas 45: might need prereq for federated ID/SSO option unless we expect them to just view the details from the cf login command -->

<strong>Opciones de mandato</strong>:
<dl>
  <dt> -a <i>API_ENDPOINT</i> (opcional)</dt>
  <dd> Punto final de la API (por ejemplo: api.ng.bluemix.net)</dd>
  <dt> --apikey <i>API_KEY o @API_KEY_FILE_PATH</i>
  <dd> Contenido de clave de API o la vía de acceso a un archivo de clave de API indicado mediante @</dd>
  <dt> --sso (opcional) </dt>
  <dd> Utilizar un código de acceso de un solo uso para iniciar sesión </dd>
  <dt> -u <i>USERNAME</i> (opcional)</dt>
  <dd> Nombre de usuario</dd>
  <dt> -p <i>PASSWORD</i> (opcional)</dt>
  <dd> Contraseña</dd>
  <dt> -c <i>ACCOUNT_ID</i> (opcional) </dt>
  <dd> ID de la cuenta de destino</dd>
  <dt> -o <i>ORG_NAME</i> (opcional) </dt>
  <dd> Nombre de la organización de destino </dd>
  <dt> -s <i>SPACE_NAME</i> (opcional) </dt>
  <dd> Nombre del espacio de destino</dd>
  <dt> --skip-ssl-validation (opcional) </dt>
  <dd> Omite la validación SSL de solicitudes HTTP. No se recomienda esta opción.</dd>
</dl>

<strong>Ejemplos</strong>:

#### Inicio de sesión interactivo

```
bluemix login
```

Iniciar sesión con un nombre de usuario y su contraseña, estableciendo un espacio, una organización y una cuenta de destino:

```
bluemix login -u username -p password -c MyAccountID -o MyOrg -s MySpace
```

Iniciar sesión con un código de acceso de una sola vez, estableciendo una cuenta, una organización y un espacio de destino

```
bluemix login --sso -c MyAccountID -o MyOrg -s MySpace
```

Iniciar sesión con una clave de API y estableciendo destinos:

#### La clave de API tiene asociada una cuenta

```
bluemix login --apikey api-key-string -o MyOrg -s MySpace
```

```
bluemix login --apikey @filename -o MyOrg -s MySpace
```

#### La clave de API no tiene asociada una cuenta

```
bluemix login --apikey api-key-string -c MyAccountID -o MyOrg -s MySpace
```

```
bluemix login --apikey @fileName -c MyAccountID -o MyOrg -s MySpace
```

<strong>Nota:</strong> Si la clave de API tiene asociada una cuenta, no se permite conmutar a otra cuenta.

#### Utilizar un código de acceso de una sola

```
bluemix login -u UserID --sso
```

A continuación, la CLI proporcionará un enlace de URL y pedirá el código de acceso:
```
Código de un solo uso (obtenga uno en https://enlace_URL_para_obtener_código_acceso):
```

Abra el enlace en el navegador, que le guiará para obtener el código de acceso. Escriba el código de acceso en la consola y podrá iniciar la sesión.

## bluemix logout
{: #bluemix_logout}

Cerrar sesión de usuario.

```
bluemix logout
```

<strong>Requisitos previos</strong>:  Ninguno

## bluemix regions
{: #bluemix_regions}

Visualiza la información para todas las regiones en {{site.data.keyword.Bluemix_notm}}.

```
bluemix regions
```

<strong>Requisitos previos</strong>:  Punto final


## bluemix target
{: #bluemix_target}


Establece o visualiza la cuenta, región, organización o espacio de destino.

```
bluemix target [-r REGION_NAME] [-c ACCOUNT_ID] [--cf] [-o ORG] [-s SPACE]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>-r <i>REGION_NAME</i> (opcional)</dt>
   <dd>Nombre de la región a la que se conmutará, como por ejemplo 'us-south' o 'eu-gb'.</dd>
   <dt>-c <i>ACCOUNT_ID</i> (opcional)</dt>
   <dd>ID de la cuenta de destino.</dd>
   <dt>--cf</dt>
   <dd>Seleccionar interactivamente la organización y el espacio de destino</dd>
   <dt>-o <i>ORG_NAME</i> (opcional)</dt>
   <dd>Nombre de la organización de destino.</dd>
   <dt>-s <i>SPACE_NAME</i> (opcional)</dt>
   <dd>Nombre del espacio de destino.</dd>
   </dl>
Si no se especifica ninguna opción, se visualiza la cuenta, la región, la organización y el espacio actuales.

<strong>Ejemplos</strong>:

Establecer la cuenta, organización y espacio actuales:

```
bluemix target -c MyAccountID -o MyOrg -s MySpace
```

Cambiar a una nueva región:

```
bluemix target -r eu-gb
```

Visualiza la cuenta, región, organización y espacio actual:

```
bluemix target
```

### bluemix update
{: #bluemix_update}

Actualiza la CLI a la última versión.

```
bluemix update
```

<strong>Requisitos previos</strong>:  Ninguno

### bluemix account orgs
{: #bluemix_account_orgs}

Listar todas las organizaciones

```
bluemix account orgs [-r REGION] [--guid]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>-r <i>REGION</i> (opcional)</dt>
   <dd>Indica para qué región se muestra información sobre la organización. Si se establece en 'all', se listan todas las organizaciones de todas las regiones.</dd>
   <dt>--guid (opcional)</dt>
   <dd>Muestra el GUID de las organizaciones.</dd>
   </dl>

<strong>Ejemplos</strong>:

Listar todas las organizaciones de la región: `us-south` con GUID visualizado

```
bluemix account orgs -r us-south --guid
```

## bluemix account org
{: #bluemix_account_org}

Mostrar la información para la organización especificada.

```
bluemix account org ORG_NAME [--guid]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización.</dd>
   <dt>--guid (opcional)</dt>
   <dd>Muestra el GUID de la organización.</dd>
   </dl>

<strong>Ejemplos</strong>:

Mostrar la información de la organización `IBM` con GUID visualizado

```
bluemix account org IBM --guid
```


## bluemix account org-create
{: #bluemix_account_org_create}

Crear una nueva organización. Esta operación solamente la puede realizar el propietario de cuenta.

```
bluemix account org-create ORG_NAME
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización que se está creando.</dd>
   </dl>

<strong>Ejemplos</strong>:

Cree una organización denominada `IBM`.

```
bluemix account org-create IBM
```

## bluemix account org-replicate
{: #bluemix_account_org_replicate}

Replicar una organización desde la región actual a otra región.

```
bluemix account org-replicate ORG_NAME REGION_NAME
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización existente que se debe replicar.</dd>
   <dt>REGION_NAME (necesario)</dt>
   <dd>Nombre de la región que aloja la organización replicada.</dd>
   </dl>

<strong>Ejemplos</strong>:

Replicar la organización `myorg` en la región `eu-gb`:

```
bluemix account org-replicate myorg eu-gb
```


## bluemix account org-rename
{: #bluemix_account_org_rename}

Cambiar el nombre de una organización. Esta operación solamente la puede llevar a cabo un gestor de la organización.

```
bluemix account org-rename OLD_ORG_NAME NEW_ORG_NAME
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>OLD_ORG_NAME (necesario)</dt>
   <dd>Nombre antiguo de la organización que se debe renombrar.</dd>
   <dt>NEW_ORG_NAME (necesario)</dt>
   <dd>Nombre de la nueva organización.</dd>
   </dl>


## bluemix account spaces
{: #bluemix_account_spaces}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf spaces`.


## bluemix account space
{: #bluemix_account_space}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf space`.


## bluemix account space-create
{: #bluemix_account_space_create}

Este mandato tiene la misma función y las mismas opciones que el mandato que el mandato `cf create-space`.


## bluemix account space-rename
{: #bluemix_account_space_rename}


Este mandato tiene la misma función y las mismas opciones que el mandato que el mandato `cf rename-space`.


## bluemix account space-delete
{: #bluemix_account_space_delete}


Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-space`.

## bluemix account org-users
{: #bluemix_account_org_users}

Visualice usuarios en el archivo de organización según el rol.

```
bluemix account org-users ORG_NAME [-a]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>ORG_NAME (necesario)</dt>
<dd>Nombre de la organización.</dd>
<dt>-a (opcional)</dt>
<dd>Lista todos los usuarios de la organización especificada, no agrupada por rol.</dd>
</dl>

## bluemix account org-user-add
{: #bluemix_account_org_user_add}

Añadir un usuario a la organización (es necesario ser gestor de organización).

```
 bluemix account org-user-add USER_NAME ORG
```

## bluemix account org-user-remove
{: #bluemix_account_org_user_remove}

Eliminar un usuario de la organización (gestor de organización o usuario mismo solamente)

```
   bluemix account org-user-remove USER_NAME ORG [-f, --force]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--force, -f</dt>
<dd>Forzar la eliminación sin confirmación.</dd>
</dl>

## bluemix account org-roles
{: #bluemix_account_org_roles}

Obtiene todos los roles de la organización del usuario actual

```
bluemix account org-roles
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

## bluemix account org-role-set
{: #bluemix_account_org_role_set}

Asignar un rol de organización a un usuario. Esta operación solamente la puede llevar a cabo un gestor de la organización.

```
bluemix account org-role-set USER_NAME ORG_NAME ORG_ROLE
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
  <dl>
   <dt>USER_NAME (necesario)</dt>
   <dd>Nombre del usuario al que se asigna.</dd>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización a la que se asigna a este usuario.</dd>
   <dt>ORG_ROLE (necesario)</dt>
   <dd>Nombre del rol de la organización al que se asigna a este usuario. Por ejemplo:
   <ul>
   <li>OrgManager: este rol puede invitar y gestionar usuarios, seleccionar y cambiar planes y establecer límites de gasto.</li>
   <li>BillingManager: este rol puede crear y gestionar la cuenta de facturación y la información de pago.</li>
   <li>OrgAuditor: este rol tiene acceso de sólo lectura a informes e información de organización.</li>
   </ul>
   </dd>
  </dl>

<strong>Ejemplos</strong>:

Asigne el usuario `Mary` a la organización `IBM` como el rol de `OrgManager`:

```
bluemix account org-role-set Mary IBM OrgManager
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: Establezca roles de espacios/organizaciones utilizando la interfaz de línea de mandatos, sin embargo, si desea establecer otros permisos, utilice la interfaz de usuario. Para obtener más información, consulte [Asignación de acceso de usuarios](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- Begin Staging URL vs Prod URL -->

## bluemix account org-role-unset
{: #bluemix_account_org_role_unset}

Elimine un rol de organización de un usuario. Esta operación solamente la puede llevar a cabo un gestor de la organización.

```
bluemix account org-role-unset USER_NAME ORG_NAME ORG_ROLE
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>USER_NAME (necesario)</dt>
   <dd>Nombre del usuario al que se elimina.</dd>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización de la que se elimina a este usuario.</dd>
   <dt>ORG_ROLE (necesario)</dt>
   <dd>Nombre del rol de la organización de la que se elimina a este usuario. Por ejemplo:
   <ul>
   <li>OrgManager: este rol puede invitar y gestionar usuarios, seleccionar y cambiar planes y establecer límites de gasto.</li>
   <li>BillingManager: este rol puede crear y gestionar la cuenta de facturación y la información de pago.</li>
   <li>OrgAuditor: este rol tiene acceso de sólo lectura a informes e información de organización.</li>
   </ul>
   </dd>
    </dl>

<strong>Ejemplos</strong>:

Elimine el usuario `Mary` de la organización `IBM` como el rol de `OrgManager`:

```
bluemix account org-role-unset Mary IBM OrgManager
```

## bluemix account space-users
{: #bluemix_account_space_users}

Visualice usuarios en el espacio especificado según el rol.

```
bluemix account space-users ORG_NAME SPACE_NAME
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización.</dd>
   <dt>SPACE_NAME (necesario)</dt>
   <dd>El nombre del espacio.</dd>
   </dl>


## bluemix account space-role-set
{: #bluemix_account_space_role_set}

Asignar un rol de espacio a un usuario. Esta operación solamente la puede llevar a cabo un gestor de espacios.

```
bluemix account space-role-set USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>USER_NAME (necesario)</dt>
   <dd>Nombre del usuario al que se asigna.</dd>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización a la que se asigna a este usuario.</dd>
   <dt>SPACE_NAME (necesario)</dt>
   <dd>Nombre del espacio al que se asigna a este usuario.</dd>
   <dt>SPACE_ROLE (necesario)</dt>
   <dd>Nombre del rol de espacio al que se asigna a este usuario. Por ejemplo:
   <ul>
   <li>SpaceManager: este rol puede invitar y gestionar usuarios, y habilitar características para un espacio dado.</li>
   <li>SpaceDeveloper: este rol puede crear y gestionar apps y servicios, y ver registros e informes.</li>
   <li>SpaceAuditor: este rol puede ver los registros, informes y valores para el espacio.</li>
   </ul></dd>
    </dl>

<strong>Ejemplos</strong>:

Asigne el usuario `Mary` a la organización `IBM` y al espacio `Cloud` como rol `SpaceManager`:

```
bluemix account space-role-set Mary IBM Cloud SpaceManager
```

## bluemix account space-role-unset
{: #bluemix_account_space_role_unset}

Elimine un rol de espacio de un usuario. Esta operación solamente la puede llevar a cabo un gestor de espacios.

```
bluemix account space-role-unset USER_NAME ORG_NAME SPACE_NAME SPACE_ROLE
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>USER_NAME (necesario)</dt>
   <dd>Nombre del usuario al que se elimina.</dd>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización de la que se elimina a este usuario.</dd>
   <dt>SPACE_NAME (necesario)</dt>
   <dd>Nombre del espacio del que se elimina a este usuario.</dd>
   <dt>SPACE_ROLE (necesario)</dt>
   <dd>Nombre del rol del espacio del que se elimina a este usuario. Por ejemplo:
   <ul>
   <li>SpaceManager: este rol puede invitar y gestionar usuarios, y habilitar características para un espacio dado.</li>
   <li>SpaceDeveloper: este rol puede crear y gestionar apps y servicios, y ver registros e informes.</li>
   <li>SpaceAuditor: este rol puede ver los registros, informes y valores para el espacio.</li>
   </ul></dd>
    </dl>


<strong>Ejemplos</strong>:

Elimine el usuario `Mary` de la organización `IBM` y del espacio `Cloud` como rol `SpaceManager`:

```
bluemix account space-role-unset Mary IBM Cloud SpaceManager
```

## bluemix account list
{: #bluemix_account_list}

Lista todas las cuentas del usuario actual

```
bluemix account list
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión


## bluemix account org-account
{: #bluemix_account_org_account}

Visualiza la cuenta de la organización especificada (se necesita un usuario de la organización)

```
bluemix account org-account ORG_NAME [--guid]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
  <dt>--guid (opcional)</dt>
  <dd>Visualiza únicamente el ID de la cuenta</dd>
</dl>


## bluemix account users
{: #bluemix_account_users}

Muestra usuarios asociados con la cuenta. Esta operación solamente puede realizarla el propietario de cuenta.

```
bluemix account users
```

## bluemix account user-delete
{: #bluemix_account_user_delete}

Suprime un usuario de la cuenta actual (sólo el propietario de la cuenta)

```
bluemix account user-delete USERNAME [-c ACCOUNT_ID] [-f]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>USERNAME (necesario)</dt>
<dd>Nombre de usuario</dd>
<dt>-c ACCOUNT_ID</dt>
<dd>ID de cuenta. Si no se especifica, el valor predeterminado es la cuenta actual.</dd>
<dt>--force, -f (opcional)</dt>
<dd>Forzar la eliminación sin confirmación.</dd>
</dl>

## bluemix account user-invite
{: #bluemix_account_user_invite}

Invita a un usuario a la cuenta con una organización y un rol de espacio ya establecido. Esta operación solamente puede realizarla el propietario de cuenta.

```
bluemix account user-invite USER_NAME ORG_NAME ORG_ROLE SPACE_NAME SPACE_ROLE
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
   <dt>USER_NAME (necesario)</dt>
   <dd>Nombre del usuario al que se invita.</dd>
   <dt>ORG_NAME (necesario)</dt>
   <dd>Nombre de la organización a la que se invita a este usuario.</dd>
   <dt>ORG_ROLE (necesario)</dt>
   <dd>Nombre del rol de la organización al que se invita a este usuario. Por ejemplo:
   <ul>
  <li>OrgManager: este rol puede invitar y gestionar usuarios, seleccionar y cambiar planes y establecer límites de gasto.</li>
  <li>BillingManager: este rol puede crear y gestionar la cuenta de facturación y la información de pago.</li>
  <li>OrgAuditor: este rol tiene acceso de sólo lectura a informes e información de organización.</li>
  </ul> </dd>
   <dt>SPACE_NAME (necesario)</dt>
   <dd>Nombre del espacio al que se invita a este usuario.</dd>
   <dt>SPACE_ROLE (necesario)</dt>
   <dd>Nombre del espacio al que se invita a este usuario. Nombre del rol del espacio al que se invita a este usuario. Por ejemplo:
   <ul>
<li>SpaceManager: este rol puede invitar y gestionar usuarios, y habilitar características para un espacio dado.</li>
<li>SpaceDeveloper: este rol puede crear y gestionar apps y servicios, y ver registros e informes.</li>
<li>SpaceAuditor: este rol puede ver los registros, informes y valores para el espacio.</li>
</ul>
</dd>
</dl>

<strong>Ejemplos</strong>:

Invite al usuario `Mary` a la organización `IBM` como rol `OrgManager` y el espacio `Cloud` como rol `SpaceAuditor`:

```
bluemix account user-invite Mary IBM OrgManager Cloud SpaceAuditor
```
<!-- Begin Staging URL vs Prod URL -->
**Nota**: Establezca roles de espacios/organizaciones durante la invitación utilizando la interfaz de línea de mandatos, sin embargo, si desea establecer otros permisos, utilice la interfaz de usuario. Para obtener más información, consulte [Asignación de acceso de usuarios](https://console.stage1.bluemix.net/docs/iam/assignaccess.html#assignaccess).
<!-- End Staging URL vs Prod URL -->

## bluemix account user-reinvite
{: #bluemix_account_user_reinvite}

Reenviar invitación a un usuario (es necesario ser gestor de organización o propietario de cuenta)

```
bluemix account user-reinvite USER_EMAIL ORG_NAME
```



## bluemix iam service-ids
{: #bluemix_iam_service_ids}

Lista todos los ID de servicio

```
bluemix iam service-ids --uuid
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Mostrar UUID solo de los ID de servicio</dd>
</dl>

<strong>Ejemplos</strong>:
Lista de UUID de todos los ID de servicio bajo la cuenta actual

```
bluemix iam service-ids --uuid
```


## bluemix iam service-id
{: #bluemix_iam_service_id}

Mostrar detalles de un ID de servicio

```
bluemix iam service-id NAME [--uuid]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del servicio</dd>
  <dt>-uuid</dt>
  <dd>Mostrar el UUID del ID de servicio</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar detalles de ID de servicio `sample-test`

```
bluemix iam service-id sample-test
```


## bluemix iam service-id-create
{: #bluemix_iam_service_id_create}

Crear un ID de servicio

```
bluemix iam service-id-create NAME [-d, --description DESCRIPTION]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del servicio</dd>
  <dt>-d, --description</dt>
  <dd>Descripción del ID de servicio</dd>
</dl>

<strong>Ejemplos</strong>:

Crear un ID de servicio con nombre de servicio `sample-test` y descripción `hello, world!`

```
bluemix iam service-id-create sample-test -d 'hello, world!'
```


## bluemix iam service-id-update

{: #bluemix_iam_service_id_update}
Actualizar un ID de servicio

```
bluemix iam service-id-update NAME [-n, --name NEW_NAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del servicio</dd>
  <dt>-n, --name</dt>
  <dd>Nuevo nombre de servicio</dd>
  <dt>-d, --description</dt>
  <dd>Nueva descripción del servicio</dd>
  <dt>-v, --version</dt>
  <dd>Versión del ID de servicio</dd>
  <dt>-f, --force</dt>
  <dd>Actualizar sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Renombrar el ID de servicio `sample-test` a `sample-test-2` sin confirmación

```
bluemix iam service-id-update sample-test -n sample-test-2 -f
```

Actualizar descripción de servicio `sample-test` versión `1-0jn39fbefew`

```
bluemix iam service-id-update sample-test -d 'hello, friend!' -v 1-0jn39fbefew
```


## bluemix iam service-id-delete
{: #bluemix_iam_service_id_delete}

Suprimir un ID de servicio

```
bluemix iam service-id-delete NAME [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del servicio</dd>
  <dt>-f, --force</dt>
  <dd>Suprimir sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Suprimir ID de servicio `sample-teset` sin confirmación

```
bluemix iam service-id-delete sample-teset -f
```


## bluemix iam api-keys
{: #bluemix_iam_api_keys}

Lista todas las claves de API de la plataforma Bluemix

```
bluemix iam api-keys
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

## bluemix iam api-key-create
{: #bluemix_iam_api_key_create}

Crea una nueva clave de API de la plataforma Bluemix

```
bluemix iam api-key-create NAME [-d DESCRIPTION] [-f, --file FILE]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>NAME (necesario)</dt>
<dd>Nombre de la clave de API a crear.</dd>
<dt>-d <i>DESCRIPTION</i> (opcional)</dt>
<dd>Descripción de la clave de API</dd>
<dt>-f, -- file <i>FILE</i></dt>
<dd>Guarda la información de la clave de API en un archivo especificado. Si no se establece, se visualiza el contenido JSON.</dd>
</dl>

<strong>Ejemplos</strong>:

Crea una clave de API y la guarda en un archivo

```
bluemix iam api-key-create MyKey -d "this is my API key" -f key_file
```

## bluemix iam api-key-update
{: #bluemix_iam_api_key_update}

Actualiza una clave de API de la plataforma Bluemix

```
bluemix iam api-key-update NAME [-n NAME] [-d DESCRIPTION]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>NAME (necesario)</dt>
<dd>Nombre anterior de la clave de API a actualizar.</dd>
<dt>-n <i>NAME</i> (opcional)</dt>
<dd>Nuevo nombre de la clave de API</dd>
<dt>-d <i>DESCRIPTION</i> (opcional)</dt>
<dd>Nueva descripción de la clave de API</dd>
</dl>

<strong>Ejemplos</strong>:

Actualiza la descripción de una clave de API:

```
bluemix iam api-key-update MyKey -d "the new description of my key"
```

## bluemix api-key-delete
{: #bluemix_api_key_delete}

Suprime una clave de API de la plataforma Bluemix

```
bluemix iam api-key-delete NAME [-f]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>NAME (necesario)</dt>
<dd>Nombre de la clave de API a suprimir.</dd>
<dt>-f  (opcional)</dt>
<dd>Forzar la eliminación sin confirmación.</dd>
</dl>

## bluemix iam service-api-keys
{: #bluemix_iam_service_api_keys}

Lista todas las claves de API de servicio

```
bluemix iam service-api-keys BOUND_TO 
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
</dl>

<strong>Ejemplos</strong>:

Lista de claves de API de servicio vinculadas al CRN de servicio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-keys "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key
{: #bluemix_iam_service_api_key}

Listar detalles de una clave de API de servicio

```
bluemix iam service-api-key NAME BOUND_TO [--uuid]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-uuid</dt>
  <dd>Visualice el UUID de la clave de API de servicio</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar detalles de la clave de API de servicio `sample-key` vinculada al CRN de servicio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-key sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-create
{: #bluemix_iam_service_api_key_create}

Crear una clave de API de servicio

```
bluemix iam service-api-key-create NAME BOUND_TO [-d, --description DESCRIPTION] [-f, --file FILE]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-d, --description</dt>
  <dd>Descripción de la clave de API</dd>
  <dt>-f, --file</dt>
  <dd>Guarda la información de la clave de API en un archivo especificado. Si no se establece, se visualiza el contenido JSON.</dd>
</dl>

<strong>Ejemplos</strong>:

Crear una clave de API de servicio `sample-key` vinculada al CRN de servicio `crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da`:

```
bluemix iam service-api-key-create sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam service-api-key-update
{: #bluemix_iam_service_api_key_update}

Actualizar una clave de API de servicio

```
bluemix iam service-api-key-update NAME BOUND_TO  [-n, --name NEW_sNAME] [-d, --description DESCRIPTION] [-v, --version VERSION] [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-n, --name</dt>
  <dd>Nuevo nombre de la clave de API de servicio</dd>
  <dt>-d, --description</dt>
  <dd>Nueva descripción de la clave de API de servicio</dd>
  <dt>-v, --version</dt>
  <dd>Versión de la clave de API de servicio</dd>
  <dt>-f, --force</dt>
  <dd>Actualizar sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Renombrar la clave de API de servicio `sample-key` a `new-sample-key`:

```
bluemix iam service-api-key-update sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da" -n new-sample-key
```

## bluemix iam service-api-key-delete
{: #bluemix_iam_service_api_key_delete}

Suprimir una clave de API de servicio

```
bluemix iam service-api-key-delete NAME BOUND_TO [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Suprimir sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Suprimir clave de API de servicio `sample-key`:

```
bluemix iam service-api-key-delete sample-key "crn:v1:bluemix:public:iam:us-south:o/0ab7e8fe-0f04-4af8-b7d5-30af12125de6::serviceid:ServiceId-ec238b6a-8e18-45da-9a0f-d41c35ce04da"
```

## bluemix iam user-policies
{: #bluemix_iam_user_policies}

Lista de políticas de usuario `name@example.com`:

```
bluemix iam user-policies name@example.com
```

<strong>Requisitos previos</strong>: Punto final, inicio de sesión, cuenta de destino

<strong>Opciones de mandato</strong>:
<dl>
<dt>USER_NAME (necesario)</dt>
<dd>Nombre de usuario al que pertenecen las políticas</dd>
</dl>

<strong>Ejemplos</strong>:

Lista de políticas de usuario `name@example.com`:

```
bluemix iam user-policies name@example.com
```

## bluemix iam user-policy
{: #bluemix_iam_user_policy}

Mostrar detalles de una política de usuario

```
bluemix iam user-policy USER_NAME POLICY_ID
```

<strong>Requisitos previos</strong>: Punto final, inicio de sesión, cuenta de destino

<strong>Opciones de mandato</strong>:
<dl>
<dt>USER_NAME (necesario)</dt>
<dd>Nombre de usuario al que pertenece la política</dd>
<dt>POLICY_ID (necesario)</dt>
<dd>ID de la política</dd>
</dl>

<strong>Ejemplos</strong>:

Lista de política `0bb730daa` de usuario `name@example.com`:

```
bluemix iam user-policy name@example.com 0bb730daa
```

## bluemix iam user-policy-create
{: #bluemix_iam_user_policy_create}

Crear una política de usuario

```
bluemix iam user-policy-create USER_NAME {-f, --file JSON_FILE | --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resouce-group-id RESOURCE_GROUP_ID]}
```

<strong>Requisitos previos</strong>: Punto final, inicio de sesión, cuenta de destino

<strong>Opciones de mandato</strong>:
<dl>
<dt>USER_NAME (necesario)</dt>
<dd>Nombre de usuario al que pertenece la política</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Archivo JSON de definición de política</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (opcional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (opcional)</dt>
<dd>Nombre de servicio de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (opcional)</dt>
<dd>Instancia de servicio de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--region <i>REGION</i> (opcional)</dt>
<dd>Región de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (opcional)</dt>
<dd>Tipo de recurso de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (opcional)</dt>
<dd>Recurso de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (opcional)</dt>
<dd>Nombre del grupo de recursos. Es exclusivo con los distintivos '-f, --file', '--resource' y '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (opcional)</dt>
<dd>ID del grupo de recursos. Es exclusivo con los distintivos '-f, --file', '--resource' y '--resource-group-name'.</dd>
  <dd>Nombres de rol de la definición de política. Para los roles soportados de un servicio específico, ejecute 'bluemix iam roles --service SERVICE_NAME'. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
</dl>

<strong>Ejemplos</strong>:

Crear política de usuario para el usuario `name@example.com` desde el archivo JSON de política `policy.json`:

```
bluemix iam user-policy-create name@example.com -f @policy.json
```

Proporcione a `name@example.com` el rol de `Administrador` para todos los recursos de `sample-service`:

```
bluemix iam user-policy-create name@example.com --roles Administrator --service-name sample-service
```

Proporcione a `name@example.com` el rol de `Editor` para el recurso `key123` de la instancia de servicio de ejemplo `ServiceId-ade78e9f` en la región `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Proporcione a `name@example.com` el rol de `Operador` para el grupo de recursos con el ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Proporcione a `name@example.com` el rol de `Visor` para los miembros del grupo de recursos `sample-resource-group`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-name sample-resource-group
```

Proporcione a `name@example.com` el rol de `Visor` para los miembros del grupo de recursos con el ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-create name@example.com --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```

## bluemix iam user-policy-update
{: #bluemix_iam_user_policy_update}

Actualizar una política de usuario

```
bluemix iam user-policy-update USER_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [--roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE] [--resource-group-name RESOURCE_GROUP_NAME] [--resource-group-id RESOURCE_GROUP_ID]}
```

<strong>Requisitos previos</strong>: Punto final, inicio de sesión, cuenta de destino

<strong>Opciones de mandato</strong>:
<dt>USER_NAME (necesario)</dt>
<dd>Nombre de usuario al que pertenece la política</dd>
<dt>POLICY_ID (necesario)</dt>
<dd>ID de la política a actualizar</dd>
<dt>-v, --version <i>VERSION</i> (opcional)</dt>
<dd>Versión de la política existente</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Archivo JSON de definición de política</dd>
<dt>-f, --file <i>FILE</i> (opcional)</dt>
<dd>Archivo JSON de definición de política</dd>
<dt>--roles <i>ROLE_NAME1,ROLE_NAME2...</i> (opcional)</dt>
<dt>--service-name <i>SERVICE_NAME</i> (opcional)</dt>
<dd>Nombre de servicio de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--serivce-instance <i>SERVICE_INSTANCE</i> (opcional)</dt>
<dd>Instancia de servicio de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--region <i>REGION</i> (opcional)</dt>
<dd>Región de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource-type <i>RESOURCE_TYPE</i> (opcional)</dt>
<dd>Tipo de recurso de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource <i>RESOURCE</i> (opcional)</dt>
<dd>Recurso de la definición de política. Es exclusivo con el distintivo '-f, --file'.</dd>
<dt>--resource-group-name <i>RESOURCE_GROUP_NAME</i> (opcional)</dt>
<dd>Nombre del grupo de recursos. Es exclusivo con los distintivos '-f, --file', '--resource' y '--resource-group-id'.</dd>
<dt>--resource-group-id <i>RESOURCE_GROUP_ID</i> (opcional)</dt>
<dd>ID del grupo de recursos. Es exclusivo con los distintivos '-f, --file', '--resource' y '--resource-group-name'.</dd>
  <dd>Nombres de rol de la definición de política. Para los roles soportados de un servicio específico, ejecute 'bluemix iam roles --service SERVICE_NAME'. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
</dl>

<strong>Ejemplos</strong>:

Actualizar la política de usuario con la del archivo JSON：

```
bluemix iam user-policy-update name@example.com 0bb730daa -f @policy.json
```

Actualizar la política de usuario para dar a `name@example.com` el rol de `Administrador` para todos los recursos de `sample-service`：

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Administrator --service-name sample-service
```

 Actualizar la política de usuario para dar a `name@example.com` el rol de `Editor` para el recurso `key123` de la instancia de servicio de ejemplo `ServiceId-ade78e9f` en la región `us-south`:

```
bluemix iam user-policy-create name@example.com --roles Editor --service-name sample-service --service-instance ServiceId-ade78e9f --region us-south --resource-type key --resource key123
```

Actualizar la política de usuario para dar a `name@example.com` el rol de `Operador` para el grupo de recursos con el ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Operator --service-name resource-controller --resource-type resource-group --resource dda27e49d2a1efca58083a01dfde18f6
```

Actualizar la política de usuario para dar a `name@example.com` el rol de `Visor` para los miembros del grupo de recursos `sample-resource-group`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-name sample-resource-group
```

Actualizar la política de usuario para dar a `name@example.com` el rol de `Visor` para los miembros del grupo de recursos con el ID `dda27e49d2a1efca58083a01dfde18f6`:

```
bluemix iam user-policy-update name@example.com user-policy-id --roles Viewer --resource-group-id dda27e49d2a1efca58083a01dfde18f6
```



## bluemix iam service-policies
{: #bluemix_iam_service_policies}

Listar todas las políticas de servicio del servicio especificado

```
bluemix iam service-policies SERVICE_ID_NAME [--json] [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necesario)</dt>
  <dd>Nombre del ID de servicio</dd>
  <dt>-json</dt>
  <dd>Mostrar política en formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Mostrar las políticas de servicios sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Lista de políticas de servicio `test`:

```
bluemix iam service-policies test
```


## bluemix iam service-policy
{: #bluemix_iam_service_policy}

Mostrar detalles de una política de servicio

```
bluemix iam service-policy SERVICE_ID_NAME POLICY_ID [--json] [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necesario)</dt>
  <dd>Nombre del ID de servicio</dd>
  <dt>POLICY_ID (necesario)</dt>
  <dd>ID de la política de servicio<dd>
  <dt>-json</dt>
  <dd>Mostrar política en formato JSON</dd>
  <dt>-f, --force</dt>
  <dd>Mostrar la política de servicios sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar la política `140798e2-8ea7db3` de servicio `test`:

```
bluemix iam service-policies test 140798e2-8ea7db3
```


## bluemix iam service-policy-create
{: #bluemix_iam_service_policy_create}

Crear una política de servicio

```
bluemix iam service-policy-create SERVICE_ID_NAME {-f, --file JSON_FILE | -r, --roles ROLE_NAME1,ROLE_NAME2... [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necesario)</dt>
  <dd>Nombre del ID de servicio</dd>
  <dt>-f, --file</dt>
  <dd>Archivo JSON de definición de política. Con los distintivos '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' y '--resource' son excluyentes.</dd>
  <dt>-r, --roles</dt>
  <dd>Nombres de rol de la definición de política. Para los roles soportados de un servicio específico, ejecute 'bluemix iam roles --service SERVICE_NAME'. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-service-name</dt>
  <dd>Nombre de servicio de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-service-instance</dt>
  <dd>Instancia de servicio de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-region</dt>
  <dd>Región de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo de recurso de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-resource</dt>
  <dd>Recurso de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-F, --force</dt>
  <dd>Crear la política de servicios sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Crear la política de servicio desde el archivo JSON para el servicio `test`:

```
bluemix iam service-policy-create test -f @policy.json
```


## bluemix iam service-policy-update
{: #bluemix_iam_service_policy_update}

Actualizar una política de servicio

```
bluemix iam service-policy-update SERVICE_ID_NAME POLICY_ID [-v, --version VERSION] {-f, --file JSON_FILE | [-r, --roles ROLE_NAME1,ROLE_NAME2...] [--service-name SERVICE_NAME] [--service-instance SERVICE_INSTANCE] [--region REGION] [--resource-type RESOURCE_TYPE] [--resource RESOURCE]} [-F, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necesario)</dt>
  <dd>Nombre del ID de servicio</dd>
  <dt>POLICY_ID (necesario)</dt>
  <dd>ID de la política de servicio<dd>
  <dt>-v, --version</dt>
  <dd>Versión de la política de servicio</dd>
  <dt>-f, --file</dt>
  <dd>Archivo JSON de definición de política. Con los distintivos '-r, --roles', '--service-name', '--service-instance', '--region', '--resource-type' y '--resource' son excluyentes.</dd>
  <dt>-r, --roles</dt>
  <dd>Nombres de rol de la definición de política. Para los roles soportados de un servicio específico, ejecute 'bluemix iam roles --service SERVICE_NAME'. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-service-name</dt>
  <dd>Nombre de servicio de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-service-instance</dt>
  <dd>Instancia de servicio de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-region</dt>
  <dd>Región de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-resource-type</dt>
  <dd>Tipo de recurso de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-resource</dt>
  <dd>Recurso de la definición de política. Esta opción y el distintivo '-f, --file' son mutuamente excluyentes.</dd>
  <dt>-F, --force</dt>
  <dd>Actualizar la política de servicios sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Actualizar la política de servicio `140798e2-8ea7db3` desde el archivo JSON para el servicio `test`:

```
bluemix iam service-policy-update test 140798e2-8ea7db3 -f @policy.json
```

## bluemix iam service-policy-delete
{: #bluemix_iam_service_policy_delete}

Suprimir una política de servicio

```
bluemix iam service-policy-delete SERVICE_ID_NAME POLICY_ID [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>SERVICE_ID_NAME (necesario)</dt>
  <dd>Nombre del ID de servicio</dd>
  <dt>POLICY_ID (necesario)</dt>
  <dd>ID de la política de servicio<dd>
  <dt>-f, --force</dt>
  <dd>Suprimir sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Suprimir la política `140798e2-8ea7db3` del servicio `test`

```
bluemix iam service-policy-delete test 140798e2-8ea7db3
```


## bluemix resource groups
{: #bluemix_resource_groups}

Listar grupos de recursos

```
bluemix resource groups [--default | (-r, --resource RESOURCE_ID -o, --resource-origin RESOURCE_ORIGIN)]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>--default</dt>
  <dd>Obtener grupo predeterminado de la cuenta actual</dd>
  <dt>-r, --resource</dt>
  <dd>ID del recurso de pertenencia</dd>
  <dt>-o, --resource-origin</dt>
  <dd>Origen del recurso de pertenencia. Valores aceptados: 'CF_ORG', 'IMS_ACCOUNT'.</dd>
</dl>

<strong>Ejemplos</strong>:

Listar todos los grupos de recursos de su cuenta de destino actualmente:

```
bluemix resource groups
```

Listar el grupo predeterminado de la cuenta de destino actualmente:

```
bluemix resource groups --default
```

Lista de grupos de recursos que son la correlación de una organización CloudFoundry

```
bluemix resource groups -r d0ef0e-12n3632z9f-ef3w54n -o CF_ORG
```


## bluemix resource group
{: #bluemix_resource_group}

Mostrar detalles de un grupo de recursos

```
bluemix resource group NAME [--id]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del grupo de recursos</dd>
  <dt>--id</dt>
  <dd>Mostrar solo ID</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar grupo de recursos `example-group`:

```
bluemix resource group example-group
```

Mostrar sólo el ID del grupo de recursos `example-group`:

```
bluemix resourxce group example-group --id
```


## bluemix resource group-update
{: #bluemix_resource_group_update}

Actualizar un grupo de recursos existente

```
bluemix resource group-update NAME [-n, --name NEW_NAME] [-q, --quota NEW_QUOTA_NAME]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre del grupo de recursos de destino</dd>
  <dt>-n, --name</dt>
  <dd>Nuevo nombre de grupo de recursos</dd>
  <dt>-q, --quota</dt>
  <dd>Nombre de la nueva definición de cuota</dd>
  <dt>-f</dt>
  <dd>Forzar actualización sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:

Cambie el nombre del grupo de recursos `example-group` a `trial-group`:

```
bluemix resource group-update example-group -n trial-group
```

Cambie la cuota del grupo de recursos `example-group` a `free`:

```
bluemix resource group-update example-group -q free
```

## bluemix resource quotas
{: #bluemix_resource_quotas}

Listar todas las definiciones de cuota

```
bluemix resource quotas
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
</dl>

<strong>Ejemplos</strong>:

Listar todas las definiciones de cuota:

```
bluemix resource quotas
```

## bluemix resource quota
{: #bluemix_resource_quota}

Mostrar detalles de una definición de cuota

```
bluemix resource quota NAME
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre de la cuota</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar detalles de cuota `free`:

```
bluemix resource quota free
```


## bluemix app push
{: #bluemix_app_push}

Este mandato tiene la misma función y opciones que el mandato `cf push`.


## bluemix app list
{: #bluemix_app_list}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf apps`.


## bluemix app show
{: #bluemix_app_show}

Este mandato tiene la misma función y opciones que el mandato `cf app`.


## bluemix app delete
{: #bluemix_app_delete}

Este mandato tiene la misma función y opciones que el mandato `cf delete`.


## bluemix app rename
{: #bluemix_app_rename}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf rename`.


## bluemix app start
{: #bluemix_app_start}

Este mandato tiene la misma función y opciones que el mandato `cf start`.


## bluemix app stop
{: #bluemix_app_stop}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf stop`.


## bluemix app restart
{: #bluemix_app_restart}

Este mandato tiene la misma función y opciones que el mandato `cf restart`.


## bluemix app restage
{: #bluemix_app_restage}


Este mandato tiene la misma función y las mismas opciones que el mandato `cf restage`.


## bluemix app instance-restart
{: #bluemix_app_instance_restart}


Este mandato tiene la misma función y opciones que el mandato `cf restart-app-instance`.


## bluemix app events
{: #bluemix_app_events}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf events`.


## bluemix app files
{: #bluemix_app_files}

Este mandato tiene la misma función y opciones que el mandato `cf files`.


## bluemix app logs
{: #bluemix_app_logs}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf logs`.


## bluemix app env
{: #bluemix_app_env}

Este mandato tiene la misma función y opciones que el mandato `cf env`.


## bluemix app env-set
{: #bluemix_app_env_set}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf set-env`.


## bluemix app env-unset
{: #bluemix_app_env_unset}

Este mandato tiene la misma función y opciones que el mandato `cf unset-env`.


## bluemix app stacks
{: #bluemix_app_stacks}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf stacks`.


## bluemix app stack-show
{: #bluemix_app_stack_show}

Este mandato tiene la misma función y opciones que el mandato `cf stack`.


## bluemix app manifest-create
{: #bluemix_app_manifest_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-app-manifest`.

## bluemix app domain-cert 
{: #bluemix_app_domain_cert}

Liste la información de certificado de un dominio.

```
bluemix app domain-cert DOMAIN_NAME
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
<dl>
<dt>DOMAIN_NAME (necesario)</dt>
<dd>Nombre del dominio que aloja el certificado.</dd>
</dl>


<strong>Ejemplos</strong>:

Ver la información de certificado del dominio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert ibmcxo-eventconnect.com
```

## bluemix app domain-cert-add
{: #bluemix_app_domain_cert_add}

Añadir un certificado para el dominio especificado en la organización actual.

```
bluemix app domain-cert-add DOMAIN -k PRIVATE_KEY_FILE -c CERT_FILE [-p PASSWORD] [-i INTERMEDIATE_CERT_FILE] [-t TRUST_STORE_FILE]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>DOMAIN (necesario)</dt>
   <dd>Dominio al que se añade el certificado.</dd>
   <dt>-k <i>PRIVATE_KEY_FILE</i> (necesario)</dt>
   <dd>Vía de acceso del archivo de claves privado.</dd>
   <dt>-c <i>CERT_FILE</i> (necesario)</dt>
   <dd>Vía de acceso del archivo de certificado.</dd>
   <dt>-p <i>PASSWORD</i> (opcional)</dt>
   <dd>Contraseña del certificado.</dd>
   <dt>-i <i>INTERMEDIATE_CERT_FILE</i> (opcional)</dt>
   <dd>Vía de acceso del archivo de certificado intermedio.</dd>
   <dt>-t <i>TRUST_STORE_FILE</i> (opcional)</dt>
   <dd>Archivo del almacén de confianza.</dd>
   </dl>


<strong>Ejemplos</strong>:

Añadir un certificado al dominio `ibmcxo-eventconnect.com`:

```
bluemix app domain-cert-add ibmcxo-eventconnect.com -k key_file.key -c cert_file.crt -p 123 -i inter_cert.cert
```

## bluemix app domain-cert-remove
{: #bluemix_app_domain_cert_remove}

Eliminar un certificado del dominio especificado en la organización actual.

```
bluemix app domain-cert-remove DOMAIN [-f]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>DOMAIN (necesario)</dt>
   <dd>Dominio a eliminar del certificado.</dd>
   <dt>-f  (opcional)</dt>
   <dd>Forzar la eliminación sin confirmación.</dd>
   </dl>

## bluemix app domains
{: #bluemix_app_domains}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-shared-domain`.

## bluemix app routes
{: #bluemix_app_routes}

Este mandato tiene la misma función y opciones que el mandato `cf routes`.


## bluemix app route-check
{: #bluemix_app_route_check}

Este mandato tiene la misma función y opciones que el mandato `cf check-route`.


## bluemix app route-map
{: #bluemix_app_route_map}

Correlacione una ruta a una app cf o grupo de contenedores que tenga un dominio y nombre de host específicos.

```
bluemix app route-map CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (necesario)</dt>
   <dd>Nombre de la aplicación cf o del grupo de contenedores que debe correlacionarse con una ruta.</dd>
   <dt>DOMAIN (necesario)</dt>
   <dd>Dominio de la ruta. Por ejemplo, mychinabluemix.net o chinabluemix.net. </dd>
   <dt>-n <i>HOST_NAME</i> (opcional)</dt>
   <dd>Nombre de host de la ruta. Si no se facilita, el nombre de host se establece en el nombre de la app o grupo de contenedores de forma predeterminada.</dd>
   </dl>

<strong>Ejemplos</strong>:

Correlacionar una ruta a `my-app` con un dominio especificado:

```
bluemix app route-map my-app mychinabluemix.net
```

Correlacione una ruta a 'my-container-group' con el dominio y el nombre de host especificados:

```
bluemix app route-map my-container-group chinabluemix.net -n abc
```


## bluemix app route-unmap
{: #bluemix_app_route_unmap}

Elimina la correlación entre la ruta específica y una app cf existente o grupo de contenedores.

```
bluemix app route-unmap CF_APP_NAME|CONTAINER_GROUP_NAME  DOMAIN  [-n HOST_NAME]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>CF_APP_NAME|CONTAINER_GROUP_NAME (necesario)</dt>
   <dd>Nombre de la aplicación cf o del grupo de contenedores.</dd>
   <dt>DOMAIN (necesario)</dt>
   <dd>Dominio de la ruta (por ejemplo, mychinabluemix.net o chinabluemix.net).</dd>
   <dt>-n <i>HOST_NAME</i> (opcional)</dt>
   <dd>Nombre de host de la ruta. Si no se proporciona, el nombre de host se establece en el nombre de la app o en el nombre de grupo de contenedores de forma predeterminada.</dd>
   </dl>

<strong>Ejemplos</strong>:

Descorrelacionar `my-app.mychinabluemix.net` desde `my-app`:

```
bluemix app route-unmap my-app mychianbluemix.net
```

Descorrelacionar `abc.chinabluexmix.net` desde `my-container-group`:

```
bluemix app route-unmap my-container-group chinabluemix.net -n abc
```


## bluemix app route-create
{: #bluemix_app_route_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-route`.


## bluemix app route-delete
{: #bluemix_app_route_delete}

Este mandato tiene la misma función y opciones que el mandato `cf delete-route`.


## bluemix app orphaned-routes-delete
{: #bluemix_app_orphaned_routes_delete}

Este mandato tiene la misma función y opciones que el mandato `cf delete-orphaned-routes`.


## bluemix app domains
{: #bluemix_app_domains}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf domains`.


## bluemix app domain-create
{: #bluemix_app_domain_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-domain`.


## bluemix app domain-delete
{: #bluemix_app_domain_delete}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-domain`.


## bluemix app shared-domain-create
{: #bluemix_app_shared_domain_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-shared-domain`.


## bluemix app shared-domain-delete
{: #bluemix_app_shared_domain_delete}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-shared-domain`.


## bluemix service offerings
{: #bluemix_service_offerings}


Este mandato tiene la misma función y opciones que el mandato `cf marketplace`.


## bluemix service list
{: #bluemix_service_list}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf services`.


## bluemix service show
{: #bluemix_service_show}

Este mandato tiene la misma función y opciones que el mandato `cf service`.


## bluemix service create
{: #bluemix_service_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-service`.


## bluemix service update
{: #bluemix_service_update}

Este mandato tiene la misma función y opciones que el mandato `cf update-service`.


## bluemix service delete
{: #bluemix_service_delete}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf delete-service`.


## bluemix service rename
{: #bluemix_service_rename}

Este mandato tiene la misma función y opciones que el mandato `cf rename-service`.


## bluemix service bind
{: #bluemix_service_bind}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf bind-service`.


## bluemix service unbind
{: #bluemix_service_unbind}

Este mandato tiene la misma función y opciones que el mandato `cf unbind-service`.


## bluemix service key-create
{: #bluemix_service_key_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-service-key`.


## bluemix service key-delete
{: #bluemix_service_key_delete}

Este mandato tiene la misma función y opciones que el mandato `cf delete-service-key`.


## bluemix service keys
{: #bluemix_service_keys}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf service-keys`.


## bluemix service key-show
{: #bluemix_service_key_show}

Este mandato tiene la misma función y opciones que el mandato `cf service-key`.


## bluemix service user-provided-create
{: #bluemix_service_user_provided_create}

Este mandato tiene la misma función y las mismas opciones que el mandato `cf create-user-provided-service`.


## bluemix service user-provided-update
{: #bluemix_service_user_provided_update}

Este mandato tiene la misma función y opciones que el mandato `cf update-user-provided-service`.


## bluemix resource instances
{: #bluemix_resource_instances}

Listar instancias de recursos

```
bluemix resource instances [--resource-name RESOURCE_NAME] [-r, --region REGION_ID] [--long]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>--resource-name</dt>
  <dd>Nombre de recurso de pertenencia</dd>
  <dt>-r, --region</dt>
  <dd>Filtrar por ID de región, si no se especifica, el valor predeterminado es la región actual, '-r, --region all' para mostrar instancias de recurso de todas las regiones</dd>
  <dt>--long</dt>
  <dd>Mostrar campos adicionales en la salida</dd>
</dl>

<strong>Ejemplos</strong>:

Lista de instancias de recursos del recurso `test-resource`:

```
bluemix resource instances --resource-name test-resource
```

## bluemix resource instance
{: #bluemix_resource_instance}

Mostrar detalles de una instancia de recursos

```
bluemix resource instance NAME [-r, --region REGION] [--id]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre de la instancia de recursos</dd>
  <dt>-r, --region</dt>
  <dd>Filtrar por ID de región, si no se especifica, el valor predeterminado es la región actual, '-r, --region all' para mostrar instancias de recurso de todas las regiones</dd>
  <dt>--id</dt>
  <dd>Mostrar ID de instancia de recurso</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar detalles de instancia de recursos `my-resource-instance`:

```
bluemix resource instance my-resource-instance
```

## bluemix resource instance-create
{: #bluemix_resource_instance_create}

Crear una instancia de recurso

```
bluemix resource instance-create NAME RESOURCE_NAME|RESOURCE_ID RESOURCE_PLAN_NAME|RESOURCE_PLAN_ID [-r, --region REGION] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NAME (necesario)</dt>
  <dd>Nombre de la instancia de recursos</dd>
  <dt>RESOURCE_NAME o RESOURCE_ID (necesario)</dt>
  <dd>Nombre o ID del recurso</dd>
  <dt>RESOURCE_PLAN_NAME o RESOURCE_PLAN_ID (necesario)</dt>
  <dd>Nombre o ID del plan de recursos</dd>
  <dt>-r, --region</dt>
  <dd>Región para crear la instancia de recurso. Si no se especifica, el valor predeterminado es la región actual.</dd>
  <dt>-t, --tags</dt>
  <dd>Etiquetas</dd>
  <dt>-p, --parameters</dt>
  <dd>Archivo JSON o serie JSON de parámetros para crear instancia de recurso</dd>
</dl>

<strong>Ejemplos</strong>:
Crear una instancia de recursos denominada `my-resource-instance` utilizando el plan de recursos `test-resource-plan` del recurso `test-resource`:

```
bluemix resource instance-create my-resource-instance test-resource test-resource-plan
```

## bluemix resource instance-update
{: #bluemix_resource_instance_update}

Actualizar instancia de recursos

```
bluemix resource instance-update RESOURCE_INSTANCE_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [--resource-plan-id RESOURCE_PLAN_ID] [--update-time UPDATE_TIME] [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>RESOURCE_INSTANCE_NAME (necesario)</dt>
  <dd>Nombre de la instancia de recursos</dd>
  <dt>-n, --name</dt>
  <dd>Nuevo nombre instancia de recursos</dd>
  <dt>-t, --tags</dt>
  <dd>Etiquetas nuevas</dd>
  <dt>--resource-plan-id</dt>
  <dd>Nuevo ID de plan de recursos</dd>
  <dt>--update-time</dt>
  <dd>Tiempo en segundos desde la época en que el registro facturable debería haber entrado en vigor</dd>
  <dt>-f, --force</dt>
  <dd>Forzar actualización sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Actualizar instancia de recursos `my-resource-instance`, cambiar su nombre a `new-resource-instance`:

```
bluemix resource instance-update my-resource-instance -n new-resource-instance
```

## bluemix resource instance-delete
{: #bluemix_resource_instance_delete}

Suprimir instancia de recurso

```
bluemix resource instance-delete NAME [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-f, --force</dt>
  <dd>Forzar la supresión sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Suprimir instancia de recursos `my-resource-instance`:

```
bluemix resource instance-delete my-resource-instance
```

## bluemix resource bindings
{: #bluemix_resource_bindings}

Mostrar enlaces a alias de recurso

```
bluemix resource bindings RESOURCE_ALIAS
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>RESOURCE_ALIAS (necesario)</dt>
  <dd>Nombre de alias de recursos</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar enlaces a recursos de alias de recursos `my-resource-alias`:

```
bluemix resource bindings my-resource-alias
```
## bluemix resource binding
{: #bluemix_resource_binding}

Mostrar detalles de un enlace de recurso

```
bluemix resource binding ALIAS_NAME APP_NAME [--id]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>ALIAS_NAME (necesario)</dt>
  <dd>Nombre de alias de recursos</dd>
  <dt>APP_NAME</dt>
  <dd>Nombre de aplicación de CloudFoundry</dd>
  <dt>--id</dt>
  <dd>Solo se mostrará el ID. Se suprimirá el resto de la salida del enlace de recurso.</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar detalles de enlaces a recursos entre el alias de recurso `my-resource-alias` y la app `my-app`:

```
bluemix resource bindings my-resource-alias my-app
```

## bluemix resource binding-create
{: #bluemix_resource_binding_create}

Crear un enlace de recurso

```
bluemix resource binding-create RESOURCE_ALIAS_NAME APP_NAME ROLE_NAME [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (necesario)</dt>
  <dd>Nombre de alias de recursos</dd>
  <dt>APP_NAME</dt>
  <dd>Nombre de aplicación de CloudFoundry</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nombre del rol de usuario</dd>
  <dt>--service-id-name</dt>
  <dd>Nombre del ID de servicio al que pertenece el rol</dd>
  <dt>-f, --force</dt>
  <dd>Forzar la creación sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Crear enlaces a un recurso entre el alias de recurso `my-resource-alias` y la app `my-app` con el rol de `Administrador`:

```
bluemix resource binding-create my-resource-alias my-app Administrator
```
## bluemix resource binding-delete
{: #bluemix_resource_binding_delete}

Suprimir un enlace de recurso

```
bluemix resource binding-delete RESOURCE_ALIAS APP_NAME [-f, --force]
```

<strong>Requisitos previos</strong>: Ninguno

<strong>Opciones de mandato</strong>:
<dl>
  <dt>RESOURCE_ALIAS_NAME (necesario)</dt>
  <dd>Nombre de alias de recursos</dd>
  <dt>APP_NAME</dt>
  <dd>Nombre de aplicación de CloudFoundry</dd>
  <dt>-f, --force</dt>
  <dd>Forzar la supresión sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Suprimir el enlace a recursos entre el alias de recurso `my-resource-alias` y la app `my-app`:

```
bluemix resource binding-delete my-resource-alias my-app
```

## bluemix resource keys
{: #bluemix_resource_keys}

Listar claves de recurso de instancia de recursos o alias de recurso

```
bluemix resource keys [ --instance-id ID | --instance-name NAME | --alias-id ID | --alias-name NAME ]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID de instancia de recursos</dd>
  <dt>--instance-name</dt>
  <dd>Nombre de instancia de recursos</dd>
  <dt>--alias-id</dt>
  <dd>ID de alias de recurso</dd>
  <dt>--alias-name</dt>
  <dd>Nombre de alias de recursos</dd>
</dl>

<strong>Ejemplos</strong>:
Lista de claves de recursos de instancia de recursos `my-resource-instance`:

```
bluemix resource keys --instance-name my-resource-instance
```

## bluemix resource key
{: #bluemix_resource_key}

Mostrar detalles de una clave de recurso

```
bluemix resource key KEY_NAME [--id]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nombre de la clave</dd>
  <dt>--id</dt>
  <dd>Mostrar ID de clave de recurso</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar detalles de claves de recursos `my-resource-key`:

```
bluemix resource key my-resource-key
```

## bluemix resource key-create
{: #bluemix_resource_key_create}

Crear una clave de recurso

```
bluemix resource key-create NAME ROLE_NAME ( --instance-id RESOURCE_INSTANCE_ID | --instance-name RESOURCE_INSTANCE_NAME | --alias-id RESOURCE_ALIAS_ID | --alias-name RESOURCE_ALIAS_NAME ) [--service-id-name SERVICE_ID_NAME [-f, --force]]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>NOMBRE</dt>
  <dd>Nombre de la clave</dd>
  <dt>ROLE_NAME</dt>
  <dd>Nombre del rol de usuario</dd>
  <dt>--instance-id</dt>
  <dd>ID de instancia de recursos</dd>
  <dt>--instance-name</dt>
  <dd>Nombre de instancia de recursos</dd>
  <dt>--alias-id</dt>
  <dd>ID de alias de recurso</dd>
  <dt>--alias-name</dt>
  <dd>Nombre de alias de recursos</dd>
  <dt>-service-id-name</dt>
  <dd>Nombre del ID de servicio al que pertenece el rol</dd>
  <dt>-f, --force</dt>
  <dd>Forzar la creación sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Crear una clave de recurso denominada `my-resource-key` con el rol de `Administrador` para la instancia de recursos `my-resource-instance`:

```
bluemix resource key-create my-resource-key Administrator --instance-name my-resource-instance
```

## bluemix resource key-delete
{: #bluemix_resource_key_delete}

Suprimir una clave de recurso

```
bluemix resource key-delete KEY_NAME [-f, --forece]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>KEY_NAME</dt>
  <dd>Nombre de la clave</dd>
  <dt>-f, --force</dt>
  <dd>Forzar la supresión sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Suprimir la clave de recurso `my-resource-key`:

```
bluemix resource key-delete my-resource-key
```

## bluemix resource aliases
{: #bluemix_resource_aliases}

Listar alias de una instancia de recursos

```
bluemix resource aliases [ --instance-id ID | --instance-name NAME ]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>--instance-id</dt>
  <dd>ID de la instancia del recurso de pertenencia.</dd>
  <dt>--instance-name</dt>
  <dd>Nombre de la instancia de recurso de pertenencia.</dd>
</dl>

<strong>Ejemplos</strong>:
Lista de alias de recursos para la instancia de recursos `my-resource-instance`:
```
bluemix resource aliases my-resource-instance
```

## bluemix resource alias
{: #bluemix_resource_alias}

Mostrar detalles de un alias de recurso

```
bluemix resource alias ALIAS_NAME [--id]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>ALIAS_NAME (necesario)</dt>
  <dd>Nombre del alias de recurso</dd>
  <dt>--id</dt>
  <dd>Solo se mostrará el ID del alias de recurso proporcionado. Se suprimirá el resto de la salida para el alias.</dd>
</dl>

<strong>Ejemplos</strong>:
Mostrar detalles del alias de recursos `my-resource-alias`:
```
bluemix resource aliase  my-resource-alias
```

## bluemix resource alias-create
{: #bluemix_resource_alias_create}

Crear un alias de una instancia de recurso

```
bluemix resource alias-create ALIAS_NAME ( --instance-id ID | --instance-name NAME ) [-s SPACE_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_TEXT]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>ALIAS_NAME (necesario)</dt>
  <dd>Nombre del alias de recurso</dd>
  <dt>--instance-id</dt>
  <dd>ID de la instancia del recurso de pertenencia.</dd>
  <dt>--instance-name</dt>
  <dd>Nombre de la instancia de recurso de pertenencia.</dd>
  <dt>-s</dt>
  <dd>Nombre del espacio en el que se ha creado el alias. El valor predeterminado es el espacio actual.</dd>
  <dt>-t, --tags</dt>
  <dd>Lista de etiquetas.</dd>
  <dt>-p, --parameters</dt>
  <dd>Parámetros del archivo JSON o de la serie JSON.</dd>
</dl>

<strong>Ejemplos</strong>:
Crear un alias de recurso denominado `my-resource-alias` de la instancia de recursos `my-resource-instance`:
```
bluemix resource aliase-create my-resource-alias --instance-name my-resource-instance
```

## bluemix resource alias-update
{: #bluemix_resource_alias_update}

Actualizar un alias de recurso

```
bluemix resource alias-update ALIAS_NAME [-n, --name NEW_NAME] [-t, --tags TAGS] [-p, --parameters @JSON_FILE | JSON_STRING ][-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>ALIAS_NAME (necesario)</dt>
  <dd>Nombre del alias de recurso</dd>
  <dt>-n, --name</dt>
  <dd>Nuevo nombre de alias de recurso.</dd>
  <dt>-t, --tags</dt>
  <dd>Lista de etiquetas.</dd>
  <dt>-p, --parameters</dt>
  <dd>Parámetros del archivo JSON o de la serie JSON.</dd>
  <dt>-f, --force</dt>
  <dd>Forzar actualización sin confirmación del usuario.</dd>
</dl>

<strong>Ejemplos</strong>:
Actualizar el alias de recurso `my-resource-alias`, cambiar su nombre a `new-resource-alias`:

```
bluemix resource alias-update my-resource-alias -n new-resource-alias
```

## bluemix resource alias-delete
{: #bluemix_resource_alias_delete}

Suprimir un alias de recurso

```
bluemix resource alias-delete ALIAS_NAME [-f, --force]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>ALIAS_NAME (necesario)</dt>
  <dd>Nombre del alias de recurso</dd>
  <dt>-f, --force</dt>
  <dd>Forzar la supresión sin confirmación</dd>
</dl>

<strong>Ejemplos</strong>:
Suprimir alias de recurso `my-resource-alias`:

```
bluemix resource alias-delete my-resource-alias
```

## bluemix catalog search
{: #bluemix_catalog_search}

Buscar entradas de catálogo

```
bluemix catalog search [-q, --query KEY_WORDS] [-r, --region REGION] [-k, --kind KIND] [-p, --price PRICE] [-t, --tag TAG] [--sort-by PROPERTY] [--reverse] [--json] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-q, --query</dt>
  <dd>Palabra clave de búsqueda</dd>
  <dt>-r, --region</dt>
  <dd>Especifique la región geográfica en la que buscar. Actualmente sólo están soportadas "us-south" y "united-kingdom"</dd>
  <dt>-k, --kind</dt>
  <dd>Filtrar por tipo de recursos. Actualmente, sólo están soportados "service-cf", "iaas", "runtime", "template" y "dashboard"</dd>
  <dt>-p, --price</dt>
  <dd>Filtrar por precio. Actualmente, sólo están soportados "free", "paygo" y "bluemix-subscription"</dd>
  <dt>-t, --tag</dt>
  <dd>Filtrar por etiqueta.</dd>
  <dt>-sort-by</dt>
  <dd>Propiedad por la que ordenar</dd>
  <dt>-reverse</dt>
  <dd>Indica si debe revertirse el orden de clasificación</dd>
  <dt>-json</dt>
  <dd>Respuesta JSON original de la salida</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Busque el servicio `Prueba de automatización`:

```
bluemix catalog search -k service -q 'Automation test'
```


## bluemix catalog entry
{: #bluemix_catalog_entry}

Obtener una entrada de catálogo

```
bluemix catalog entry [-i ID] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>El ID de la entrada de catálogo.</dd>
  <dt>-children</dt>
  <dd>Obtener todos los hijos para la entrada de catálogo</dd>
  <dt>-json</dt>
  <dd>Respuesta JSON original de la salida</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Obtener entrada con el ID `a0ef1-d3b4j0`:

```
bluemix catalog entry 'a0ef1-d3b4j0'
```


## bluemix catalog entry-create
{: #bluemix_catalog_entry_create}
Crear una nueva entrada de catálogo (sólo administrador del catálogo de una cuenta)

```
bluemix catalog entry-create [-c PARAMETERS_AS_JSON] [-p, --parent PARENT] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-p, --parent</dt>
  <dd>ID padre del objeto</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido que contiene parámetros de configuración específicos del catálogo, proporcionados en línea o en un archivo. Para obtener una lista de parámetros de configuración soportados, consulte la documentación para la entrada de catálogo concreta.</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Crear recurso desde el archivo JSON con el ID padre `a0ef1-d3b4j0`:

```
bluemix catalog entry-create -c @entry.json -p 'a0ef1-d3b4j0'
```


## bluemix catalog entry-update
{: #bluemix_catalog_entry_update}
Actualizar una entrada de catálogo existente (sólo administrador o editor del catálogo de una cuenta)

```
bluemix catalog entry-update [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>El ID de la entrada de catálogo que se está actualizando.</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido que contiene parámetros de configuración específicos del catálogo, proporcionados en línea o en un archivo. Para obtener una lista de parámetros de configuración soportados, consulte la documentación para la entrada de catálogo concreta.</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Actualizar recurso `j402-dnf1i` desde el archivo JSON:

```
bluemix entry-update -i 'j402-dnf1i' -c @update.json
```

## bluemix catalog entry-visibility
{: #bluemix_catalog_entry_visibility}
Obtener la visibilidad para una entrada de catálogo (sólo administrador del catálogo de una cuenta)

```
bluemix catalog entry-visibility [-i ID] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>El ID de la entrada de catálogo.</dd>
  <dt>-json</dt>
  <dd>Respuesta JSON original de la salida</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Obtener la visibilidad de recursos `j402-dnf1i` en el ámbito global:

```
bluemix catalog entry-visibility 'j402-dnf1i' --global
```


## bluemix catalog entry-visibility-set
{: #bluemix_catalog_entry_visibility_set}
Actualizar la visibilidad de una entrada de catálogo existente (sólo administrador del catálogo de una cuenta)

```
bluemix catalog entry-visibility-set [-i ID] [-c PARAMETERS_AS_JSON] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-i, --id</dt>
  <dd>El ID de la entrada de catálogo que se está actualizando.</dd>
  <dt>-c</dt>
  <dd>Objeto JSON válido que contiene parámetros de configuración específicos del catálogo, proporcionados en línea o en un archivo. Para obtener una lista de parámetros de configuración soportados, consulte la documentación para la entrada de catálogo concreta.</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Establecer visibilidad del recurso `j402-dnf1i` desde el archivo JSON:

```
bluemix catalog entry-visibility-set -i 'j402-dnf1i' -c @visibility.json
```


## bluemix catalog service-marketplace
{: #bluemix_catalog_service_marketplace}
Lista de ofertas de servicios en el mercado

```
bluemix catalog service-marketplace [--cf] [--rc] [--global]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
<dl>
  <dt>-cf</dt>
  <dd>Mostrar sólo servicios de Cloud Foundry</dd>
  <dt>-rc</dt>
  <dd>Mostrar sólo servicios compatibles con RC</dd>
  <dt>-global</dt>
  <dd>Operar en ámbito global</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar ofertas de servicio en el ámbito global:

```
bluemix catalog service-marketplace --global
```

## bluemix catalog templates
{: #bluemix_catalog_templates}

Visualizar las plantillas de contenedor modelo en Bluemix.

```
bluemix catalog templates [-d]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>-d (opcional)</dt>
   <dd>Si se especifica la opción <i>-d</i>, también se mostrará la descripción de cada plantilla. De lo contrario, sólo se mostrará el ID y el nombre de cada plantilla.</dd>
   </dl>


## bluemix catalog template
{: #bluemix_catalog_template}

Ver la información detallada de una plantilla de contenedor modelo especificada.

```
bluemix catalog template TEMPLATE_ID
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>TEMPLATE_ID (necesario)</dt>
   <dd>ID de la plantilla de contenedor modelo. Utilice <i>bluemix templates</i> para ver los ID de todas las plantillas.</dd>
   </dl>


<strong>Ejemplos</strong>:

Ver detalles de la plantilla `mobileBackendStarter`:

```
bluemix catalog template mobileBackendStarter
```


## bluemix catalog template-run
{: #bluemix_catalog_template_run}

Crea una app cf que se base en la plantilla específica con el URL y la descripción especificados. De forma predeterminada, la nueva app se iniciará automáticamente.

```
bluemix catalog template-run TEMPLATE_ID CF_APP_NAME [-u URL] [-d DESCRIPTION] [--no-start]
```

<strong>Requisitos previos</strong>:  Punto final, inicio de sesión, destino

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>TEMPLATE_ID (necesario)</dt>
   <dd>Plantilla en la que se basará la app cuando se cree. Utilice <i>bluemix templates</i> para ver el ID de todas las plantillas.</dd>
   <dt>CF_APP_NAME (necesario)</dt>
   <dd>Nombre de la aplicación cf que se debe crear.</dd>
   <dt>-u <i>URL</i> (opcional)</dt>
   <dd>Ruta de la aplicación. Si no se especifica, Bluemix establece la ruta automáticamente basándose en el nombre de su app y el dominio predeterminado.</dd>
   <dt>-d <i>DESCRIPTION</i> (opcional)</dt>
   <dd>Descripción de la aplicación.</dd>
   <dt>--no-start (opcional)</dt>
   <dd>No inicie la app automáticamente después de crearla. Si no se especifica, la app se iniciará automáticamente una vez que se haya creado.</dd>
   </dl>


<strong>Ejemplos</strong>:

Crear una aplicación cf `my-app` basada en la plantilla `javaHelloWorld`:

```
bluemix catalog template-run javaHelloWorld my-app
```

Crear una aplicación `my-ruby-app` en función de la plantilla `rubyHelloWorld` con la ruta `myrubyapp.chinabluemix.net` y la descripción `Mi primera app ruby en {{site.data.keyword.Bluemix_notm}}.`:

```
bluemix catalog template-run rubyHelloWorld my-ruby-app -u myrubyapp.chinabluemix.net -d "My first ruby app on {{site.data.keyword.Bluemix_notm}}."
```

Crear una aplicación `my-python-app` basada en la plantilla `pythonHelloWorld` sin inicio automático:

```
bluemix catalog template-run pythonHelloWorld my-python-app --no-start
```

## bluemix billing account-usage
{: #bluemix_billing_account_usage}

Mostrar el uso y coste mensual de la cuenta.

```
bluemix billing account-usage [-d AAAA-MM] [--json]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

<dl>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Mostrar datos para el mes y la fecha especificados utilizando el formato AAAA-MM. Si no se especifica, se muestra el uso en el mes actual.</dd>
  <dt>--json (opcional)</dt>
  <dd>Mostrar el resultado del uso en formato JSON.</dd>
</dl>

<strong>Ejemplos</strong>:

Mostrar el informe de uso y coste de mi cuenta en 2016-06:

```
bluemix billing account-usage -d 2016-06
```

## bluemix billing org-usage
{: #bluemix_billing_org_usage}

Mostrar los detalles de uso mensual de una organización. Esta operación solo la puede llevar a cabo un gestor de facturación de la organización.

```
bluemix billing org-usage ORG_NAME [-d AAAAA-MM] [-r REGION_NAME] [--json]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

<dl>
  <dt>ORG_NAME (necesario)</dt>
  <dd>Nombre de la organización.</dd>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Mostrar datos para el mes y la fecha especificados utilizando el formato AAAA-MM. Si no se especifica, se muestra el uso en el mes actual.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nombre de la región en que se encuentra la organización. Si se establece en 'todas', se muestra el uso de la organización en todas las regiones.</dd>
  <dt>--json (opcional)</dt>
  <dd>Mostrar el resultado del uso en formato JSON.</dd>
</dl>



## bluemix billing orgs-usage-summary
{: #bluemix_billing_orgs_usage_summary}

Mostrar el resumen de uso mensual de las organizaciones de mi cuenta.

```
bluemix billing orgs-usage-summary [-d AAAA-MM] [-r REGION_NAME] [--json]
```

<strong>Requisitos previos</strong>:  Punto final, Inicio de sesión

<strong>Opciones de mandato</strong>:

<dl>
  <dt>-d MONTH_DATE (opcional)</dt>
  <dd>Mostrar datos para el mes y la fecha especificados utilizando el formato AAAA-MM. Si no se especifica, se muestra el uso en el mes actual.</dd>
  <dt>-r REGION_NAME</dt>
  <dd>Nombre de la región en que se encuentran las organizaciones. Si se establece en 'todas', se muestra el resumen de uso de las organizaciones en todas las regiones.</dd>
  <dt>--json (opcional)</dt>
  <dd>Mostrar el resultado del uso en formato JSON.</dd>
</dl>


## bluemix plugin repos
{: #bluemix_plugin_repos}

Cree una lista de todos los repositorios de plugin que se registran en {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repos
```

<strong>Requisitos previos</strong>:  Ninguno


## bluemix plugin repo-add
{: #bluemix_plugin_repo_add}

Agrega un nuevo repositorio de plugin a {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repo-add REPO_NAME REPO_URL
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>REPO_NAME (necesario)</dt>
   <dd>Nombre del repositorio que se debe añadir. Puede volver a definir su propio nombre para cada repositorio.</dd>
   <dt>REPO_URL (necesario)</dt>
   <dd>URL del repositorio que se debe añadir. El URL de repositorio debe contener el protocolo (por ejemplo, http://plugins.ng.bluemix.net en lugar de plugins.ng.bluemix.net). http://plugins.ng.bluemix.net
es el repositorio de plugins oficial de Bluemix
CLI.</dd>
    </dl>


<strong>Ejemplos</strong>:

Añadir el repositorio de plugins oficial de Bluemix CLI como `bluemix-repo`:

```
bluemix plugin repo-add bluemix-repo http://plugins.ng.bluemix.net
```


## bluemix plugin repo-remove
{: #bluemix_plugin_repo_remove}

Elimina el repositorio de plugins de {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin repo-remove REPO_NAME
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:
   <dl>
   <dt>REPO_NAME (necesario)</dt>
   <dd>Nombre del repositorio que se debe eliminar.</dd>
   </dl>

<strong>Ejemplos</strong>:

Eliminar el repositorio `bluemix-repo` de {{site.data.keyword.Bluemix_notm}} CLI:

```
bluemix plugin repo-remove bluemix-repo
```


## bluemix plugin repo-plugins
{: #bluemix_plugin_repo_plugins}

Crea una lista de todos los plugins disponibles en todos los repositorios o repositorios específicos.

```
bluemix plugin repo-plugins [-r REPO_NAME]
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>Lista únicamente los plugins del repositorio indicado.</dd>
   </dl>

<strong>Ejemplos</strong>:

Crea una lista de todos los plugins en todos los repositorios añadidos:

```
bluemix plugin repo-plugins
```

Listar todos los plugins del repositorio `bluemix-repo`:

```
bluemix plugin repo-plugins -r bluemix-repo
```

## bluemix plugin repo-plugin
{: #bluemix_plugin_repo_plugin}

Mostrar los detalles de un plug-in del repositorio.

```
bluemix plugin repo-plugin PLUGIN_NAME [-r REPO_NAME]
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>Nombre del repositorio. Si no se especifica ningún repositorio, el mandato utilizará el repositorio de plug-in predeterminado.</dd>
   </dl>

<strong>Ejemplos</strong>:

Lista de detalles del plugin "IBM-Containers" en el repositorio "sample-repo":

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```

Lista de detalles del plugin "IBM-Containers" en el repositorio predeterminado

```
bluemix plugin repo-plugin IBM-Containers -r sample-repo
```


## bluemix plugin list
{: #bluemix_plugin_list}

Crea una lista de todos los plugins instalados en {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin list
```

<strong>Requisitos previos</strong>:  Ninguno

## bluemix plugin show
{: #bluemix_plugin_show}

Mostrar detalles de un plugin instalado

```
bluemix plugin show PLUGIN-NAME
```

<strong>Requisitos previos</strong>:  Ninguno


## bluemix plugin install
{: #bluemix_plugin_install}

Instalar la versión específica del plugin en {{site.data.keyword.Bluemix_notm}} CLI desde la vía de acceso o el repositorio especificados.

```
bluemix plugin install PLUGIN_PATH|PLUGIN_NAME [-r REPO_NAME] [-v VERSION]
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>PLUGIN_PATH|PLUGIN_NAME (necesario)</dt>
   <dd>Si -r <i>REPO_NAME</i> no se especifica, el plugin se instala desde la vía de acceso local o el URL remoto indicados.</dd>
   <dt>-r <i>REPO_NAME</i> (opcional)</dt>
   <dd>Nombre del repositorio en el que se encuentra el binario del plugin. Si no se especifica ningún repositorio, el mandato utilizará el repositorio de plug-in predeterminado.</dd>
   <dt>-v <i>VERSION</i> (opcional)</dt>
   <dd>Versión del plugin que se debe instalar. Si no se proporciona, se instalará la versión más reciente del plugin. Esta opción sólo es válida al instalar el plugin desde el repositorio.</dd>
    </dl>

<strong>Ejemplos</strong>:

Instala un plugin desde el archivo local:

```
bluemix plugin install /downloads/new_plugin
```

Instala un plugin desde el URL remoto:

```
bluemix plugin install http://plugins.ng.bluemix.net/downloads/new_plugin
```

Instala el plugin `IBM-Containers` de la versión más reciente del repositorio `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo
```
Instala el plugin `IBM-Containers` con la versión `0.5.800` del repositorio `bluemix-repo`:

```
bluemix plugin install IBM-Containers -r bluemix-repo -v 0.5.800
```

## bluemix plugin update
{: #bluemix_plugin_update}

Actualiza el plugin desde un repositorio

```
bluemix plugin update [PLUGIN NAME] [-r REPO_NAME] [-v VERSION] [--all]
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:
<dl>
 <dt>PLUGIN NAME</dt>
 <dd>Nombre del plug-in que se debe actualizar. Si no se especifica, el mandato comprobará las actualizaciones para todos los plug-ins instalados.</dd>
 <dt>-r REPO_NAME</dt>
 <dd>Nombre del repositorio en el que se encuentra el binario del plugin. Si no se especifica, el mandato utilizará el repositorio de plugins predeterminado.</dd>
 <dt>-v <i>VERSION</i> (opcional)</dt>
 <dd>Versión a la que se tiene que actualizar el plugin. Si no se proporciona, actualiza el plugin a la última versión disponible.</dd>
 <dt>--all</dt>
 <dd>Actualiza todos los plugins disponibles</dd>
</dl>

<strong>Ejemplos</strong>:

Comprueba todas las actualizaciones disponibles en el repositorio de plugins "My-Repo":

```
bluemix plugin update -r My-Repo
```

Actualiza el plugin "plugin-echo" en el repositorio "My-Repo" a la última versión:

```
bluemix plugin update -r My-Repo plugin-echo
```

Actualiza el plugin "plugin-echo" en el repositorio "My-Repo" a la versión "1.0.1":

```
bluemix plugin update -r My-Repo plugin-echo -v 1.0.1
```

## bluemix plugin uninstall
{: #bluemix_plugin_uninstall}

Desinstala el plugin especificado desde {{site.data.keyword.Bluemix_notm}} CLI.

```
bluemix plugin uninstall PLUGIN_NAME
```

<strong>Requisitos previos</strong>:  Ninguno

<strong>Opciones de mandato</strong>:

   <dl>
   <dt>PLUGIN_NAME (necesario)</dt>
   <dd>Nombre del plugin que se debe desinstalar.</dd>
    </dl>

<strong>Ejemplos</strong>:

Desinstala el plugin `IBM-Containers` que se ha instalado previamente:

```
bluemix plugin uninstall IBM-Containers
```

