---

copyright:

  years: 2016,2017

lastupdated: "2017-09-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Mandatos de {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl)
{: #softlayer_cli}

El plugin de {{site.data.keyword.BluSoftlayer}} se ha fusionado en la CLI de {{site.data.keyword.Bluemix_notm}}. Ya no necesita instalar el plugin.

Utilice los mandatos de {{site.data.keyword.BluSoftlayer_notm}} en la interfaz de línea de mandatos (CLI) de {{site.data.keyword.Bluemix_notm}} para configurar y gestionar los servicios de SoftLayer.


Para empezar, instale IBM {{site.data.keyword.Bluemix_notm}} CLI. Consulte
[CLI de Bluemix ![Icono de enlace externo](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window} para obtener más detalles.

Para obtener una lista completa de los mandatos de {{site.data.keyword.Bluemix_notm}}, consulte: [Mandatos de {{site.data.keyword.Bluemix_notm:}} (bx)](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)


## Mandatos de {{site.data.keyword.BluSoftlayer_notm}} generales

Se da soporte a los mandatos siguientes. Utilice el mandato `bluemix sl` para ver la lista de mandatos disponibles:

<table summary="Mandatos ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 1. Mandatos generales de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos generales Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## Mandatos de almacenamiento en bloque de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 2. Almacenamiento en bloque de Softlayer</caption>
 <thead>
 <th colspan="6">Almacenamiento en bloque de Softlayer</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix sl block access-authorize](/docs/cli/reference/softlayer/index.html#sl_block_access_authorize)</td>
  <td>[bluemix sl block access-list](/docs/cli/reference/softlayer/index.html#sl_block_access_list)</td>
  <td>[bluemix sl block access-revoke](/docs/cli/reference/softlayer/index.html#sl_block_access_revoke)</td>
  <td>[bluemix sl block replica-failback](/docs/cli/reference/softlayer/index.html#sl_block_replica_failback)</td>
  <td>[bluemix sl block replica-failover](/docs/cli/reference/softlayer/index.html#sl_block_replica_failover)</td>
  <td>[bluemix sl block replica-locations](/docs/cli/reference/softlayer/index.html#sl_block_replica_locations)</td>
   </tr>
 <tr>
  <td>[bluemix sl block replica-order](/docs/cli/reference/softlayer/index.html#sl_block_replica_order)</td>
  <td>[bluemix sl block replica-partners](/docs/cli/reference/softlayer/index.html#sl_block_replica_partners)</td>
  <td>[bluemix sl block snapshot-cancel](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_cancel)</td>
  <td>[bluemix sl block snapshot-create](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_create)</td>
  <td>[bluemix sl block snapshot-disable](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_disable)</td>
  <td>[bluemix sl block snapshot-enable](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_enable)</td>
  </tr>
 <tr>
  <td>[bluemix sl block snapshot-delete](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_delete)</td>
  <td>[bluemix sl block snapshot-list](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_list)</td>
  <td>[bluemix sl block snapshot-order](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_order)</td>
  <td>[bluemix sl block snapshot-restore](/docs/cli/reference/softlayer/index.html#sl_block_snapshot_restore)</td>
  <td>[bluemix sl block volume-cancel](/docs/cli/reference/softlayer/index.html#sl_block_volume_cancel)</td>  
  <td>[bluemix sl block volume-detail](/docs/cli/reference/softlayer/index.html#sl_block_volume_detail)</td>
   </tr>
 <tr>
   <td>[bluemix sl block volume-duplicate](/docs/cli/reference/softlayer/index.html#sl_block_volume_duplicate)</td>
   <td>[bluemix sl block volume-list](/docs/cli/reference/softlayer/index.html#sl_block_volume_list)</td>
   <td>[bluemix sl block volume-order](/docs/cli/reference/softlayer/index.html#sl_block_volume_order)</td>
   <td>[bluemix sl block volume-options](/docs/cli/reference/softlayer/index.html#sl_block_volume_options)</td>
 </tr>
   </tbody>
 </table>

 ## Mandatos CDN de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 3. CDN de Softlayer</caption>
 <thead>
 <th colspan="6">CDN de Softlayer</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix sl cdn cancel](/docs/cli/reference/softlayer/index.html#sl_cdn_cancel)</td>
  <td>[bluemix sl cdn detail](/docs/cli/reference/softlayer/index.html#sl_cdn_detail)</td>
  <td>[bluemix sl cdn list](/docs/cli/reference/softlayer/index.html#sl_cdn_list)</td>
  <td>[bluemix sl cdn load](/docs/cli/reference/softlayer/index.html#sl_cdn_load)</td>
  <td>[bluemix sl cdn order](/docs/cli/reference/softlayer/index.html#sl_cdn_order)</td>
  <td>[bluemix sl cdn options](/docs/cli/reference/softlayer/index.html#sl_cdn_options)</td>
   </tr>
 <tr>
  <td>[bluemix sl cdn origin-add](/docs/cli/reference/softlayer/index.html#sl_cdn_origin_add)</td>
  <td>[bluemix sl cdn origin-list](/docs/cli/reference/softlayer/index.html#sl_cdn_origin_list)</td>
  <td>[bluemix sl cdn origin-remove](/docs/cli/reference/softlayer/index.html#sl_cdn_origin_remove)</td>
  <td>[bluemix sl cdn purge](/docs/cli/reference/softlayer/index.html#sl_cdn_purge)</td>
  </tr>
   </tbody>
 </table>

## Mandatos de almacenamiento de archivos de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 4. Almacenamiento de archivos de Softlayer</caption>
 <thead>
 <th colspan="6">Almacenamiento de archivos de Softlayer</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix sl file access-authorize](/docs/cli/reference/softlayer/index.html#sl_file_access_authorize)</td>
  <td>[bluemix sl file access-list](/docs/cli/reference/softlayer/index.html#sl_file_access_list)</td>
  <td>[bluemix sl file access-revoke](/docs/cli/reference/softlayer/index.html#sl_file_access_revoke)</td>
  <td>[bluemix sl file replica-failback](/docs/cli/reference/softlayer/index.html#sl_file_replica_failback)</td>
  <td>[bluemix sl file replica-failover](/docs/cli/reference/softlayer/index.html#sl_file_replica_failover)</td>
  <td>[bluemix sl file replica-locations](/docs/cli/reference/softlayer/index.html#sl_file_replica_locations)</td>
   </tr>
 <tr>
  <td>[bluemix sl file replica-order](/docs/cli/reference/softlayer/index.html#sl_file_replica_order)</td>
  <td>[bluemix sl file replica-partners](/docs/cli/reference/softlayer/index.html#sl_file_replica_partners)</td>
  <td>[bluemix sl file snapshot-cancel](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_cancel)</td>
  <td>[bluemix sl file snapshot-create](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_create)</td>
  <td>[bluemix sl file snapshot-disable](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_disable)</td>
  <td>[bluemix sl file snapshot-enable](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_enable)</td>
  </tr>
 <tr>
  <td>[bluemix sl file snapshot-delete](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_delete)</td>
  <td>[bluemix sl file snapshot-list](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_list)</td>
  <td>[bluemix sl file snapshot-order](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_order)</td>
  <td>[bluemix sl file snapshot-restore](/docs/cli/reference/softlayer/index.html#sl_file_snapshot_restore)</td>
  <td>[bluemix sl file volume-cancel](/docs/cli/reference/softlayer/index.html#sl_file_volume_cancel)</td>  
  <td>[bluemix sl file volume-detail](/docs/cli/reference/softlayer/index.html#sl_file_volume_detail)</td>
   </tr>
 <tr>
   <td>[bluemix sl file volume-duplicate](/docs/cli/reference/softlayer/index.html#sl_file_volume_duplicate</td>
   <td>[bluemix sl file volume-list](/docs/cli/reference/softlayer/index.html#sl_file_volume_list)</td>
   <td>[bluemix sl file volume-order](/docs/cli/reference/softlayer/index.html#sl_file_volume_order)</td>
   <td>[bluemix sl file volume-options](/docs/cli/reference/softlayer/index.html#sl_file_volume_options)</td>
 </tr>
   </tbody>
 </table>

## Mandatos DNS de {{site.data.keyword.BluSoftlayer_notm}}

<table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 5. Mandatos DNS de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos DNS de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl dns import](/docs/cli/reference/softlayer/index.html#sl_dns_import)</td>
 <td>[bluemix sl dns record-add](/docs/cli/reference/softlayer/index.html#sl_dns_record_add)</td>
 <td>[bluemix sl dns record-edit](/docs/cli/reference/softlayer/index.html#sl_dns_record_edit)</td>
 <td>[bluemix sl dns record-list](/docs/cli/reference/softlayer/index.html#sl_dns_record_list)</td>
 <td>[bluemix sl dns record-remove](/docs/cli/reference/softlayer/index.html#sl_dns_record_remove)</td>
 <td>[bluemix sl dns zone-create](/docs/cli/reference/softlayer/index.html#sl_dns_zone_create)</td>
 </tr>
 <tr>
   <td>[bluemix sl dns zone-delete](/docs/cli/reference/softlayer/index.html#sl_dns_zone_delete)</td>
   <td>[bluemix sl dns zone-list](/docs/cli/reference/softlayer/index.html#sl_dns_zone_list)</td>
   <td>[bluemix sl dns zone-print](/docs/cli/reference/softlayer/index.html#sl_dns_zone_print)</td>
 </tr>
   </tbody>
 </table>

<table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 6. Mandatos de IP de Softlayer Global</caption>
 <thead>
 <th colspan="6">Mandatos de IP de Softlayer Global</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix sl globalip assign](/docs/cli/reference/softlayer/index.html#sl_globalip_assign)</td>
  <td>[bluemix sl globalip cancel](/docs/cli/reference/softlayer/index.html#sl_globalip_cancel)</td>
  <td>[bluemix sl globalip create](/docs/cli/reference/softlayer/index.html#sl_globalip_create)</td>
 <td>[bluemix sl globalip list](/docs/cli/reference/softlayer/index.html#sl_globalip_list)</td>
 <td>[bluemix sl globalip unassign](/docs/cli/reference/softlayer/index.html#sl_globalip_cancel)</td>
 </tr>
   </tbody>
 </table>

## Mandatos image de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 7. Mandatos image de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos image de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl image delete](/docs/cli/reference/softlayer/index.html#sl_image_delete)</td>
 <td>[bluemix sl image detail](/docs/cli/reference/softlayer/index.html#sl_image_detail)</td>
 <td>[bluemix sl image edit](/docs/cli/reference/softlayer/index.html#sl_image_edit)</td>
 <td>[bluemix sl image list](/docs/cli/reference/softlayer/index.html#sl_image_list)</td>
 </tr>
   </tbody>
 </table>
 
 ## Mandatos VPN de IPSec de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 7. Mandatos VPN de IPSec de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos VPN de IPSec de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl ipsec cancel](/docs/cli/reference/softlayer/index.html#sl_ipsec_cancel)</td>
 <td>[bluemix sl ipsec config](/docs/cli/reference/softlayer/index.html#sl_ipsec_config)</td>
 <td>[bluemix sl ipsec detail](/docs/cli/reference/softlayer/index.html#sl_ipsec_detail)</td>
 <td>[bluemix sl ipsec list](/docs/cli/reference/softlayer/index.html#sl_ipsec_list)</td>
 <td>[bluemix sl ipsec order](/docs/cli/reference/softlayer/index.html#sl_ipsec_order)</td>
 <td>[bluemix sl ipsec subnet-add](/docs/cli/reference/softlayer/index.html#sl_ipsec_subnet_add)</td>
 </tr>
 <tr>
 <td>[bluemix sl ipsec subnet-remove](/docs/cli/reference/softlayer/index.html#sl_ipsec_subnet_remove)</td>
 <td>[bluemix sl ipsec translation-add](/docs/cli/reference/softlayer/index.html#sl_ipsec_translation_add)</td>
 <td>[bluemix sl ipsec translation-remove](/docs/cli/reference/softlayer/index.html#sl_ipsec_translation_remove)</td>
 <td>[bluemix sl ipsec translation-update](/docs/cli/reference/softlayer/index.html#sl_ipsec_translation_update)</td>
 <td>[bluemix sl ipsec update](/docs/cli/reference/softlayer/index.html#sl_ipsec_update)</td>
 </tr>
   </tbody>
 </table>

 ## Mandatos Load Balancer de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 8. Mandatos Load Balancer de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos Load Balancer de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl loadbal cancel](/docs/cli/reference/softlayer/index.html#sl_loadbal_cancel)</td>
 <td>[bluemix sl loadbal create](/docs/cli/reference/softlayer/index.html#sl_loadbal_create)</td>
 <td>[bluemix sl loadbal create-options](/docs/cli/reference/softlayer/index.html#sl_loadbal_create_options)</td>
 <td>[bluemix sl loadbal detail](/docs/cli/reference/softlayer/index.html#sl_loadbal_detail)</td>
 <td>[bluemix sl loadbal group-add](/docs/cli/reference/softlayer/index.html#sl_loadbal_group_add)</td>
 <td>[bluemix sl loadbal group-delete](/docs/cli/reference/softlayer/index.html#sl_loadbal_group_delete)</td>
 </tr>
 <tr>
 <td>[bluemix sl loadbal group-edit](/docs/cli/reference/softlayer/index.html#sl_loadbal_group_edit)</td>
 <td>[bluemix sl loadbal group-reset](/docs/cli/reference/softlayer/index.html#sl_loadbal_group_reset)</td>
 <td>[bluemix sl loadbal health-checks](/docs/cli/reference/softlayer/index.html#sl_loadbal_health_checks)</td>
 <td>[bluemix sl loadbal list](/docs/cli/reference/softlayer/index.html#sl_loadbal_list)</td>
 <td>[bluemix sl loadbal routing-methods](/docs/cli/reference/softlayer/index.html#sl_loadbal_routing_methods)</td>
 <td>[bluemix sl loadbal routing-types](/docs/cli/reference/softlayer/index.html#sl_loadbal_routing_types)</td>
 </tr>
 <tr>
 <td>[bluemix sl loadbal service-add](/docs/cli/reference/softlayer/index.html#sl_loadbal_service_add)</td>
 <td>[bluemix sl loadbal service-delete](/docs/cli/reference/softlayer/index.html#sl_loadbal_service_delete)</td>
 <td>[bluemix sl loadbal service-edit](/docs/cli/reference/softlayer/index.html#sl_loadbal_service_edit)</td>
 <td>[bluemix sl loadbal service-toggle](/docs/cli/reference/softlayer/index.html#sl_loadbal_service_toggle)</td>
 </tr>
</tbody>
 </table>

## Mandatos security de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 9. Mandatos security de Softlayer</caption>
 <thead>
 <th colspan="5">Mandatos security de Softlayer</th>
 </thead>
 <tbody>
 <tr>
  <td>[bluemix sl security sshkey-add](/docs/cli/reference/softlayer/index.html#sl_security_sshkey_add)</td>
  <td>[bluemix sl security sshkey-edit](/docs/cli/reference/softlayer/index.html#sl_security_sshkey_edit)</td>
  <td>[bluemix sl security sshkey-list](/docs/cli/reference/softlayer/index.html#sl_security_sshkey_list)</td>
  <td>[bluemix sl security sshkey-print](/docs/cli/reference/softlayer/index.html#sl_security_sshkey_print)</td>   
  <td>[bluemix sl security sshkey-remove](/docs/cli/reference/softlayer/index.html#sl_security_sshkey_remove)</td>
 </tr>
 <tr>
  <td>[bluemix sl security cert-add](/docs/cli/reference/softlayer/index.html#sl_security_cert_add)</td>
  <td>[bluemix sl security cert-edit](/docs/cli/reference/softlayer/index.html#sl_security_cert_edit)</td>
  <td>[bluemix sl security cert-download](/docs/cli/reference/softlayer/index.html#sl_security_cert_download)</td>
  <td>[bluemix sl security cert-list](/docs/cli/reference/softlayer/index.html#sl_security_cert_list)</td>
  <td>[bluemix sl security cert-remove](/docs/cli/reference/softlayer/index.html#sl_security_cert_remove)</td>
 </tr>
   </tbody>
 </table>

## Mandatos subnet de {{site.data.keyword.BluSoftlayer_notm}}
 
 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 10. Mandatos subnet de Softlayer</caption>
 <thead>
 <th colspan="5">Mandatos subnet de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl subnet cancel](/docs/cli/reference/softlayer/index.html#sl_subnet_cancel)</td>
 <td>[bluemix sl subnet create](/docs/cli/reference/softlayer/index.html#sl_subnet_create)</td>
 <td>[bluemix sl subnet detail](/docs/cli/reference/softlayer/index.html#sl_subnet_detail)</td>
 <td>[bluemix sl subnet list](/docs/cli/reference/softlayer/index.html#sl_subnet_list)</td>
 <td>[bluemix sl subnet lookup](/docs/cli/reference/softlayer/index.html#sl_subnet_lookup)</td>
 </tr>
   </tbody>
 </table>
 
## Mandatos de servidor virtual de {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 11. Mandatos de servidor virtual de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos de servidor virtual de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl vs cancel](/docs/cli/reference/softlayer/index.html#sl_vs_cancel)</td>
 <td>[bluemix sl vs capture](/docs/cli/reference/softlayer/index.html#sl_vs_capture)</td>
 <td>[bluemix sl vs create](/docs/cli/reference/softlayer/index.html#sl_vs_create)</td>
 <td>[bluemix sl vs options](/docs/cli/reference/softlayer/index.html#sl_vs_options)</td>
 <td>[bluemix sl vs credentials](/docs/cli/reference/softlayer/index.html#sl_vs_credentials)</td>
 <td>[bluemix sl vs detail](/docs/cli/reference/softlayer/index.html#sl_vs_detail)</td>
 </tr><tr>
 <td>[bluemix sl vs dns-sync](/docs/cli/reference/softlayer/index.html#sl_vs_dns_sync)</td>
 <td>[bluemix sl vs edit](/docs/cli/reference/softlayer/index.html#sl_vs_edit)</td>
 <td>[bluemix sl vs list](/docs/cli/reference/softlayer/index.html#sl_vs_list)</td>
 <td>[bluemix sl vs pause](/docs/cli/reference/softlayer/index.html#sl_vs_pause)</td>
 <td>[bluemix sl vs power-off](/docs/cli/reference/softlayer/index.html#sl_vs_power_off)</td>
 <td>[bluemix sl vs power-on](/docs/cli/reference/softlayer/index.html#sl_vs_power_on)
 </tr><tr>
 <td>[bluemix sl vs ready](/docs/cli/reference/softlayer/index.html#sl_vs_ready)</td>
 <td>[bluemix sl vs reboot](/docs/cli/reference/softlayer/index.html#sl_vs_reboot)</td>
 <td>[bluemix sl vs reload](/docs/cli/reference/softlayer/index.html#sl_vs_reload)</td>
 <td>[bluemix sl vs rescure](/docs/cli/reference/softlayer/index.html#sl_vs_rescure)</td>
 <td>[bluemix sl vs resume](/docs/cli/reference/softlayer/index.html#sl_vs_resume)</td>
 <td>[bluemix sl vs upgrade](/docs/cli/reference/softlayer/index.html#sl_vs_upgrade)</td>
 </tr>
   </tbody>
 </table>
 
## Mandatos VLAN de {{site.data.keyword.BluSoftlayer_notm}}

  <table summary="Mandatos de Softlayer generales ordenados alfabéticamente que tienen enlaces que le proporcionan más información del mandato">
<caption>Tabla 12. Mandatos VLAN de Softlayer</caption>
 <thead>
 <th colspan="6">Mandatos VLAN de Softlayer</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl vlan create](/docs/cli/reference/softlayer/index.html#sl_vlan_create)</td>
 <td>[bluemix sl vlan cancel](/docs/cli/reference/softlayer/index.html#sl_vlan_cancel)</td>
 <td>[bluemix sl vlan detail](/docs/cli/reference/softlayer/index.html#sl_vlan_detail)</td>
 <td>[bluemix sl vlan edit](/docs/cli/reference/softlayer/index.html#sl_vlan_edite)</td>
 <td>[bluemix sl vlan list](/docs/cli/reference/softlayer/index.html#sl_vlan_list)</td>
 <td>[bluemix sl vlan options](/docs/cli/reference/softlayer/index.html#sl_vlan_options)</td>
 </tr>
   </tbody>
 </table>

### Utilización del mandato
Para ver la información de ayuda de los mandatos, ejecute: `bluemix sl [command] -h`.

### bluemix sl init
{: #sl_init}

Inicialice los valores de configuración que se utilizan para conectarse al entorno de SoftLayer. La configuración incluye nombre de usuario, contraseña o una clave de API, cuenta y punto final.
```
bluemix sl init [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-a, --api-endpoint</dt>
<dd>URL de punto final de la API de Softlayer, el valor predeterminado es: https://api.softlayer.com/rest/v3.1 para la autenticación de claves de API de Softlayer, https://api.softlayer.com/mobile/v3.1 para la autenticación del ID de IBM.</dd>
<dt>-u, --sl-user</dt>
<dd>Nombre de usuario de Softlayer.</dd>
<dt>-p, --sl-password</dt>
<dd>Contraseña de Softlayer o clave de API.</dd>
<dt>-c, --account-id</dt>
<dd>ID de cuenta de Softlayer.</dd>
<dt>-q, --security-question-id</dt>
<dd>ID de pregunta de seguridad utilizado para autenticar. Pregunte al propietario de la cuenta si no lo conoce.</dd>
<dt>-w, --security-question-answer</dt>
<dd>Respuesta a la pregunta de seguridad utilizada para autenticar. Pregunte al propietario de la cuenta si no la conoce.</dd>
<dt>-s, --security-code</dt>
<dd>Código de seguridad generado por el proveedor de seguridad cuando está habilitada la autenticación de 2 factores.</dd>
<dt>-v, --security-vendor</dt>
<dd>Proveedor de seguridad que proporciona código de seguridad para la autenticación. Las opciones son: VERISIGN,TOTP,PHONE_FACTOR.</dd>
<dt>-t, --auth-token</dt>
<dd>Señal de autenticación cuando se habilita la autenticación telefónica.</dd>
</dl>

Por ejemplo, inicie la sesión con nombre de usuario y contraseña/clave de API de Softlayer
```
$ bluemix sl config
Elija cómo configurar la autenticación de Softlayer:
1. Iniciar sesión con nombre de usuario y contraseña/clave de API de Softlayer
2. Utilizar inicio de sesión único de Bluemix
Escriba un número>1
URL de punto final de API de Softlayer: [https://api.softlayer.com/rest/v3.1]>
Nombre de usuario: []> wangjunl@cn.ibm.com
Clave de API o contraseña: []> abcd

Punto final de API de Softlayer: https://api.softlayer.com/rest/v3.1
ID de cuenta:                    278444
ID de usuario:                   wangjunl@cn.ibm.com
Clave de API:                    xxxxxxxxxx
```
Por ejemplo, utilice el inicio de sesión único de Bluemix para iniciar la sesión en Softlayer
```
$ bx login -a api.ng.bluemix.net -u wangjunl@cn.ibm.com -p xxxxxxx -c 65ce8074c6c62b5
Punto final de la API: api.ng.bluemix.net
Autenticando...
Correcto

Cuenta de destino Wilma's Account (65ce8074c6c62b5)
                  
Punto final de la API:   https://api.ng.bluemix.net (Versión de la API: 2.54.0)   
Región:                  us-south
Usuario:                 wangjunl@cn.ibm.com
Cuenta:                  Wilma's Account (65ce8074c6c62b5)   
Ninguna organización ni espacio de destino. Utilice 'bx target --cf or bx target -o ORG -s SPACE'

Sugerencia: Utilice 'bx cf <command>' para ejecutar la CLI de Cloud Foundry con el contexto de CLI de Bluemix.
```

$ bx sl init
Elija cómo configurar la autenticación Softlayer: 
1. Iniciar sesión con nombre de usuario y contraseña/clave de API de Softlayer
2. Utilizar inicio de sesión único de Bluemix
Escriba un número>2
URL de punto final de API de Softlayer: [https://api.softlayer.com/mobile/v3.1]> 
Estableciendo la cuenta en: 278444
Correcto
                              
Punto final de API de Softlayer:    https://api.softlayer.com/mobile/v3.1   
ID de cuenta:                278444   
ID de usuario:                   12345678   
Señal de IMS:                 xxxxxxxxxx
```

### bluemix sl help
{: #sl_help}

Vea la información de ayuda para que todos los mandatos operen en el entorno de Softlayer.
```
bluemix sl help

```

### bluemix sl block access-authorize
{: #sl_block_access_authorize}

Autorice a los hosts a acceder a un volumen determinado.
```
bluemix sl block access-authorize VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>El ID de un servidor hardware para autorizar.</dd>
<dt>-v, --virtual-id</dt>
<dd>El ID de un servidor virtual para autorizar.</dd>
<dt>-i, --ip-address-id</dt>
<dd>El ID de una dirección IP para autorizar.</dd>
<dt>-p, --ip-address</dt>
<dd>Una dirección IP para autorizar.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
Este mandato autoriza al servidor virtual con el ID 87654321 a acceder al volumen con el ID 12345678.

### bluemix sl block access-list
{: #sl_block_access_list}

Lista de ACL.
```
bluemix sl block access-list VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que ordenar. Las opciones son: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Columnas a visualizar. Las opciones son: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block access-list 12345678 --sortby id
```
Este mandato lista todos los hosts que están autorizados para acceder al volumen con el ID 12345678 y los ordena por ID.

### bluemix sl block access-revoke
{: #sl_block_access_revoke}

Revocar la autorización para los hosts que acceden a un volumen determinado.
```
bluemix sl block access-revoke VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>El ID de un servidor hardware a revocar.</dd>
<dt>-v, --virtual-id</dt>
<dd>El ID de un servidor virtual a revocar.</dd>
<dt>-i, --ip-address-id</dt>
<dd>El ID de una dirección IP a revocar.</dd>
<dt>-p, --ip-address</dt>
<dd>Una dirección IP a revocar.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
Este mandato revoca el acceso del servidor virtual con el ID 87654321 al volumen con el ID 12345678.

### bluemix sl block replica-failback
{: #sl_block_replica_failback}

Restablecimiento de un volumen de bloque de la réplica.
```
bluemix sl block replica-failback VOLUME_ID
```


**Ejemplos**:
```
bluemix sl block replica-failback 12345678
```
Este mandato realiza la operación de restablecimiento para el volumen con el ID 12345678.

### bluemix sl block replica-failover
{: #sl_block_replica_failover}

Migración tras error de un volumen de bloque al volumen de réplica determinado.
```
bluemix sl block replica-failover VOLUME_ID REPLICA_ID
```


**Ejemplos**:
```
bluemix sl block replica-failover 12345678 87654321
```
Este mandato realiza la operación de migración tras error para el volumen con el ID 12345678 al volumen de réplica con el ID 87654321.

### bluemix sl block replica-locations
{: #sl_block_replica_locations}

Lista de centros de datos de réplica adecuados para el volumen determinado.
```
bluemix sl block replica-locations VOLUME_ID
```


**Ejemplos**:
```
bluemix sl block replica-locations 12345678
```
Este mandato lista los centros de datos de réplica adecuados para el volumen de bloque con el ID 12345678.

### bluemix sl block replica-order
{: #sl_block_replica_order}

Pida un volumen de réplica de almacenamiento en bloque.
```
bluemix sl block replica-order VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Obligatorio. Planificación de instantáneas para utilizar para la réplica. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos para la réplica, p. ej. dal09.</dd>
<dt>-t, --tier</dt>
<dd>Opcional. Nivel de almacenamiento resistente (IOPS por GB) del volumen primario para el cual se solicita una réplica. Las opciones son: 0,25, 2, 4, 10. Si no se especifica el nivel, se utilizará el nivel del volumen original.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100. Si no se especifica IOPS, se utilizará el IOPS del volumen original.</dd>
<dt>-o, --os-type</dt>
<dd>Opcional. Tipo de sistema operativo (p. ej. LINUX) del volumen primario para el que se pide una réplica. Las opciones son: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
Este mandato solicita una réplica para el volumen con el ID 12345678, que realiza una réplica DIARIA, está ubicado en dal09, el nivel de grados es 4, el tipo de SO es Linux.

### bluemix sl block replica-partners
{: #sl_block_replica_partners}

Lista de volúmenes existentes replicantes para un volumen de bloque.
```
bluemix sl block replica-partners VOLUME_ID [OPTIONS]
```


**Ejemplos**:
```
bluemix sl block replica-partners 12345678
```
Este mandato lista los volúmenes replicantes existentes para el volumen de bloque con el ID 12345678.

### bluemix sl block snapshot-cancel
{: #sl_block_snapshot_cancel}

Cancelar el espacio de instantáneas existente para un volumen determinado.
```
bluemix sl block snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--reason</dt>
<dd>Una razón opcional para la cancelación.</dd>
<dt>--immediate</dt>
<dd>Cancelar el espacio de instantáneas inmediatamente, en lugar de en el aniversario de facturación.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-cancel 12345678 --immediate -f
```
Este mandato cancela la instantánea con el ID 12345678 inmediatamente sin pedir confirmación.

### bluemix sl block snapshot-create
{: #sl_block_snapshot_create}

Crear una instantánea en un volumen determinado.
```
bluemix sl block snapshot-create VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Notas para establecer en la nueva instantánea.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
Este mandato crea una instantánea para el volumen con el ID 12345678 y con una nota de adición como snapshotforbluemix.

### bluemix sl block snapshot-disable
{: #sl_block_snapshot_disable}

Inhabilitar instantáneas en la planificación especificada para un volumen determinado.
```
bluemix sl block snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obligatorio. Planificación de instantáneas. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-disable 12345678 -s DAILY
```
Este mandato inhabilita la instantánea diaria para el volumen con el ID 12345678.

### bluemix sl block snapshot-enable
{: #sl_block_snapshot_enable}

Habilitar instantáneas para un volumen determinado en la planificación especificada.
```
bluemix sl block snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obligatorio. Planificación de instantáneas. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Obligatorio. Número de instantáneas que se deben retener.</dd>
<dt>-m, --minute</dt>
<dd>Minuto de la hora en el que deben tomarse las instantáneas, entero entre 0 y 59-</dd>
<dt>-r, --hour</dt>
<dd>Hora del día en la que deben tomarse las instantáneas, número entero entre 0 y 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Día de la semana en que deben tomarse las instantáneas, número entero entre 0 y 6. 0 significa domingo, 1 significa lunes, 2 significa martes, 3 significa miércoles, 4 significa jueves, 5 significa viernes, 6 significa sábado.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
Este mandato habilita la instantánea para el volumen con el ID 12345678. La instantánea se toma semanalmente cada domingo a las 2:00, y se retienen hasta 5 instantáneas.

### bluemix sl block snapshot-delete
{: #sl_block_snapshot_delete}

Suprimir una instantánea en un volumen determinado.
```
bluemix sl block snapshot-delete SNAPSHOT_ID
```


**Ejemplos**:
```
bluemix sl block snapshot-delete 12345678
```
Este mandato suprime la instantánea con el ID 12345678.

### bluemix sl block snapshot-list
{: #sl_block_snapshot_list}

Lista de instantáneas de almacenamiento en bloque.
```
bluemix sl block snapshot-list VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que se debe ordenar. Las opciones son: id,name,created,size_bytes.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-list 12345678 --sortby id
```
Este mandato lista todas las instantáneas de volumen con el ID 12345678 y las ordena por ID.

### bluemix sl block snapshot-order
{: #sl_block_snapshot_order}

Solicitar espacio de instantáneas para un volumen de almacenamiento en bloques.
```
bluemix sl block snapshot-order VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Obligatorio. Tamaño del espacio de instantáneas para crear en GB.</dd>
<dt>-t, --tier</dt>
<dd>Opcional. Nivel de almacenamiento resistente (IOPS por GB) del volumen de bloques para el cual se solicita el espacio. Las opciones son: 0,25, 2, 4, 10.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Distintivo para indicar que el pedido es una actualización.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
Este mandato solicita espacio de instantáneas para el volumen con el ID 12345678, el tamaño es de 1000 GB, el nivel de grados es de 4 IOPS por GB.

### bluemix sl block snapshot-restore
{: #sl_block_snapshot_restore}

Restaurar volumen de bloque mediante una instantánea determinada.
```
bluemix sl block snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**Ejemplos**:
```
bluemix sl block snapshot-restore 12345678 87654321
```
Este mandato restaura el volumen con el ID 12345678 a partir de la instantánea con el ID 87654321.

### bluemix sl block volume-cancel
{: #sl_block_volume_cancel}

Cancelar un volumen de almacenamiento en bloques existente.
```
bluemix sl block volume-cancel VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--reason</dt>
<dd>Una razón opcional para la cancelación.</dd>
<dt>--immediate</dt>
<dd>Cancelar el volumen de almacenamiento en bloques inmediatamente en lugar de en el aniversario de facturación.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block volume-cancel 12345678 --immediate -f
```
Este mandato cancela el volumen con el ID 12345678 inmediatamente y sin solicitar confirmación.

### bluemix sl block volume-list
{: #sl_block_volume_list}

Lista de almacenamiento en bloque.
```
bluemix sl block volume-list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filtrar por nombre de usuario del volumen.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtrar por nombre abreviado de centro de datos.</dd>
<dt>-t, --storage-type</dt>
<dd>Filtrar por tipo de volumen de almacenamiento. Las opciones son: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filtrar por ID del pedido que ha comprado el almacenamiento en bloque.</dd>
<dt>--sortby</dt>
<dd>Columna para ordenar por las siguientes opciones: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, active_transactions, created_by.</dd>
<dt>--columns</dt>
<dd>Columnas por visualizar, las opciones son: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, created_by.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
Este mandato lista todos los volúmenes de resistencia en la cuenta actual que están ubicados en dal09, y los ordena por capacidad.

### bluemix sl block volume-detail
{: #sl_block_volume_detail}

Mostrar detalles para un volumen especificado.
```
bluemix sl block volume-detail VOLUME_ID
```


**Ejemplos**:
```
bluemix sl block volume-detail 12345678
```
Este mandato muestra detalles de volumen con el ID 12345678.

### bluemix sl block volume-duplicate
{: #sl_block_volume_duplicate}

Solicitar un volumen de bloque duplicando uno existente.
```
bluemix sl block volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID de una instantánea de volumen de origen a utilizar para la duplicación.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Tamaño de volumen de bloque duplicado en GB. Si no se especifica ningún tamaño, se utilizará el tamaño del volumen original.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>IOPS de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100. Si no se especifica IOPS, se utilizará el IOPS del volumen original.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Nivel de almacenamiento resistente. Si no se especifica ningún tamaño, se utilizará el nivel del volumen original.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>El tamaño de espacio de instantáneas para solicitar el duplicado. Si no se especifica ningún tamaño de espacio de instantáneas, se utilizará el tamaño de espacio de instantáneas del volumen de origen.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block volume-duplicate 12345678
```
Este mandato muestra la solicitud de un volumen nuevo duplicando el volumen con el ID 12345678.

### bluemix sl block volume-order
{: #sl_block_volume_order}

Solicitar un volumen de almacenamiento en bloques.
```
bluemix sl block volume-order [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Obligatorio. Tipo de volumen de almacenamiento. Las opciones son: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Obligatorio. Tamaño de volumen de almacenamiento en GB.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100 [obligatorio para el rendimiento de tipo de almacenamiento].</dd>
<dt>-e, --tier</dt>
<dd>Nivel de almacenamiento resistente (IOP por GB) [obligatorio para la resistencia de tipo de almacenamiento]. Las opciones son: 0,25, 2, 4, 10.</dd>
<dt>-o, --os-type</dt>
<dd>Obligatorio. Sistema operativo. Las opciones son: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos.</dd>
<dt>-n, --snapshot-size</dt>
<dd>Parámetro opcional para solicitar espacio de instantáneas junto con almacenamiento en bloque de resistencia; especifica el tamaño (en GB) del espacio de instantáneas que se debe solicitar.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
Este mandato solicita un volumen de rendimiento cuyo tamaño es 1000 GB, IOPS es 4000, el tipo de sistema operativo es LINUX, ubicado en dal09.

### bluemix sl block volume-options
{: #sl_block_volume_options}

Listar todas las opciones para solicitar un almacenamiento en bloque.
```
bluemix sl block volume-options
```


**Ejemplos**:
```
bluemix sl block volume-options
```
Este mandato lista todas las opciones para crear un volumen de almacenamiento en bloques, incluyendo el tipo de almacenamiento, el tamaño de volumen, el tipo de sistema operativo, IOPS, nivel de grados, centro de datos y tamaño de instantánea.

### bluemix sl cdn cancel
{: #sl_cdn_cancel}

Cancelar una cuenta CDN.
```
bluemix sl cdn cancel ACCOUNT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>
### bluemix sl cdn detail
{: #sl_cdn_detail}

Detalle de una cuenta CDN.
```
bluemix sl cdn detail ACCOUNT_ID
```

### bluemix sl cdn list
{: #sl_cdn_list}

Listar todas las cuentas CDN.
```
bluemix sl cdn list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que ordenar. Las opciones son: id, name, type, created.</dd>
<dt>--order</dt>
<dd>Filtrar por ID de pedido.</dd>
</dl>
### bluemix sl cdn load
{: #sl_cdn_load}

Almacenar en la memoria caché uno o más archivos en todos los nodos extremos.
```
bluemix sl cdn load ACCOUNT_ID CONTENT_URL [CONTENT_URL...]
```

### bluemix sl cdn order
{: #sl_cdn_order}

Solicitar una cuenta CDN.
```
bluemix sl cdn order [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-b, --bandwidth</dt>
<dd>Ancho de banda de CDN, si no se especifica se utilizará el precio de 'Pago según uso'.</dd>
<dt>-s, --storage</dt>
<dd>Almacenamiento de CDN, si no se especifica se utilizará el precio de 'Pago según uso'.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>
### bluemix sl cdn options
{: #sl_cdn_options}

Opciones de ancho de banda y almacenamiento para solicitar una cuenta CDN.
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add
{: #sl_cdn_origin_add}

Crear una correlación de extracción origen.
```
bluemix sl cdn origin-add ACCOUNT_ID CONTENT_URL [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-t, --type</dt>
<dd>El tipo de soporte para esta correlación (http, flash, wm, ...). El valor predeterminado es: http.</dd>
<dt>-c, --cname</dt>
<dd>Un CNAME opcional para adjuntar a la correlación.</dd>
</dl>
### bluemix sl cdn origin-list
{: #sl_cdn_origin_list}

Listar correlaciones de extracción de origen.
```
bluemix sl cdn origin-list ACCOUNT_ID
```

### bluemix sl cdn origin-remove
{: #sl_cdn_origin_remove}

Eliminar una correlación de extracción origen.
```
bluemix sl cdn origin-remove ACCOUNT_ID ORIGIN_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>
### bluemix sl cdn purge
{: #sl_cdn_purge}

Depurar archivos de memoria caché de todos los nodos extremos.
```
bluemix sl cdn purge ACCOUNT_ID CONTENT_URL [CONTENT_URL...][OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>
### bluemix sl file access-authorize
{: #sl_file_access_authorize}

Autorizar que los hosts accedan a un volumen determinado.
```
bluemix sl file access-authorize VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>El ID de un servidor hardware para autorizar.</dd>
<dt>-v, --virtual-id</dt>
<dd>El ID de un servidor virtual para autorizar.</dd>
<dt>-i, --ip-address-id</dt>
<dd>El ID de una dirección IP para autorizar.</dd>
<dt>-p, --ip-address</dt>
<dd>Una dirección IP para autorizar.</dd>
<dt>-s, --subnet-id</dt>
<dd>ID de una subred que se va a autorizar.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
Este mandato autoriza al servidor virtual con el ID 87654321 a acceder al volumen con el ID 12345678.

### bluemix sl file access-list
{: #sl_file_access_list}

Listar ACL.
```
bluemix sl file access-list VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que ordenar. Las opciones son: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Columnas a visualizar. Las opciones son: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file access-list 12345678 --sortby id
```
Este mandato lista todos los hosts que están autorizados para acceder al volumen con el ID 12345678 y los ordena por ID.

### bluemix sl file access-revoke
{: #sl_file_access_revoke}

Revocar autorización para hosts que acceden a un volumen determinado.
```
bluemix sl file access-revoke VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>El ID de un servidor hardware a revocar.</dd>
<dt>-v, --virtual-id</dt>
<dd>El ID de un servidor virtual a revocar.</dd>
<dt>-i, --ip-address-id</dt>
<dd>El ID de una dirección IP a revocar.</dd>
<dt>-p, --ip-address</dt>
<dd>Una dirección IP a revocar.</dd>
<dt>-s, --subnet-id</dt>
<dd>ID de una subred que se va a revocar.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
Este mandato revoca el acceso del servidor virtual con el ID 87654321 al volumen con el ID 12345678.

### bluemix sl file replica-failback
{: #sl_file_replica_failback}

Restablecimiento de un volumen de archivo a partir de una réplica.
```
bluemix sl file replica-failback VOLUME_ID
```


**Ejemplos**:
```
bluemix sl file replica-failback 12345678
```
Este mandato realiza la operación de restablecimiento para el volumen con el ID 12345678.

### bluemix sl file replica-failover
{: #sl_file_replica_failover}

Migración tras error de un volumen de archivo a un volumen de réplica determinado.
```
bluemix sl file replica-failover VOLUME_ID REPLICA_ID
```


**Ejemplos**:
```
bluemix sl file replica-failover 12345678 87654321
```
Este mandato realiza la operación de migración tras error para el volumen con el ID 12345678 al volumen de réplica con el ID 87654321.

### bluemix sl file replica-locations
{: #sl_file_replica_locations}

Listar centros de datos de réplicas adecuados para el volumen indicado.
```
bluemix sl file replica-locations VOLUME_ID
```


**Ejemplos**:
```
bluemix sl file replica-locations 12345678
```
Este mandato lista centros de datos de réplicas adecuados para el volumen de archivo con el ID 12345678.

### bluemix sl file replica-order
{: #sl_file_replica_order}

Solicitar un volumen de réplica de almacenamiento en archivo.
```
bluemix sl file replica-order VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Obligatorio. Planificación de instantáneas para utilizar para la réplica. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos para la réplica, p. ej. dal09.</dd>
<dt>-t, --tier</dt>
<dd>Opcional. Nivel de almacenamiento resistente (IOPS por GB) del volumen primario para el cual se solicita una réplica. Las opciones son: 0,25, 2, 4, 10. Si no se especifica el nivel, se utilizará el nivel del volumen original.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100. Si no se especifica IOPS, se utilizará el IOPS del volumen original.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
Este mandato solicita una réplica para el volumen con el ID 12345678, que realiza una réplica DIARIA, está ubicado en dal09, nivel de grados 4.

### bluemix sl file replica-partners
{: #sl_file_replica_partners}

Listar volúmenes replicantes existentes de un volumen de archivo.
```
bluemix sl file replica-partners VOLUME_ID [OPTIONS]
```


**Ejemplos**:
```
bluemix sl file replica-partners 12345678
```
Este mandato lista volúmenes replicantes existentes de un volumen de archivo con el ID 12345678.

### bluemix sl file snapshot-cancel
{: #sl_file_snapshot_cancel}

Cancelar el espacio de instantáneas existente para un volumen determinado.
```
bluemix sl file snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--reason</dt>
<dd>Una razón opcional para la cancelación.</dd>
<dt>--immediate</dt>
<dd>Cancelar el espacio de instantáneas inmediatamente, en lugar de en el aniversario de facturación.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
Este mandato cancela la instantánea con el ID 12345678 inmediatamente sin pedir confirmación.

### bluemix sl file snapshot-create
{: #sl_file_snapshot_create}

Crear una instantánea en un volumen determinado.
```
bluemix sl file snapshot-create VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Notas para establecer en la nueva instantánea.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
Este mandato crea una instantánea para el volumen con el ID 12345678 y con una nota de adición como snapshotforbluemix.

### bluemix sl file snapshot-disable
{: #sl_file_snapshot_disable}

Inhabilitar instantáneas en la planificación especificada para un volumen determinado.
```
bluemix sl file snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obligatorio. Planificación de instantáneas. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
Este mandato inhabilita la instantánea diaria para el volumen con el ID 12345678.

### bluemix sl file snapshot-enable
{: #sl_file_snapshot_enable}

Habilitar instantáneas para un volumen determinado en la planificación especificada.
```
bluemix sl file snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obligatorio. Planificación de instantáneas. Las opciones son: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Obligatorio. Número de instantáneas que se deben retener.</dd>
<dt>-m, --minute</dt>
<dd>Minuto de la hora en el que deben tomarse las instantáneas, entero entre 0 y 59-</dd>
<dt>-r, --hour</dt>
<dd>Hora del día en la que deben tomarse las instantáneas, número entero entre 0 y 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Día de la semana en que deben tomarse las instantáneas, número entero entre 0 y 6. 0 significa domingo, 1 significa lunes, 2 significa martes, 3 significa miércoles, 4 significa jueves, 5 significa viernes, 6 significa sábado.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
Este mandato habilita la instantánea para el volumen con el ID 12345678. La instantánea se toma semanalmente cada domingo a las 2:00, y se retienen hasta 5 instantáneas.

### bluemix sl file snapshot-delete
{: #sl_file_snapshot_delete}

Suprimir una instantánea en un volumen determinado.
```
bluemix sl file snapshot-delete SNAPSHOT_ID
```


**Ejemplos**:
```
bluemix sl file snapshot-delete 12345678
```
Este mandato suprime la instantánea con el ID 12345678.

### bluemix sl file snapshot-list
{: #sl_file_snapshot_list}

Listar las instantáneas de almacenamiento en archivo.
```
bluemix sl file snapshot-list VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que se debe ordenar. Las opciones son: id,name,created,size_bytes.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-list 12345678 --sortby id
```
Este mandato lista todas las instantáneas de volumen con el ID 12345678 y las ordena por ID.

### bluemix sl file snapshot-order
{: #sl_file_snapshot_order}

Solicitar espacio de instantáneas para un volumen de almacenamiento en archivos.
```
bluemix sl file snapshot-order VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Obligatorio. Tamaño del espacio de instantáneas para crear en GB.</dd>
<dt>-t, --tier</dt>
<dd>Opcional. Nivel de almacenamiento resistente (IOPS por GB) del volumen de archivo para el cual se solicita el espacio. Las opciones son: 0,25, 2, 4, 10.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Distintivo para indicar que el pedido es una actualización.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
Este mandato solicita espacio de instantáneas para el volumen con el ID 12345678, el tamaño es 1000 GB, el nivel de grados es 4 IOPS por GB.

### bluemix sl file snapshot-restore
{: #sl_file_snapshot_restore}

Restaurar volumen de archivo mediante una instantánea determinada.
```
bluemix sl file snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**Ejemplos**:
```
bluemix sl file snapshot-restore 12345678 87654321
```
Este mandato restaura el volumen con el ID 12345678 a partir de la instantánea con el ID 87654321.

### bluemix sl file volume-cancel
{: #sl_file_volume_cancel}

Cancelar un volumen de almacenamiento de archivos existente.
```
bluemix sl file volume-cancel VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--reason</dt>
<dd>Una razón opcional para la cancelación.</dd>
<dt>--immediate</dt>
<dd>Cancelar el volumen de almacenamiento de archivos inmediatamente, en lugar de en el aniversario de facturación.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
Este mandato cancela el volumen con el ID 12345678 inmediatamente y sin solicitar confirmación.

### bluemix sl file volume-list
{: #sl_file_volume_list}

Listar el almacenamiento en archivo.
```
bluemix sl file volume-list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filtrar por nombre de usuario del volumen.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtrar por nombre abreviado de centro de datos.</dd>
<dt>-t, --storage-type</dt>
<dd>Filtrar por tipo de volumen de almacenamiento. Las opciones son: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filtrar por ID del pedido que ha comprado el almacenamiento en archivo.</dd>
<dt>--sortby</dt>
<dd>Columna por la que se debe ordenar. Las opciones son: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,active_transactions,mount_addr.</dd>
<dt>--columns</dt>
<dd>Columnas que se deben visualizar. Las opciones son: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,mount_addr.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
Este mandato lista todos los volúmenes de resistencia en la cuenta actual que están ubicados en dal09, y los ordena por capacidad.

### bluemix sl file volume-detail
{: #sl_file_volume_detail}

Mostrar detalles de un volumen especificado.
```
bluemix sl file volume-detail VOLUME_ID
```


**Ejemplos**:
```
bluemix sl file volume-detail 12345678
```
Este mandato muestra detalles de volumen con el ID 12345678.

### bluemix sl file volume-duplicate
{: #sl_file_volume_duplicate}

Solicitar un volumen de archivo duplicando un volumen existente.
```
bluemix sl file volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID de la instantánea de volumen original a utilizar para la duplicación.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Tamaño del volumen de archivo duplicado en GB, si no se especifica el tamaño se utilizará el del volumen original.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>IOPS de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100. Si no se especifica IOPS, se utilizará el IOPS del volumen original.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Nivel de almacenamiento resistente. Si no se especifica ningún tamaño, se utilizará el nivel del volumen original.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>El tamaño del espacio de instantáneas para la duplicación, si no se especifica espacio de instantáneas, se utilizará el espacio de instantáneas del volumen original.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file volume-duplicate 12345678
```
Este mandato muestra la solicitud de un volumen nuevo duplicando el volumen con el ID 12345678.

### bluemix sl file volume-order
{: #sl_file_volume_order}

Solicitar un volumen de almacenamiento en archivo.
```
bluemix sl file volume-order [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Obligatorio. Tipo de volumen de almacenamiento. Las opciones son: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Obligatorio. Tamaño de volumen de almacenamiento en GB.</dd>
<dt>-i, --iops</dt>
<dd>IOP de almacenamiento de rendimiento, entre 100 y 6000 en múltiplos de 100 [obligatorio para el rendimiento de tipo de almacenamiento].</dd>
<dt>-e, --tier</dt>
<dd>Nivel de almacenamiento resistente (IOP por GB) [obligatorio para la resistencia de tipo de almacenamiento]. Las opciones son: 0,25, 2, 4, 10.</dd>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos.</dd>
<dt>-n, --snapshot-size</dt>
<dd>Parámetro opcional para solicitar espacio de instantáneas junto con el volumen.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
Este mandato solicita un volumen de rendimiento cuyo tamaño es 1000 GB, IOPS es 4000, ubicado en dal09.

### bluemix sl file volume-options
{: #sl_file_volume_options}

Listar todas las opciones para solicitar un almacenamiento en archivo.
```
bluemix sl file volume-options
```


**Ejemplos**:
```
bluemix sl file volume-options
```
Este mandato lista todas las opciones para crear un volumen de almacenamiento en archivos, incluyendo el tipo de almacenamiento, el tamaño de volumen, IOPS, nivel de grados, centro de datos y tamaño de instantánea.

### bluemix sl dns import
{: #sl_dns_import}

Importar una zona basada en un archivo de zona BIND.
```
bluemix sl dns import ZONEFILE [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--dry-run</dt>
<dd>No crear realmente los registros.</dd>
</dl>

**Ejemplos**:
```
bluemix sl dns import ~/blumix.net.txt
```
Este mandato importa la zona y sus registros de recursos del archivo: ~/blumix.net.txt.

### bluemix sl dns record-add
{: #sl_dns_record_add}

Añadir registro de recurso en una zona.
```
bluemix sl dns record-add ZONE RECORD TYPE DATA [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--ttl</dt>
<dd>TTL (Time-To-Live) en segundos, como por ejemplo: 86400. El valor predeterminado es: 7200.</dd>
</dl>

**Ejemplos**:
```
bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
Este mandato añade un registro A a la zona: bluemix.net, su host es "ftp", los datos son "127.0.0.1" y el ttl es 86400 segundos.

### bluemix sl dns record-edit
{: #sl_dns_record_edit}

Actualizar los registros de recursos en una zona.
```
bluemix sl dns record-edit ZONE [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--by-record</dt>
<dd>Editar por registro de host, como www.</dd>
<dt>--by-id</dt>
<dd>Editar un registro único por su ID.</dd>
<dt>--data</dt>
<dd>Registrar datos, como una dirección IP.</dd>
<dt>--ttl</dt>
<dd>Valor de TTL en segundos, como: 86400.</dd>
</dl>

**Ejemplos**:
```
bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
Este mandato edita los registros de la zona: bluemix.net, cuyo ID es 12345678, y establece sus datos en "127.0.0.2" y el ttl a 3600.

### bluemix sl dns record-list
{: #sl_dns_record_list}

Listar todos los registros de recursos en una zona.
```
bluemix sl dns record-list ZONE [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--data</dt>
<dd>Filtrar por datos de registro, como una dirección IP.</dd>
<dt>--record</dt>
<dd>Filtrar por registro de host, como por ejemplo www.</dd>
<dt>--ttl</dt>
<dd>Filtrar por valor de TTL en segundos, como 86400.</dd>
<dt>--type</dt>
<dd>Filtrar por tipo de registro, como A o CNAME.</dd>
</dl>

**Ejemplos**:
```
bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
Este mandato lista todos los registros A en la zona: bluemix.net, filtrado por el host elasticsearch y el ttl es 900 segundos.

### bluemix sl dns record-remove
{: #sl_dns_record_remove}

Eliminar registro de recurso de una zona.
```
bluemix sl dns record-remove RECORD_ID
```


**Ejemplos**:
```
bluemix sl dns record-remove 12345678
```
Este mandato elimina el registro de recurso con el ID 12345678.

### bluemix sl dns zone-create
{: #sl_dns_zone_create}

Crear una zona.
```
bluemix sl dns zone-create ZONE
```


**Ejemplos**:
```
bluemix sl dns zone-create bluemix.net
```
Este mandato crea una zona denominada bluemix.net.

### bluemix sl dns zone-delete
{: #sl_dns_zone_delete}

Suprimir una zona.
```
bluemix sl dns zone-delete ZONE
```


**Ejemplos**:
```
bluemix sl dns zone-delete bluemix.net
```
Este mandato suprime una zona denominada bluemix.net.

### bluemix sl dns zone-list
{: #sl_dns_zone_list}

Listar todas las zonas de su cuenta.
```
bluemix sl dns zone-list
```


**Ejemplos**:
```
bluemix sl dns zone-list
```
Este mandato lista todas las zonas en la cuenta actual.

### bluemix sl dns zone-print
{: #sl_dns_zone_print}

Imprimir registros del recurso y zona en formato BIND.
```
bluemix sl dns zone-print ZONE
```


**Ejemplos**:
```
bluemix sl dns zone-print bluemix.net
```
Este mandato imprime la zona denominada bluemix.net en formato BIND.

### bluemix sl globalip create
{: #sl_globalip_create}

Crear una IP global.
```
bluemix sl globalip create [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--v6</dt>
<dd>Solicitar una dirección IP IPv6.</dd>
<dt>--test</dt>
<dd>Pedido de prueba.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl globalip create --v6
```
Este mandato crea una dirección IP V6.

### bluemix sl globalip assign
{: #sl_globalip_assign}

Asignar una IP global a un direccionador de destino o dispositivo.
```
bluemix sl globalip assign IDENTIFIER TARGET
```


**Ejemplos**:
```
bluemix sl globalip assign 12345678 9.111.123.456
```
Este mandato asigna la dirección IP con el ID 12345678 a un dispositivo de destino cuya dirección IP es 9.111.123.456.

### bluemix sl globalip cancel
{: #sl_globalip_cancel}

Cancelar una IP global.
```
bluemix sl globalip cancel IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl globalip cancel 12345678
```
Este mandato cancela la dirección IP con el ID 12345678.

### bluemix sl globalip list
{: #sl_globalip_list}

Listar todas las IP globales de su cuenta.
```
bluemix sl globalip list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--v4</dt>
<dd>Mostrar solo las IP IPv4.</dd>
<dt>--v6</dt>
<dd>Mostrar solo las IP IPv6.</dd>
<dt>--order</dt>
<dd>Filtrar por el ID del pedido que ha comprado esta dirección IP.</dd>
</dl>

**Ejemplos**:
```
bluemix sl globalip list --v4
```
Este mandato lista todas las direcciones IP V4 en la cuenta actual.

### bluemix sl globalip unassign
{: #sl_globalip_unassign}

Desasignar una IP global de un direccionador de destino o dispositivo.
```
bluemix sl globalip unassign IDENTIFIER
```


**Ejemplos**:
```
bluemix sl globalip unassign 12345678
```
Este mandato desasigna la dirección IP con el ID 12345678 del dispositivo de destino.

### bluemix sl image delete
{: #sl_image_delete}

Suprimir una imagen.
```
bluemix sl image delete IDENTIFIER
```
**Ejemplos**:
```
   bluemix sl image delete 12345678
```
Este mandato suprime la imagen con el ID `12345678`.

### bluemix sl image detail
{: #sl_image_detail}

Obtener detalles para una imagen.
```
bluemix sl image detail IDENTIFIER
```
**Ejemplos**:
```
 bluemix sl image detail 12345678
```
Este mandato obtiene los detalles para la imagen con el ID 12345678.

### bluemix sl image edit
{: #sl_image_edit}

Editar los detalles de una imagen.
```
bluemix sl image edit IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--name</dt>
<dd>Nombre de la imagen.</dd>
<dt>--note</dt>
<dd>Nota adicional para la imagen.</dd>
<dt>--tag</dt>
<dd>Etiquetas para la imagen.</dd>
</dl>

*Ejemplos**:
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
Este mandato edita la imagen con el ID `12345678` y establece el nombre en `ubuntu16`, la nota en `testing`, y la etiqueta en `staging`.

### bluemix sl image list
{: #sl_image_list}

Listar todas las imágenes de su cuenta.
```
bluemix sl image list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--name</dt>
<dd>Filtrar en el nombre de imagen.</dd>
<dt>--public</dt>
<dd>Mostrar solo imágenes públicas.</dd>
<dt>--private</dt>
<dd>Mostrar solo imágenes privadas.</dd>
</dl>

### bluemix sl ipsec cancel
{: #sl_ipsec_cancel}
Cancelar un contexto de túnel VPN de IPSec.
```
bluemix sl ipsec cancel CONTEXT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--immediate</dt>
<dd>Cancelar la IPSec inmediatamente, en lugar de en el aniversario de facturación.</dd>
<dt>--reason</dt>
<dd>Una razón opcional para la cancelación.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl ipsec config
{: #sl_ipsec_config}

Solicitar configuración de un contexto de túnel.
```
bluemix sl ipsec config CONTEXT_ID [OPTIONS]
```

### bluemix sl ipsec detail
{: #sl_ipsec_detail}

Listar detalles de contexto de túnel VPN de IPSec.
```
bluemix sl ipsec detail CONTEXT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-i, --include</dt>
<dd>Incluir recursos adicionales, las opciones son: at,is,rs,sr,ss.</dd>
</dl>
### bluemix sl ipsec list
{: #sl_ipsec_list}

Listar contextos de túnel VPN de IPSec.
```
bluemix sl ipsec list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--order</dt>
<dd>Filtrar por ID del pedido que ha comprado la IPSEC.</dd>
</dl>
### bluemix sl ipsec order
{: #sl_ipsec_order}

Solicitar un túnel VPN de IPSec.
```
bluemix sl ipsec order [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos para la IPSEC, por ejemplo dal09 .</dd>
</dl>

### bluemix sl ipsec subnet-add
{: #sl_ipsec_subnet_add}

Añadir una nueva subred al contexto de túnel de IPSec.
```
bluemix sl ipsec subnet-add CONTEXT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --subnet-id</dt>
<dd>Identificador de subred que se va a añadir, obligatorio.</dd>
<dt>-t, --subnet-type</dt>
<dd>Tipo de subred que se va a añadir, obligatorio, las opciones son: internal,remote,service.</dd>
<dt>-n, --network</dt>
<dd>Identificador de red de subred que se va a crear.</dd>
</dl>

### bluemix sl ipsec subnet-remove
{: #sl_ipsec_subnet_remove}

Eliminar una subred del contexto de túnel de IPSEC.
```
bluemix sl ipsec subnet-remove CONTEXT_ID SUBNET_ID SUBNET_TYPE [OPTIONS]
```

### bluemix sl ipsec translation-add
{: #sl_ipsec_translation_add}

Añadir una conversión de dirección a un túnel de IPSec.
```
bluemix sl ipsec translation-add CONTEXT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Dirección IP estática, obligatoria.</dd>
<dt>-r, --remote-ip</dt>
<dd>Dirección IP remota, obligatoria.</dd>
<dt>-n, --note</dt>
<dd>Nota.</dd>
</dl>
### bluemix sl ipsec translation-remove
{: #sl_ipsec_translation_remove}

Eliminar una entrada de conversión de una IPSec.
```
bluemix sl ipsec translation-remove CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

### bluemix sl ipsec translation-update
{: #sl_ipsec_translation_update}

Actualizar una conversión de dirección para una IPSec.
```
bluemix sl ipsec translation-update CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Dirección IP estática, obligatoria.</dd>
<dt>-r, --remote-ip</dt>
<dd>Dirección IP remota, obligatoria.</dd>
<dt>-n, --note</dt>
<dd>Nota.</dd>
</dl>
### bluemix sl ipsec update
{: #sl_ipsec_update}

Actualizar propiedades de contexto de túnel.
```
bluemix sl ipsec update CONTEXT_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Nombre descriptivo.</dd>
<dt>-r, --remote-peer</dt>
<dd>Dirección IP igual remota.</dd>
<dt>-k, --preshared-key</dt>
<dd>Clave precompartida.</dd>
<dt>-a, --phase1-auth</dt>
<dd>Autenticación de fase 1, las opciones son: MD5,SHA1,SHA256.</dd>
<dt>-c, --phase1-crypto</dt>
<dd>Cifrado de fase 1, las opciones son: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-d, --phase1-dh</dt>
<dd>Grupo diffie hellman de fase 1, las opciones son: 0,1,2,5.</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>Clave para la vida de fase 1, rango 120-172800.</dd>
<dt>-u, --phase2-auth</dt>
<dd>Autenticación de fase 2, las opciones son: MD5,SHA1,SHA256.</dd>
<dt>-y, --phase2-crypto</dt>
<dd>Cifrado de fase 2, las opciones son: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-e, --phase2-dh</dt>
<dd>Grupo diffie hellman de fase 2, las opciones son: 0,1,2,5.</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>PFS de fase 2, rango 0-1.</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>Clave para la vida de fase 2, rango 120-172800.</dd>
</dl>

### bluemix sl loadbal cancel
{: #sl_loadbal_cancel}

Cancelar un equilibrador de carga existente.
```
bluemix sl loadbal cancel LOADBAL_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl loadbal create
{: #sl_loadbal_create}

Añade un equilibrador de carga basado en el ID devuelto desde create-options.
```
bluemix sl loadbal create PRICE_ID LOCATION [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl loadbal create-options
{: #sl_loadbal_create_options}

Obtener opciones de precios con las que crear un equilibrador de carga.
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail
{: #sl_loadbal_detail}

Obtener detalles del equilibrador de carga.
```
bluemix sl loadbal detail LOADBAL_ID
```

### bluemix sl loadbal group-add
{: #sl_loadbal_group_add}

Añade un nuevo servicio load_balancer.
```
bluemix sl loadbal group-add LOADBAL_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Obligatorio. El porcentaje de conexiones asignadas.</dd>
<dt>-p, --port</dt>
<dd>Obligatorio. El número de puerto.</dd>
<dt>-t, --routing-type</dt>
<dd>Obligatorio. El ID del tipo de direccionamiento. Ejecute 'bluemix sl loadbal routing-types' para buscar un ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Obligatorio. El ID del método de direccionamiento. Ejecute 'bluemix sl loadbal routing-methods' para buscar un ID.</dd>
</dl>

### bluemix sl loadbal group-delete
{: #sl_loadbal_group_delete}

Suprime un grupo de servicios de equilibrador de carga existente.
```
bluemix sl loadbal group-delete GROUP_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl loadbal group-edit
{: #sl_loadbal_group_edit}

Editar un grupo de servicios de equilibrador de carga existente.
```
bluemix sl loadbal group-edit LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Cambie el porcentaje asignado de las conexiones.</dd>
<dt>-p, --port</dt>
<dd>Cambie el número de puerto.</dd>
<dt>-t, --routing-type</dt>
<dd>Cambie el ID del tipo de direccionamiento. Ejecute 'bluemix sl loadbal routing-types' para buscar un ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Cambie el ID del método de direccionamiento. Ejecute 'bluemix sl loadbal routing-methods' para buscar un ID.</dd>
</dl>

### bluemix sl loadbal group-reset
{: #sl_loadbal_group_reset}

Restablecer conexiones en un determinado grupo de servicios.
```
bluemix sl loadbal group-reset LOADBAL_ID GROUP_ID
```

### bluemix sl loadbal health-checks
{: #sl_loadbal_health_checks}

Listar tipos de comprobación de estado.
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list
{: #sl_loadbal_list}

Listar equilibradores de carga activos.
```
bluemix sl loadbal list
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Filtrar por nombre abreviado de centro de datos.</dd>
<dt>-o, --order</dt>
<dd>Filtrar por ID del pedido que ha comprado el equilibrador de carga.</dd>
<dt>-p, --ip-address</dt>
<dd>Filtrar por dirección IP.</dd>
</dl>
### bluemix sl loadbal routing-methods
{: #sl_loadbal_routing_methods}

Listar métodos de direccionamiento.
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types
{: #sl_loadbal_routing_types}

Listar tipos de direccionamiento.
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add
{: #sl_loadbal_service_add}

Añade un nuevo servicio de equilibrador de carga.
```
bluemix sl loadbal service-add LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--disabled</dt>
<dd>Opcional. Cree el servicio como inhabilitado, el valor predeterminado es habilitado si no se especifica.</dd>
<dt>-p, --port</dt>
<dd>Obligatorio. El número de puerto del servicio.</dd>
<dt>-w, --weight</dt>
<dd>Obligatorio. El peso del servicio.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Obligatorio. El tipo de comprobación de estado.</dd>
<dt>-i, --ip-address</dt>
<dd>Obligatorio. La dirección IP del servicio.</dd>
</dl>

### bluemix sl loadbal service-delete
{: #sl_loadbal_service_delete}

Suprime un servicio de equilibrador de carga existente.
```
bluemix sl loadbal service-delete SERVICE_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl loadbal service-edit
{: #sl_loadbal_service_edit}

Editar las propiedades de un grupo de servicios.
```
bluemix sl loadbal service-edit LOADBAL_ID SERVICE_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--disabled</dt>
<dd>Inhabilitar el servicio.</dd>
<dt>--enabled</dt>
<dd>Habilitar el servicio.</dd>
<dt>-p, --port</dt>
<dd>Cambie el número de puerto del servicio.</dd>
<dt>-w, --weight</dt>
<dd>Cambie el peso del servicio.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Cambie el tipo de comprobación de estado.</dd>
<dt>-i, --ip-address</dt>
<dd>Cambie la dirección IP del servicio.</dd>
</dl>

### bluemix sl loadbal service-toggle
{: #sl_loadbal_service_toggle}

Conmutar el estado de un servicio de equilibrador de carga existente.
```
bluemix sl loadbal service-toggle SERVICE_ID
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

### bluemix sl security sshkey-add
{: #sl_security_sshkey_add}

Añadir una nueva clave SSH.
```
bluemix sl security sshkey-add LABEL [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --in-file</dt>
<dd>El archivo id_rsa.pub a importar para esta clave.</dd>
<dt>-k, --key</dt>
<dd>La clave SSH real.</dd>
<dt>--note</dt>
<dd>Nota adicional que se asociará a la clave.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
Este mandato añade una clave SSH desde el archivo: ~/.ssh/id_rsa.pub con la nota "mykey".

### bluemix sl security sshkey-edit
{: #sl_security_sshkey_edit}

Editar una clave SSH.
```
bluemix sl security sshkey-edit IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--label</dt>
<dd>La nueva etiqueta para la clave.</dd>
<dt>--note</dt>
<dd>Nuevas notas para la clave.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
Este mandato actualiza la clave SSH con el ID 12345678 y establece la etiqueta en "Bluemix" y la nota en "testing".

### bluemix sl security sshkey-list
{: #sl_security_sshkey_list}

Listar claves SSH de su cuenta.
```
bluemix sl security sshkey-list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna por la que se debe ordenar. Las opciones son: id,label,fingerprint,notes.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security sshkey-list --sortby label
```
Este mandato lista todas las claves SSH de la cuenta actual y las ordena por etiqueta.

### bluemix sl security sshkey-print
{: #sl_security_sshkey_print}

Imprime una clave SSH para la pantalla.
```
bluemix sl security sshkey-print IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --out-file</dt>
<dd>La clave SSH pública se escribirá en este archivo.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
Este mandato muestra el ID, la etiqueta y las notas de la clave SSH con el ID 12345678 y escribe la clave pública en el archivo: ~/mykey.pub.

### bluemix sl security sshkey-remove
{: #sl_security_sshkey_remove}

Elimina una clave SSH de forma permanente.
```
bluemix sl security sshkey-remove IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security sshkey-remove 12345678 -f
```
Este mandato elimina la clave SSH con el ID 12345678 sin solicitar confirmación.

### bluemix sl security cert-add
{: #sl_security_cert_add}

Añadir y cargar detalles del certificado SSL.
```
bluemix sl security cert-add [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--crt</dt>
<dd>Archivo de certificado.</dd>
<dt>--csr</dt>
<dd>Archivo de solicitud de solicitud de firma de certificado.</dd>
<dt>--icc</dt>
<dd>Archivo de certificado intermedio.</dd>
<dt>--key</dt>
<dd>Archivo de claves privado.</dd>
<dt>--notes</dt>
<dd>Notas adicionales.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key
```
Este mandato añade un archivo de certificado: ~/bluemix.net.cert y el archivo de claves privado ~/bluemix.net.key para el dominio bluemix.net.

### bluemix sl security cert-edit
{: #sl_security_cert_edit}

Editar certificado SSL.
```
bluemix sl security cert-edit IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--crt</dt>
<dd>Archivo de certificado.</dd>
<dt>--csr</dt>
<dd>Archivo de solicitud de solicitud de firma de certificado.</dd>
<dt>--icc</dt>
<dd>Archivo de certificado intermedio.</dd>
<dt>--key</dt>
<dd>Archivo de claves privado.</dd>
<dt>--notes</dt>
<dd>Notas adicionales.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
Este mandato edita el certificado con el ID 12345678 y actualiza su clave privada con el archivo: ~/bluemix.net.key.

### bluemix sl security cert-download
{: #sl_security_cert_download}

Descargar el certificado SSL y los archivos de claves.
```
bluemix sl security cert-download IDENTIFIER
```


**Ejemplos**:
```
bluemix sl security cert-download 12345678
```
Este mandato descarga 4 archivos al directorio actual para el certificado con el ID 12345678. Los 4 archivos son: archivo de certificado, archivo de solicitud de firma de certificado, archivo de certificado intermedio y archivo de claves privado.

### bluemix sl security cert-list
{: #sl_security_cert_list}

Listar certificados SSL de su cuenta.
```
bluemix sl security cert-list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--status</dt>
<dd>Mostrar certificados con este estado, el valor predeterminado es: all, las opciones son: all,valid,expired.</dd>
<dt>--sortby</dt>
<dd>Columna por la que se debe ordenar. Las opciones son: id,common_name,days_until_expire,notes.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security cert-list --status valid --sortby days_until_expire
```
Este mandato lista todos los certificados válidos de la cuenta actual y los ordena por días de validez.

### bluemix sl security cert-remove
{: #sl_security_cert_remove}

Eliminar certificado SSL.
```
bluemix sl security cert-remove IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl security cert-remove 12345678
```
Este mandato elimina el certificado con el ID 12345678.

### bluemix sl subnet cancel
{: #sl_subnet_cancel}

Cancelar una subred.
```
bluemix sl subnet cancel IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl subnet cancel 12345678 -f
```
Este mandato cancela la subred con el ID 12345678 sin solicitar confirmación.

### bluemix sl subnet create
{: #sl_subnet_create}

Añadir una nueva subred a su cuenta.
```
bluemix sl subnet create NETWORK QUANTITY VLAN_ID [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--v6, --ipv6</dt>
<dd>Solicitar direcciones IPv6.</dd>
<dt>--test</dt>
<dd>No realizar el pedido de la subred; solo obtener un presupuesto.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl subnet create public 16 567
```
Este mandato crea una subred pública con direcciones 16 IP v4 y la coloca en la vlan con el ID 567.

### bluemix sl subnet detail
{: #sl_subnet_detail}

Obtener detalles de una subred.
```
bluemix sl subnet detail IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Ocultar lista de servidores virtuales.</dd>
<dt>--no-hardware</dt>
<dd>Ocultar lista de hardware.</dd>
</dl>

**Ejemplos**:
```
bluemix sl subnet detail 12345678
```
Este mandato muestra información detallada sobre la subred con el ID 12345678, incluyendo información de servidores de hardware y servidores virtuales.

### bluemix sl subnet list
{: #sl_subnet_list}

Listar todas las subredes de su cuenta.
```
bluemix sl subnet list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna para ordenar por. Las opciones son: id,identifier,type,network_space,datacenter,vlan_id,IPs,hardware,vs.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtrar por nombre abreviado de centro de datos.</dd>
<dt>--identifier</dt>
<dd>Filtrar por identificador de red.</dd>
<dt>-t, --subnet-type</dt>
<dd>Filtrar por tipo de subred.</dd>
<dt>--network-space</dt>
<dd>Filtrar por espacio de red.</dd>
<dt>--v4, --ipv4</dt>
<dd>Mostrar solo subredes IPv4.</dd>
<dt>--v6, --ipv6</dt>
<dd>Mostrar solo subredes IPv6.</dd>
<dt>--order</dt>
<dd>Filtrar por el ID del pedido que ha comprado las subredes.</dd>
</dl>

**Ejemplos**:
```
bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
Este mandato lista subredes IP V4 de la cuenta actual, filtrando por centro de datos es dal09, el tipo de subred es PRIMARY y el espacio de red es PUBLIC.

### bluemix sl subnet lookup
{: #sl_subnet_lookup}

Buscar una dirección IP y visualizar su información de dispositivos y subredes.
```
bluemix sl subnet lookup IP_ADDRESS
```


**Ejemplos**:
```
bluemix sl subnet lookup 9.125.235.255
```
Este mandato encuentra el registro de dirección IP con la dirección 9.125.235.255 y muestra la información del dispositivo y la subred.

### bluemix sl vlan create
{: #sl_vlan_create}

Crear una nueva VLAN.
```
bluemix sl vlan create [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-t, --vlan-type</dt>
<dd>El tipo de VLAN, ya sea pública o privada.</dd>
<dt>-r, --router</dt>
<dd>El nombre de host del direccionador.</dd>
<dt>-d, --datacenter</dt>
<dd>El nombre abreviado del centro de datos.</dd>
<dt>-s, --size</dt>
<dd>El tamaño de las subredes, las opciones son: 8 (5 IP utilizables) o 16 (13 IP utilizables) o 32 (29 IP utilizables).</dd>
<dt>-n, --name</dt>
<dd>El nombre de la VLAN.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
Este mandato crea una vlan pública, ubicada en el centro de datos dal09 con 16 direcciones IP y el nombre es myvlan.

### bluemix sl vlan cancel
{: #sl_vlan_cancel}

Cancelar una VLAN.
```
bluemix sl vlan cancel IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vlan cancel 12345678 -f
```
Este mandato cancela la vlan con el ID 12345678 sin solicitar confirmación.

### bluemix sl vlan detail
{: #sl_vlan_detail}

Obtener detalles sobre una VLAN.
```
bluemix sl vlan detail IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Ocultar lista de servidores virtuales.</dd>
<dt>--no-hardware</dt>
<dd>Ocultar lista de hardware.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
Este mandato muestra los detalles de la vlan con el ID 12345678, y no la lista de servidor virtual ni servidor de hardware.

### bluemix sl vlan edit
{: #sl_vlan_edit}

Editar los detalles sobre una VLAN.
```
bluemix sl vlan edit IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-n, --name</dt>
<dd>El nombre de la VLAN.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vlan edit 12345678 -n myvlan-rename
```
Este mandato actualiza la vlan con el ID 12345678 y le da un nombre nuevo "myvlan-rename".

### bluemix sl vlan list
{: #sl_vlan_list}

Listar todas las VLAN de su cuenta.
```
bluemix sl vlan list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--sortby</dt>
<dd>Columna para ordenar por las siguientes opciones: id, number, name, firewall, datacenter, hardware, virtual_servers, public_ips.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtrar por nombre abreviado de centro de datos.</dd>
<dt>-n, --number</dt>
<dd>Filtrar por número de VLAN.</dd>
<dt>--name</dt>
<dd>Filtrar por nombre de VLAN.</dd>
<dt>--order</dt>
<dd>Filtrar por ID del pedido que ha comprado la VLAN.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vlan list -d dal09 --sortby number
```
Este mandato lista todas las vlans de la cuenta actual filtrando por centro de datos igual a dal09, y los ordena por número de vlan.

### bluemix sl vlan options
{: #sl_vlan_options}

Listar todas las opciones para crear VLAN.
```
bluemix sl vlan options
```


**Ejemplos**:
```
bluemix sl vlan options
```
Este mandato lista todas las opciones para crear una vlan, por ejemplo, tipo de vlan, centros de datos, tamaño de subred, direccionadores, etc.

### bluemix sl vs cancel
{: #sl_vs_cancel}

Cancelar la instancia de servidor virtual.
```
bluemix sl vs cancel IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs cancel 12345678
```
Este mandato cancela la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs capture
{: #sl_vs_capture}

Capturar la instancia de servidor virtual en una imagen.
```
bluemix sl vs capture IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Obligatorio. Nombre de la imagen.</dd>
<dt>--all</dt>
<dd>Capturar todos los discos que pertenecen al VS.</dd>
<dt>--note</dt>
<dd>Añadir una nota para asociar a la imagen.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
Este mandato captura la instancia de servidor virtual con el ID de 12345678 con todos los discos en una imagen denominada "mybluemix" con la nota "testing".

### bluemix sl vs create
{: #sl_vs_create}

Crear una instancia de servidor virtual.
```
bluemix sl vs create [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-H, --hostname</dt>
<dd>Obligatorio. Parte de host del FQDN.</dd>
<dt>-D, --domain</dt>
<dd>Obligatorio. Parte de dominio del FQDN.</dd>
<dt>-c, --cpu</dt>
<dd>Obligatorio. Número de núcleos de CPU.</dd>
<dt>-m, --memory</dt>
<dd>Obligatorio. Memoria en megabytes.</dd>
<dt>-d, --datacenter</dt>
<dd>Obligatorio. Nombre abreviado del centro de datos.</dd>
<dt>-o, --os</dt>
<dd>Código de instalación de sistema operativo. Consejo: puede especificar <OS>_LATEST.</dd>
<dt>--image</dt>
<dd>ID de imagen. Consulte: 'bluemix sl image list' como referencia.</dd>
<dt>--billing</dt>
<dd>Tasa de facturación. El valor predeterminado es: por hora. Las opciones son: por hora, mensual.</dd>
<dt>--dedicated</dt>
<dd>Crear un servidor virtual dedicado (nodo privado).</dd>
<dt>--san</dt>
<dd>Utilizar un almacenamiento SAN en lugar de un disco local.</dd>
<dt>--test</dt>
<dd>No crear realmente el servidor virtual.</dd>
<dt>--export</dt>
<dd>Exporta opciones a un archivo de plantilla.</dd>
<dt>-i, --postinstall</dt>
<dd>Publicar-instalar script para descargar.</dd>
<dt>-k, --key</dt>
<dd>ID de las claves SSH para añadir al usuario root (se permiten varios).</dd>
<dt>--disk</dt>
<dd>Tamaños de disco (se permiten varios).</dd>
<dt>--private</dt>
<dd>Fuerza el servidor virtual para que sólo tenga acceso a la red privada.</dd>
<dt>--like</dt>
<dd>Utilizar la configuración de un servidor virtual existente.</dd>
<dt>-n, --network</dt>
<dd>Velocidad de puerto de red en Mbps.</dd>
<dt>--tag</dt>
<dd>Etiquetas para añadir a la instancia (se permiten varias).</dd>
<dt>-t, --template</dt>
<dd>Un archivo de plantilla que establece valores predeterminados en las opciones de línea de mandatos.</dd>
<dt>-u, --userdata</dt>
<dd>Cadena de metadatos definida por el usuario.</dd>
<dt>-F, --userfile</dt>
<dd>Leer datos de usuario del archivo.</dd>
<dt>--vlan-public</dt>
<dd>ID de la VLAN pública donde quiere colocar el servidor virtual.</dd>
<dt>--vlan-private</dt>
<dd>ID de la VLAN privada donde quiere colocar el servidor virtual.</dd>
<dt>--wait</dt>
<dd>Espere hasta que el servidor virtual finalice el suministro durante x segundos antes de volver.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
Este mandato solicita una instancia de servidor virtual cuyo nombre de host es myvsi, el dominio es bluemix.net, 4 núcleos de cpu, 4096M de memoria, ubicada en el centro de datos: dal10,

### bluemix sl vs options
{: #sl_vs_options}

Listar las opciones para crear una instancia de servidor virtual.
```
bluemix sl vs options [OPTIONS]
```


**Ejemplos**:
```
bluemix sl vs options
```
Este mandato lista todas las opciones para crear una instancia de servidor virtual, por ejemplo centros de datos, cpu, memoria, sistema operativo, disco, velocidad de red, etc.

### bluemix sl vs credentials
{: #sl_vs_credentials}

Listar las credenciales de instancia de servidor virtual.
```
bluemix sl vs credentials IDENTIFIER [OPTIONS]
```


**Ejemplos**:
```
bluemix sl vs credentials 12345678
```
Este mandato lista todos los pares de nombres de usuario y contraseñas de la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs detail
{: #sl_vs_detail}

Obtener detalles para una instancia de servidor virtual.
```
bluemix sl vs detail IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--passwords</dt>
<dd>Mostrar contraseñas (revise por encima).</dd>
<dt>--price</dt>
<dd>Mostrar precios asociados.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs details 12345678
```
Este mandato lista información detallada sobre la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs dns-sync
{: #sl_vs_dns_sync}

Sincronizar los registros de DNS para una instancia de servidor virtual.
```
bluemix sl vs dns-sync IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-a, --a-record</dt>
<dd>Sincronizar el registro A para el host.</dd>
<dt>--aaaa-record</dt>
<dd>Sincronizar el registro AAAA para el host.</dd>
<dt>--ptr</dt>
<dd>Sincronizar el registro PTR para el host.</dd>
<dt>--ttl</dt>
<dd>Establece el TTL para los registros A y/o PTR, el valor predeterminado es: 7200.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
Este mandato sincroniza un registro A (dirección IP V4) de la instancia de servidor virtual con el ID 12345678 con el servidor DNS y establece el ttl de este registro A en 3600.

### bluemix sl vs edit
{: #sl_vs_edit}

Editar detalles de una instancia de servidor virtual.
```
bluemix sl vs edit IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-D, --domain</dt>
<dd>Parte de dominio del FQDN.</dd>
<dt>-H, --hostname</dt>
<dd>Parte de host del FQDN. Ejemplo: servidor.</dd>
<dt>--tag</dt>
<dd>Etiquetas para establecer o cadena vacía para eliminar todas.</dd>
<dt>-u, --userdata</dt>
<dd>Cadena de metadatos definida por el usuario.</dd>
<dt>-F, --userfile</dt>
<dd>Leer datos de usuario del archivo.</dd>
<dt>--public-speed</dt>
<dd>Velocidad de puerto público, las opciones son: 0,10,100,1000,10000.</dd>
<dt>--private-speed</dt>
<dd>Velocidad de puerto privado, las opciones son: 0,10,100,1000,10000.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
Este mandato actualiza la instancia de servidor virtual con el ID 12345678 y establece su dominio en "bluemix.net", el nombre de host en "myapp", la etiqueta en "testcli",

### bluemix sl vs list
{: #sl_vs_list}

Listar las instancias de servidor virtual de su cuenta.
```
bluemix sl vs list [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Número de núcleos de CPU.</dd>
<dt>-D, --domain</dt>
<dd>Parte de dominio del FQDN.</dd>
<dt>-d, --datacenter</dt>
<dd>Nombre abreviado del centro de datos.</dd>
<dt>-H, --hostname</dt>
<dd>Parte de host del FQDN.</dd>
<dt>-m, --memory</dt>
<dd>Memoria en megabytes.</dd>
<dt>-n, --network</dt>
<dd>Velocidad de puerto de red en Mbps.</dd>
<dt>--hourly</dt>
<dd>Mostrar solo las instancias por hora.</dd>
<dt>--monthly</dt>
<dd>Mostrar solo las instancias mensuales.</dd>
<dt>--tag</dt>
<dd>Filtrar por etiquetas (se permiten varias).</dd>
<dt>--sortby</dt>
<dd>Columna para ordenar por las siguientes opciones: id,hostname,domain,datacenter,cpu,memory,primary_ip,backend_ip. El valor predeterminado es: hostname.</dd>
<dt>--columns</dt>
<dd>Columnas por visualizar, las opciones son: guid,primary_ip,backend_ip,datacenter,action,power_state,created_by,tags. El valor predeterminado es: id,hostname,primary_ip,backend_ip,datacenter,action.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
Este mandato lista todas las instancias de servidor virtual de facturación por hora de la cuenta actual, filtrando el dominio igual a "bluemix.net" y ordenándolas por memoria.

### bluemix sl vs pause
{: #sl_vs_pause}

Detener una instancia de servidor virtual activa.
```
bluemix sl vs pause IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs pause 12345678 -f
```
Este mandato detiene la instancia de servidor virtual con el ID 12345678 sin solicitar confirmación.

### bluemix sl vs power-off
{: #sl_vs_power_off}

Apagar una instancia de servidor virtual activa.
```
bluemix sl vs power-off IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--hard</dt>
<dd>Realizar un cierre (hard shutdown).</dd>
<dt>--soft</dt>
<dd>Realizar un cierre (soft shutdown).</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs power-off 12345678 --soft
```
Este mandato realiza un apagado (soft power off) para la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs power-on
{: #sl_vs_power_on}

Encender una instancia de servidor virtual.
```
bluemix sl vs power-on IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs power-on 12345678
```
Este mandato realiza un encendido para la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs ready
{: #sl_vs_ready}

Comprobar si hay una instancia de servidor virtual lista para su uso.
```
bluemix sl vs ready IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--wait</dt>
<dd>Espere hasta que el servidor virtual finalice el suministro durante x segundos antes de volver.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs ready 12345678 --wait 30
```
Este mandato comprueba la instancia de servidor virtual con el estado del ID 12345678 para ver si está lista para su uso continuado y espera hasta 30 segundos.

### bluemix sl vs reboot
{: #sl_vs_reboot}

Rearrancar una instancia de servidor virtual activa.
```
bluemix sl vs reboot IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>--hard</dt>
<dd>Realizar un rearranque (hard reboot).</dd>
<dt>--soft</dt>
<dd>Realizar un rearranque (hard reboot).</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs reboot 12345678 --hard
```
Este mandato realiza un rearranque (hard reboot) para la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs reload
{: #sl_vs_reload}

Volver a cargar el sistema operativo en una instancia de servidor virtual.
```
bluemix sl vs reload IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-i, --postinstall</dt>
<dd>Publicar-instalar script para descargar.</dd>
<dt>--image</dt>
<dd>ID de imagen. El valor predeterminado es utilizar el sistema operativo actual.</dd>
<dt>Consulte:</dt>
<dd>'bluemix sl image list' como referencia.</dd>
<dt>-k, --key</dt>
<dd>ID de las claves SSH para añadir al usuario root (se permiten varios).</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs reload 12345678
```
Este mandato vuelve a cargar el sistema operativo actual para la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs rescue
{: #sl_vs_rescue}

Rearrancar una instancia de servidor virtual en una imagen de rescate.
```
bluemix sl vs rescue IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs rescue 12345678
```
Este mandato rearranca la instancia de servidor virtual con el ID 12345678 en una imagen de rescate.

### bluemix sl vs resume
{: #sl_vs_resume}

Reanudar una instancia de servidor virtual detenida.
```
bluemix sl vs resume IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs resume 12345678
```
Este mandato reanuda la instancia de servidor virtual con el ID 12345678.

### bluemix sl vs upgrade
{: #sl_vs_upgrade}

Actualizar una instancia de servidor virtual.
```
bluemix sl vs upgrade IDENTIFIER [OPTIONS]
```

<strong>Opciones de mandato</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Número de núcleos de CPU.</dd>
<dt>--private</dt>
<dd>El núcleo de CPU estará en un servidor de host dedicado.</dd>
<dt>-m, --memory</dt>
<dd>Memoria en megabytes.</dd>
<dt>--network</dt>
<dd>Velocidad de puerto de red en Mbps.</dd>
<dt>-f, --force</dt>
<dd>Forzar la operación sin confirmación.</dd>
</dl>

**Ejemplos**:
```
bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
Este mandato actualiza la instancia de servidor virtual con el ID 12345678 y establece el número de núcleos de CPU en 8, la memoria en 8192M, la velocidad de puerto de red en 1000 Mbps.

