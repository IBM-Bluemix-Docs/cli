---

copyright:

  years: 2016,2017

lastupdated: "2017-09-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Comandi {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl)
{: #softlayer_cli}

Il plug-in {{site.data.keyword.BluSoftlayer}} è stato inglobato nella CLI {{site.data.keyword.Bluemix_notm}} e non devi più installarlo.

Utilizza i comandi {{site.data.keyword.BluSoftlayer_notm}} nella CLI (command line interface) {{site.data.keyword.Bluemix_notm}} per configurare e gestire i servizi SoftLayer.


Per iniziare, installa la CLI di IBM {{site.data.keyword.Bluemix_notm}}. Per i dettagli, vedi
[CLI Bluemix ![Icona link esterno](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window}.

Per un elenco completo dei comandi {{site.data.keyword.Bluemix_notm}}, vedi: [Comandi {{site.data.keyword.Bluemix_notm:}} (bx)](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)


## Comandi {{site.data.keyword.BluSoftlayer_notm}} generali

Sono supportati i seguenti comandi. Utilizza il comando `bluemix sl` per visualizzare l'elenco di comandi disponibili:

<table summary="Comandi generali riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 1. Comandi Softlayer generali</caption>
 <thead>
 <th colspan="6">Comandi Softlayer generali</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## Comandi di archiviazione blocchi {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 2. Archiviazione blocchi Softlayer</caption>
 <thead>
 <th colspan="6">Archiviazione blocchi Softlayer</th>
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

 ## Comandi CDN {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 3. CDN Softlayer</caption>
 <thead>
 <th colspan="6">CDN Softlayer</th>
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

## Comandi di archiviazione di file {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 4. Archiviazione file Softlayer</caption>
 <thead>
 <th colspan="6">Archiviazione file Softlayer</th>
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

## Comandi DNS {{site.data.keyword.BluSoftlayer_notm}}

<table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 5. Comandi DNS Softlayer</caption>
 <thead>
 <th colspan="6">Comandi DNS Softlayer</th>
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

<table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 6. Comandi IP globali Softlayer</caption>
 <thead>
 <th colspan="6">Comandi IP globali Softlayer</th>
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

## Comandi di immagine {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 7. Comandi immagine Softlayer</caption>
 <thead>
 <th colspan="6">Comandi di immagine Softlayer</th>
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
 
 ## Comandi VPN IPSec {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 7. Comandi VPN IPSec Softlayer</caption>
 <thead>
 <th colspan="6">Comandi VPN IPSec Softlayer</th>
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

 ## Comandi Load Balancer {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 8. Comandi del programma di bilanciamento del carico Softlayer</caption>
 <thead>
 <th colspan="6">Comandi del programma di bilanciamento del carico Softlayer</th>
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

## Comandi di sicurezza {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 9. Comandi di sicurezza Softlayer</caption>
 <thead>
 <th colspan="5">Comandi di sicurezza Softlayer</th>
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

## Comandi di sottorete {{site.data.keyword.BluSoftlayer_notm}}
 
 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 10. Comandi di sottorete Softlayer</caption>
 <thead>
 <th colspan="5">Comandi di sottorete Softlayer</th>
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
 
## Comandi di server virtuale {{site.data.keyword.BluSoftlayer_notm}}

 <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 11. Comandi di server virtuale Softlayer</caption>
 <thead>
 <th colspan="6">Comandi di server virtuale Softlayer</th>
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
 
## Comandi VLAN {{site.data.keyword.BluSoftlayer_notm}}

  <table summary="Comandi generali di Softlayer riportati in ordine alfabetico con dei link a ulteriori informazioni sul comando">
<caption>Tabella 12. Comandi VLAN Softlayer</caption>
 <thead>
 <th colspan="6">Comandi VLAN Softlayer</th>
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

### Utilizzo dei comandi
Per visualizzare le informazioni sulla guida per i comandi, esegui: `bluemix sl [command] -h`.

### bluemix sl init
{: #sl_init}

Inizializza le impostazioni di configurazione utilizzate per connettersi all'ambiente SoftLayer. La configurazione include nome utente, chiave API o password, account ed endpoint.
```
bluemix sl init [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-a, --api-endpoint</dt>
<dd>URL dell'endpoint API Softlayer; il valore predefinito è:  https://api.softlayer.com/rest/v3.1 per l'autenticazione di chiave API Softlayer, https://api.softlayer.com/mobile/v3.1 per l'autenticazione di ID IBM.</dd>
<dt>-u, --sl-user</dt>
<dd>Nome utente Softlayer.</dd>
<dt>-p, --sl-password</dt>
<dd>Password o chiave API Softlayer.</dd>
<dt>-c, --account-id</dt>
<dd>ID account Softlayer.</dd>
<dt>-q, --security-question-id</dt>
<dd>ID della domanda di sicurezza utilizzato per l'autenticazione; chiedi al tuo proprietario dell'account se non lo conosci.</dd>
<dt>-w, --security-question-answer</dt>
<dd>Risposta alla domanda di sicurezza utilizzata per l'autenticazione; chiedi al tuo proprietario dell'account se non la conosci.</dd>
<dt>-s, --security-code</dt>
<dd>Codice di sicurezza generato dal fornitore della sicurezza quando è abilitata l'autenticazione a 2 fattori.</dd>
<dt>-v, --security-vendor</dt>
<dd>Fornitore della sicurezza che fornisce il codice di sicurezza per l'autenticazione; le opzioni sono: VERISIGN,TOTP,PHONE_FACTOR.</dd>
<dt>-t, --auth-token</dt>
<dd>Token di autenticazione quando è abilitata l'autenticazione tramite telefono.</dd>
</dl>

Ad esempio, accedi con nome utente e password o chiave API Softlayer
```
$ bluemix sl config
Scegli come configurare l'autenticazione Softlayer:
1. Accedi con nome utente e password/chiave API Softlayer
2. Utilizza SSO (Single-Sign-On) Bluemix
Immetti un numero>1
URL endpoint API Softlayer: [https://api.softlayer.com/rest/v3.1]>
Nome utente: []> wangjunl@cn.ibm.com
Chiave API o password: []> abcd

Endpoint API Softlayer:    https://api.softlayer.com/rest/v3.1
ID account:                278444
ID utente:                   wangjunl@cn.ibm.com
Chiave API:                   xxxxxxxxxx
```
Ad esempio, utilizza SSO (Single-Sign-On) Bluemix per accedere a Softlayer
```
$ bx login -a api.ng.bluemix.net -u wangjunl@cn.ibm.com -p xxxxxxx -c 65ce8074c6c62b5
Endpoint API: api.ng.bluemix.net
Autenticazione in corso...
OK

Account di destinazione account di Wilma (65ce8074c6c62b5)
                  
Endpoint API:   https://api.ng.bluemix.net (API version: 2.54.0)   
Regione:         us-south
Utente:           wangjunl@cn.ibm.com
Account:        Account di Wilma (65ce8074c6c62b5)   
Nessuna organizzazione o nessuno spazio di destinazione; usa 'bx target --cf oppure bx target -o ORGANIZZAZIONE -s SPAZIO'

Suggerimento: usa 'bx cf <command>' per eseguire la CLI Cloud Foundry con il contesto di CLI Bluemix.
```

$ bx sl init
Scegli come configurare l'autenticazione Softlayer: 
1. Esegui l'accesso con il nome utente e la password/chiave API Softlayer
2. Utilizza SSO (Single-Sign-On) Bluemix
Immetti un numero> 2
URL endpoint API Softlayer: [https://api.softlayer.com/mobile/v3.1]> 
Impostazione dell'account su: 278444
OK
                              
Endpoint API Softlayer:    https://api.softlayer.com/mobile/v3.1   
ID account:                278444   
ID utente:                   12345678   
Token IMS:                 xxxxxxxxxx
```

### bluemix sl help
{: #sl_help}

Visualizza le informazioni della guida per tutti i comandi per gestire l'ambiente Softlayer.
```
bluemix sl help

```

### bluemix sl block access-authorize
{: #sl_block_access_authorize}

Autorizza gli host ad accedere a un volume fornito.
```
bluemix sl block access-authorize ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>L'ID di un server hardware da autorizzare.</dd>
<dt>-v, --virtual-id</dt>
<dd>L'ID di un server virtuale da autorizzare.</dd>
<dt>-i, --ip-address-id</dt>
<dd>L'ID di un indirizzo IP da autorizzare.</dd>
<dt>-p, --ip-address</dt>
<dd>Un indirizzo IP da autorizzare.</dd>
</dl>

**Esempi**:
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
Questo comando autorizza il server virtuale con ID 87654321 ad accedere al volume con ID 12345678.

### bluemix sl block access-list
{: #sl_block_access_list}

Elenca gli ACL.
```
bluemix sl block access-list ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Colonne da visualizzare; le opzioni sono: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Esempi**:
```
bluemix sl block access-list 12345678 --sortby id
```
Questo comando elenca tutti gli host autorizzati ad accedere al volume con ID 12345678 e li ordina in base all'ID.

### bluemix sl block access-revoke
{: #sl_block_access_revoke}

Revoca l'autorizzazione per gli host che accedono a un volume fornito.
```
bluemix sl block access-revoke ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>L'ID di un server hardware da revocare.</dd>
<dt>-v, --virtual-id</dt>
<dd>L'ID di un server virtuale da revocare.</dd>
<dt>-i, --ip-address-id</dt>
<dd>L'ID di un indirizzo IP da revocare.</dd>
<dt>-p, --ip-address</dt>
<dd>Un indirizzo IP da revocare.</dd>
</dl>

**Esempi**:
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
Questo comando revoca l'accesso del server virtuale con ID 87654321 al volume con ID 12345678.

### bluemix sl block replica-failback
{: #sl_block_replica_failback}

Failback di un volume di blocchi dalla replica.
```
bluemix sl block replica-failback ID_VOLUME
```


**Esempi**:
```
bluemix sl block replica-failback 12345678
```
Questo comando esegue l'operazione di failback per il volume con ID 12345678.

### bluemix sl block replica-failover
{: #sl_block_replica_failover}

Failover di un volume di blocchi per uno specifico volume di replica.
```
bluemix sl block replica-failover ID_VOLUME ID_REPLICA
```


**Esempi**:
```
bluemix sl block replica-failover 12345678 87654321
```
Questo comando esegue l'operazione di failover per il volume con ID 12345678 nel volume di replica con ID 87654321.

### bluemix sl block replica-locations
{: #sl_block_replica_locations}

Elenca i datacenter di replica appropriati per lo specifico volume.
```
bluemix sl block replica-locations ID_VOLUME
```


**Esempi**:
```
bluemix sl block replica-locations 12345678
```
Questo comando elenca i datacenter di replica appropriati per il volume di blocchi con ID 12345678.

### bluemix sl block replica-order
{: #sl_block_replica_order}

Ordina un volume di replica dell'archiviazione blocchi.
```
bluemix sl block replica-order ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea da utilizzare per la replica; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter per la replica, ad es. dal09.</dd>
<dt>-t, --tier</dt>
<dd>Facoltativo. Livello archiviazione durata (IOPS per GB) del volume primario per cui è ordinata la replica; le opzioni sono: 0.25,2,4,10; se non si specifica un livello, verrà utilizzato il livello del volume originale.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100; se non si specifica l'IOPS, verrà utilizzato il volume originale.</dd>
<dt>-o, --os-type</dt>
<dd>Facoltativo. Tipo di sistema operativo (es. LINUX) del volume primario per cui è ordinata la replica; le opzioni sono: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
Questo comando ordina una replica per il volume con ID 12345678, che esegue la replica giornaliera (DAILY); è ubicato in dal09, il livello è 4, il tipo di SO è Linux.

### bluemix sl block replica-partners
{: #sl_block_replica_partners}

Elenca i volumi di replica esistenti per un volume di blocchi.
```
bluemix sl block replica-partners ID_VOLUME [OPZIONI]
```


**Esempi**:
```
bluemix sl block replica-partners 12345678
```
Questo comando elenca i volumi di replica esistenti per il volume di blocchi con ID 12345678.

### bluemix sl block snapshot-cancel
{: #sl_block_snapshot_cancel}

Annulla uno spazio dell'istantanea esistente per un volume fornito.
```
bluemix sl block snapshot-cancel ID_ISTANTANEA [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--reason</dt>
<dd>Un motivo facoltativo per l'annullamento.</dd>
<dt>--immediate</dt>
<dd>Annulla lo spazio dell'istantanea immediatamente invece che a una ricorrenza di fatturazione.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-cancel 12345678 --immediate -f
```
Questo comando annulla l'istantanea con ID 12345678 immediatamente senza richiedere la conferma.

### bluemix sl block snapshot-create
{: #sl_block_snapshot_create}

Crea un'istantanea su un volume fornito.
```
bluemix sl block snapshot-create ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Note da impostare sulla nuova istantanea.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
Questo comando crea un'istantanea per il volume con ID 12345678 e con una nota aggiunta come snapshotforbluemix.

### bluemix sl block snapshot-disable
{: #sl_block_snapshot_disable}

Disabilita le istantanee nella pianificazione specificata per un volume fornito.
```
bluemix sl block snapshot-disable ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-disable 12345678 -s DAILY
```
Questo comando disabilita l'istantanea giornaliera per il volume con ID 12345678.

### bluemix sl block snapshot-enable
{: #sl_block_snapshot_enable}

Abilita le istantanee per un volume fornito sulla pianificazione specificata.
```
bluemix sl block snapshot-enable ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Obbligatorio. Numero di istantanee da conservare.</dd>
<dt>-m, --minute</dt>
<dd>Minuto dell'ora in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 59.</dd>
<dt>-r, --hour</dt>
<dd>Ora del giorno in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Giorno della settimana in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 6. 0 indica domenica, 1 indica lunedì, 2 indica martedì, 3 indica mercoledì, 4 indica giovedì, 5 indica venerdì, 6 indica sabato.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
Questo comando abilita l'istantanea per il volume con ID 12345678, l'istantanea viene acquisita settimanalmente ogni domenica alle 2:00 e vengono conservate fino a 5 istantanee.

### bluemix sl block snapshot-delete
{: #sl_block_snapshot_delete}

Elimina un'istantanea su un volume fornito.
```
bluemix sl block snapshot-delete ID_ISTANTANEA
```


**Esempi**:
```
bluemix sl block snapshot-delete 12345678
```
Questo comando elimina l'istantanea con ID 12345678.

### bluemix sl block snapshot-list
{: #sl_block_snapshot_list}

Elenca le istantanee dell'archiviazione blocchi.
```
bluemix sl block snapshot-list ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,name,created,size_bytes.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-list 12345678 --sortby id
```
Questo comando elenca tutte le istantanee del volume con ID 12345678 e le ordina in base all'ID.

### bluemix sl block snapshot-order
{: #sl_block_snapshot_order}

Ordina lo spazio dell'istantanea per un volume dell'archiviazione blocchi.
```
bluemix sl block snapshot-order ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Obbligatorio. Dimensione dello spazio dell'istantanea da creare in GB.</dd>
<dt>-t, --tier</dt>
<dd>Facoltativo. Livello archiviazione durata (IOPS per GB) di un volume di blocchi per cui è ordinato lo spazio; le opzioni sono: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Contrassegno per indicare che l'ordine è un aggiornamento.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
Questo comando ordina lo spazio dell'istantanea per il volume con ID 12345678, la dimensione è 1000 GB, la classe di livello è 4 IOPS per GB.

### bluemix sl block snapshot-restore
{: #sl_block_snapshot_restore}

Ripristina il volume dei blocchi utilizzando un'istantanea fornita.
```
bluemix sl block snapshot-restore ID_VOLUME ID_ISTANTANEA
```


**Esempi**:
```
bluemix sl block snapshot-restore 12345678 87654321
```
Questo comando ripristina il volume con ID 12345678 dall'istantanea con ID 87654321.

### bluemix sl block volume-cancel
{: #sl_block_volume_cancel}

Annulla un volume di archiviazione blocchi esistente.
```
bluemix sl block volume-cancel ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--reason</dt>
<dd>Un motivo facoltativo per l'annullamento.</dd>
<dt>--immediate</dt>
<dd>Annulla il volume di archiviazione blocchi immediatamente invece che a una ricorrenza di fatturazione.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block volume-cancel 12345678 --immediate -f
```
Questo comando annulla il volume con ID 12345678 immediatamente e senza richiedere conferma.

### bluemix sl block volume-list
{: #sl_block_volume_list}

Elenca l'archiviazione blocchi.
```
bluemix sl block volume-list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filtra per nome utente del volume.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtra per nome breve del datacenter.</dd>
<dt>-t, --storage-type</dt>
<dd>Filtra in base al tipo di volume di archiviazione; le opzioni sono: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato l'archiviazione blocchi.</dd>
<dt>--sortby</dt>
<dd>Colonna da ordinare, le opzioni sono: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, active_transactions, created_by.</dd>
<dt>--columns</dt>
<dd>Colonne da visualizzare, le opzioni sono: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, created_by.</dd>
</dl>

**Esempi**:
```
bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
Questo comando elenca i volumi di durata sull'account corrente ubicati in dal09 e li ordina per capacità.

### bluemix sl block volume-detail
{: #sl_block_volume_detail}

Visualizza i dettagli per un volume specificato.
```
bluemix sl block volume-detail ID_VOLUME
```


**Esempi**:
```
bluemix sl block volume-detail 12345678
```
Questo comando mostra i dettagli del volume con ID 12345678.

### bluemix sl block volume-duplicate
{: #sl_block_volume_duplicate}

Ordina un volume di blocchi duplicando un volume esistente.
```
bluemix sl block volume-duplicate ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID di un'istantanea del volume di origine da utilizzare per la duplicazione.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Dimensione del volume di blocchi duplicato in GB; se non si specifica alcuna dimensione, verrà utilizzata la dimensione del volume originale.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100; se non viene specificato un IOPS, verrà utilizzato l'IOPS del volume originale.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Livello archiviazione durata, se non si specifica un livello, verrà utilizzato il livello del volume originale.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>La dimensione dello spazio dell'istantanea da ordinare per il duplicato; se non si specifica alcuna dimensione di spazio dell'istantanea, verrà utilizzata la dimensione di spazio istantanea del volume di origine.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block volume-duplicate 12345678
```
Questo comando mostra come ordinare un nuovo volume duplicando il volume con ID 12345678.

### bluemix sl block volume-order
{: #sl_block_volume_order}

Ordina un volume di archiviazione blocchi.
```
bluemix sl block volume-order [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Obbligatorio. Tipo del volume di archiviazione; le opzioni sono: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Obbligatorio. Dimensione del volume di archiviazione in GB.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100 [obbligatorio per storage-type performance].</dd>
<dt>-e, --tier</dt>
<dd>Livello archiviazione durata (IOPS per GB) [obbligatorio per storage-type endurance]; le opzioni sono: 0.25,2,4,10.</dd>
<dt>-o, --os-type</dt>
<dd>Obbligatorio. Sistema operativo; le opzioni sono: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter.</dd>
<dt>-n, --snapshot-size</dt>
<dd>Parametro facoltativo per l'ordinamento dello spazio dell'istantanea insieme all'archiviazione blocchi della durata; specifica la dimensione (in GB) dello spazio dell'istantanea da ordinare.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
Questo comando ordina un volume delle prestazioni con dimensione di 1000 GB, IOPS di 4000, tipo di SO LINUX, ubicato in dal09.

### bluemix sl block volume-options
{: #sl_block_volume_options}

Elenca tutte le opzioni per ordinare un'archiviazione blocchi.
```
bluemix sl block volume-options
```


**Esempi**:
```
bluemix sl block volume-options
```
Questo comando elenca tutte le opzioni per la creazione di un volume di archiviazione blocchi, inclusi il tipo di archiviazione, la dimensione del volume, il tipo di SO, l'IOPS, la classe di livello, il datacenter e la dimensione dell'istantanea.

### bluemix sl cdn cancel
{: #sl_cdn_cancel}

Annulla un account CDN.
```
bluemix sl cdn cancel ID_ACCOUNT [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>
### bluemix sl cdn detail
{: #sl_cdn_detail}

Fornisce i dettagli di un account CDN.
```
bluemix sl cdn detail ID_ACCOUNT
```

### bluemix sl cdn list
{: #sl_cdn_list}

Elenca tutti gli account CDN.
```
bluemix sl cdn list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id, name, type, created.</dd>
<dt>--order</dt>
<dd>Filtra in base all'ID ordine.</dd>
</dl>
### bluemix sl cdn load
{: #sl_cdn_load}

Memorizza in cache uno o più file su tutti i nodi edge.
```
bluemix sl cdn load ID_ACCOUNT URL_CONTENUTO [URL_CONTENUTO...]
```

### bluemix sl cdn order
{: #sl_cdn_order}

Ordina un account CDN.
```
bluemix sl cdn order [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-b, --bandwidth</dt>
<dd>Larghezza di banda CDN, verrà utilizzato il prezzo 'Pagamento a consumo', se non specificato.</dd>
<dt>-s, --storage</dt>
<dd>Archiviazione CDN, verrà utilizzato il prezzo 'Pagamento a consumo', se non specificato.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>
### bluemix sl cdn options
{: #sl_cdn_options}

Opzioni di larghezza di banda e archiviazione per ordinare l'account CDN.
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add
{: #sl_cdn_origin_add}

Crea un'associazione del pull di origine.
```
bluemix sl cdn origin-add ID_ACCOUNT URL_CONTENUTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-t, --type</dt>
<dd>Il tipo di elemento multimediale per questa associazione (http, flash, wm, ...); il valore predefinito è: http.</dd>
<dt>-c, --cname</dt>
<dd>Un CNAME facoltativo da collegare all'associazione.</dd>
</dl>
### bluemix sl cdn origin-list
{: #sl_cdn_origin_list}

Elenca le associazioni del pull di origine.
```
bluemix sl cdn origin-list ID_ACCOUNT
```

### bluemix sl cdn origin-remove
{: #sl_cdn_origin_remove}

Rimuove un'associazione del pull di origine.
```
bluemix sl cdn origin-remove ID_ACCOUNT ID_ORIGINE [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>
### bluemix sl cdn purge
{: #sl_cdn_purge}

Elimina i file memorizzati nella cache da tutti i nodi edge.
```
bluemix sl cdn purge ID_ACCOUNT URL_CONTENUTO [URL_CONTENUTO...][OPTIONS]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>
### bluemix sl file access-authorize
{: #sl_file_access_authorize}

Autorizza gli host ad accedere a un volume fornito.
```
bluemix sl file access-authorize ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>L'ID di un server hardware da autorizzare.</dd>
<dt>-v, --virtual-id</dt>
<dd>L'ID di un server virtuale da autorizzare.</dd>
<dt>-i, --ip-address-id</dt>
<dd>L'ID di un indirizzo IP da autorizzare.</dd>
<dt>-p, --ip-address</dt>
<dd>Un indirizzo IP da autorizzare.</dd>
<dt>-s, --subnet-id</dt>
<dd>Un ID di una sottorete da autorizzare.</dd>
</dl>

**Esempi**:
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
Questo comando autorizza il server virtuale con ID 87654321 ad accedere al volume con ID 12345678.

### bluemix sl file access-list
{: #sl_file_access_list}

Elenca gli ACL.
```
bluemix sl file access-list ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Colonne da visualizzare; le opzioni sono: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Esempi**:
```
bluemix sl file access-list 12345678 --sortby id
```
Questo comando elenca tutti gli host autorizzati ad accedere al volume con ID 12345678 e li ordina in base all'ID.

### bluemix sl file access-revoke
{: #sl_file_access_revoke}

Revoca l'autorizzazione per gli host che accedono a un volume fornito.
```
bluemix sl file access-revoke ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>L'ID di un server hardware da revocare.</dd>
<dt>-v, --virtual-id</dt>
<dd>L'ID di un server virtuale da revocare.</dd>
<dt>-i, --ip-address-id</dt>
<dd>L'ID di un indirizzo IP da revocare.</dd>
<dt>-p, --ip-address</dt>
<dd>Un indirizzo IP da revocare.</dd>
<dt>-s, --subnet-id</dt>
<dd>Un ID di una sottorete da revocare.</dd>
</dl>

**Esempi**:
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
Questo comando revoca l'accesso del server virtuale con ID 87654321 al volume con ID 12345678.

### bluemix sl file replica-failback
{: #sl_file_replica_failback}

Failback di un volume di file dalla replica.
```
bluemix sl file replica-failback ID_VOLUME
```


**Esempi**:
```
bluemix sl file replica-failback 12345678
```
Questo comando esegue l'operazione di failback per il volume con ID 12345678.

### bluemix sl file replica-failover
{: #sl_file_replica_failover}

Failover di un volume di file per un volume di replica fornito.
```
bluemix sl file replica-failover ID_VOLUME ID_REPLICA
```


**Esempi**:
```
bluemix sl file replica-failover 12345678 87654321
```
Questo comando esegue l'operazione di failover per il volume con ID 12345678 nel volume di replica con ID 87654321.

### bluemix sl file replica-locations
{: #sl_file_replica_locations}

Elenca i datacenter di replica appropriati per il volume fornito.
```
bluemix sl file replica-locations ID_VOLUME
```


**Esempi**:
```
bluemix sl file replica-locations 12345678
```
Questo comando elenca i datacenter di replica appropriati per il volume di file con ID 12345678.

### bluemix sl file replica-order
{: #sl_file_replica_order}

Ordina un volume di replica dell'archiviazione file.
```
bluemix sl file replica-order ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea da utilizzare per la replica; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter per la replica, ad es. dal09.</dd>
<dt>-t, --tier</dt>
<dd>Facoltativo. Livello archiviazione durata (IOPS per GB) del volume primario per cui è ordinata la replica; le opzioni sono: 0.25,2,4,10; se non si specifica un livello, verrà utilizzato il livello del volume originale.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100; se non si specifica l'IOPS, verrà utilizzato il volume originale.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
Questo comando ordina una replica per il volume con ID 12345678, che esegue la replica giornaliera (DAILY); è ubicato in dal09, il livello è 4.

### bluemix sl file replica-partners
{: #sl_file_replica_partners}

Elenca i volumi di replica esistenti per un volume di file.
```
bluemix sl file replica-partners ID_VOLUME [OPZIONI]
```


**Esempi**:
```
bluemix sl file replica-partners 12345678
```
Questo comando elenca i volumi di replica esistenti per il volume di file con ID 12345678.

### bluemix sl file snapshot-cancel
{: #sl_file_snapshot_cancel}

Annulla uno spazio dell'istantanea esistente per un volume fornito.
```
bluemix sl file snapshot-cancel ID_ISTANTANEA [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--reason</dt>
<dd>Un motivo facoltativo per l'annullamento.</dd>
<dt>--immediate</dt>
<dd>Annulla lo spazio dell'istantanea immediatamente invece che a una ricorrenza di fatturazione.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
Questo comando annulla l'istantanea con ID 12345678 immediatamente senza richiedere la conferma.

### bluemix sl file snapshot-create
{: #sl_file_snapshot_create}

Crea un'istantanea su un volume fornito.
```
bluemix sl file snapshot-create ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Note da impostare sulla nuova istantanea.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
Questo comando crea un'istantanea per il volume con ID 12345678 e con una nota aggiunta come snapshotforbluemix.

### bluemix sl file snapshot-disable
{: #sl_file_snapshot_disable}

Disabilita le istantanee nella pianificazione specificata per un volume fornito.
```
bluemix sl file snapshot-disable ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
Questo comando disabilita l'istantanea giornaliera per il volume con ID 12345678.

### bluemix sl file snapshot-enable
{: #sl_file_snapshot_enable}

Abilita le istantanee per un volume fornito sulla pianificazione specificata.
```
bluemix sl file snapshot-enable ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Obbligatorio. Pianificazione dell'istantanea; le opzioni sono: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Obbligatorio. Numero di istantanee da conservare.</dd>
<dt>-m, --minute</dt>
<dd>Minuto dell'ora in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 59.</dd>
<dt>-r, --hour</dt>
<dd>Ora del giorno in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Giorno della settimana in cui dovrebbero essere acquisite le istantanee, numero intero compreso tra 0 e 6. 0 indica domenica, 1 indica lunedì, 2 indica martedì, 3 indica mercoledì, 4 indica giovedì, 5 indica venerdì, 6 indica sabato.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
Questo comando abilita l'istantanea per il volume con ID 12345678, l'istantanea viene acquisita settimanalmente ogni domenica alle 2:00 e vengono conservate fino a 5 istantanee.

### bluemix sl file snapshot-delete
{: #sl_file_snapshot_delete}

Elimina un'istantanea su un volume fornito.
```
bluemix sl file snapshot-delete ID_ISTANTANEA
```


**Esempi**:
```
bluemix sl file snapshot-delete 12345678
```
Questo comando elimina l'istantanea con ID 12345678.

### bluemix sl file snapshot-list
{: #sl_file_snapshot_list}

Elenca le istantanee dell'archiviazione file.
```
bluemix sl file snapshot-list ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,name,created,size_bytes.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-list 12345678 --sortby id
```
Questo comando elenca tutte le istantanee del volume con ID 12345678 e le ordina in base all'ID.

### bluemix sl file snapshot-order
{: #sl_file_snapshot_order}

Ordina lo spazio dell'istantanea per un volume dell'archiviazione file.
```
bluemix sl file snapshot-order ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Obbligatorio. Dimensione dello spazio dell'istantanea da creare in GB.</dd>
<dt>-t, --tier</dt>
<dd>Facoltativo. Livello archiviazione durata (IOPS per GB) del volume di file per cui è ordinato lo spazio; le opzioni sono: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Contrassegno per indicare che l'ordine è un aggiornamento.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
Questo comando ordina lo spazio dell'istantanea per il volume con ID 12345678, la dimensione è 1000GB, la classe di livello è 4 IOPS per GB.

### bluemix sl file snapshot-restore
{: #sl_file_snapshot_restore}

Ripristina il volume di file utilizzando un'istantanea fornita.
```
bluemix sl file snapshot-restore ID_VOLUME ID_ISTANTANEA
```


**Esempi**:
```
bluemix sl file snapshot-restore 12345678 87654321
```
Questo comando ripristina il volume con ID 12345678 dall'istantanea con ID 87654321.

### bluemix sl file volume-cancel
{: #sl_file_volume_cancel}

Annulla un volume di archiviazione file esistente.
```
bluemix sl file volume-cancel ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--reason</dt>
<dd>Un motivo facoltativo per l'annullamento.</dd>
<dt>--immediate</dt>
<dd>Annulla il volume di archiviazione file immediatamente invece che a una ricorrenza di fatturazione.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
Questo comando annulla il volume con ID 12345678 immediatamente e senza richiedere conferma.

### bluemix sl file volume-list
{: #sl_file_volume_list}

Elenca l'archiviazione file.
```
bluemix sl file volume-list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filtra per nome utente del volume.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtra per nome breve del datacenter.</dd>
<dt>-t, --storage-type</dt>
<dd>Filtra in base al tipo di volume di archiviazione; le opzioni sono: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato l'archiviazione file.</dd>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,active_transactions,mount_addr.</dd>
<dt>--columns</dt>
<dd>Colonne da visualizzare; le opzioni sono: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,mount_addr.</dd>
</dl>

**Esempi**:
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
Questo comando elenca i volumi di durata sull'account corrente ubicati in dal09 e li ordina per capacità.

### bluemix sl file volume-detail
{: #sl_file_volume_detail}

Visualizza i dettagli per un volume specificato.
```
bluemix sl file volume-detail ID_VOLUME
```


**Esempi**:
```
bluemix sl file volume-detail 12345678
```
Questo comando mostra i dettagli del volume con ID 12345678.

### bluemix sl file volume-duplicate
{: #sl_file_volume_duplicate}

Ordina un volume di file duplicando un volume esistente.
```
bluemix sl file volume-duplicate ID_VOLUME [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID di un'istantanea del volume originale da utilizzare per la duplicazione.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Dimensione del volume di file duplicato in GB; se non si specifica alcuna dimensione, verrà utilizzata la dimensione del volume originale.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100; se non viene specificato un IOPS, verrà utilizzato l'IOPS del volume originale.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Livello archiviazione durata, se non si specifica un livello, verrà utilizzato il livello del volume originale.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>La dimensione dello spazio dell'istantanea da ordinare per il duplicato; se non si specifica alcuna dimensione di spazio dell'istantanea, verrà utilizzata la dimensione di spazio istantanea del volume originale.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file volume-duplicate 12345678
```
Questo comando mostra come ordinare un nuovo volume duplicando il volume con ID 12345678.

### bluemix sl file volume-order
{: #sl_file_volume_order}

Ordina un volume di archiviazione file.
```
bluemix sl file volume-order [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Obbligatorio. Tipo del volume di archiviazione; le opzioni sono: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Obbligatorio. Dimensione del volume di archiviazione in GB.</dd>
<dt>-i, --iops</dt>
<dd>IOPS archiviazione prestazioni, compreso tra 100 e 6000 in multipli di 100 [obbligatorio per storage-type performance].</dd>
<dt>-e, --tier</dt>
<dd>Livello archiviazione durata (IOPS per GB) [obbligatorio per storage-type endurance]; le opzioni sono: 0.25,2,4,10.</dd>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter.</dd>
<dt>-n, --snapshot-size</dt>
<dd>Parametro facoltativo per l'ordinamento dello spazio dell'istantanea con il volume.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
Questo comando ordina un volume delle prestazioni con dimensione di 1000GB, IOPS di 4000, ubicato in dal09.

### bluemix sl file volume-options
{: #sl_file_volume_options}

Elenca tutte le opzioni per l'ordinamento di un'archiviazione file.
```
bluemix sl file volume-options
```


**Esempi**:
```
bluemix sl file volume-options
```
Questo comando elenca tutte le opzioni per la creazione di un volume di archiviazione file, inclusi il tipo di archiviazione, la dimensione del volume, gli IOPS, la classe di livello, il datacenter e la dimensione dell'istantanea.

### bluemix sl dns import
{: #sl_dns_import}

Importa una zona in base a un file di zona BIND.
```
bluemix sl dns import FILEDIZONA [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--dry-run</dt>
<dd>Non creare al momento i record.</dd>
</dl>

**Esempi**:
```
bluemix sl dns import ~/blumix.net.txt
```
Questo comando importa la zona e i suoi record della risorsa dal file: ~/blumix.net.txt.

### bluemix sl dns record-add
{: #sl_dns_record_add}

Aggiungi il record della risorsa in una zona.
```
bluemix sl dns record-add ZONA RECORD TIPO DATI [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--ttl</dt>
<dd>Valore TTL (Time-To-Live) in secondi, come: 86400; il valore predefinito è: 7200.</dd>
</dl>

**Esempi**:
```
bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
Questo comando aggiunge un record A alla zona: bluemix.net; il relativo host è "ftp", i dati sono "127.0.0.1" e TTL è 86400 secondi.

### bluemix sl dns record-edit
{: #sl_dns_record_edit}

Aggiorna i record della risorsa in una zona.
```
bluemix sl dns record-edit ZONE [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--by-record</dt>
<dd>Modifica per record host, ad esempio www.</dd>
<dt>--by-id</dt>
<dd>Modifica un solo record dal suo ID</dd>
<dt>--data</dt>
<dd>Dati di record, ad esempio un indirizzo IP.</dd>
<dt>--ttl</dt>
<dd>Valore TTL in secondi, ad esempio: 86400.</dd>
</dl>

**Esempi**:
```
bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
Questo comando modifica i record nella zona: bluemix.net, dove l'ID è 12345678 e imposta i suoi dati su "127.0.0.2" e ttl su 3600.

### bluemix sl dns record-list
{: #sl_dns_record_list}

Elenca tutti i record di risorsa in una zona.
```
bluemix sl dns record-list ZONE [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--data</dt>
<dd>Filtra per dati di record, ad esempio un indirizzo IP.</dd>
<dt>--record</dt>
<dd>Filtra per record host, ad esempio www.</dd>
<dt>--ttl</dt>
<dd>Filtra per valore TTL in secondi, ad esempio 86400.</dd>
<dt>--type</dt>
<dd>Filtra in base al tipo di record, ad esempio A o CNAME.</dd>
</dl>

**Esempi**:
```
bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
Questo comando elenca tutti i record A nella zona: bluemix.net, il filtro in base all'host è elasticsearch e ttl è 900 secondi.

### bluemix sl dns record-remove
{: #sl_dns_record_remove}

Rimuovi record della risorsa da una zona.
```
bluemix sl dns record-remove ID_RECORD
```


**Esempi**:
```
bluemix sl dns record-remove 12345678
```
Questo comando rimuove il record della risorsa con ID 12345678.

### bluemix sl dns zone-create
{: #sl_dns_zone_create}

Crea una zona.
```
bluemix sl dns zone-create ZONE
```


**Esempi**:
```
bluemix sl dns zone-create bluemix.net
```
Questo comando crea una zona denominata bluemix.net.

### bluemix sl dns zone-delete
{: #sl_dns_zone_delete}

Elimina una zona.
```
bluemix sl dns zone-delete ZONE
```


**Esempi**:
```
bluemix sl dns zone-delete bluemix.net
```
Questo comando elimina una zona denominata bluemix.net.

### bluemix sl dns zone-list
{: #sl_dns_zone_list}

Elenca tutte le zone nel tuo account.
```
bluemix sl dns zone-list
```


**Esempi**:
```
bluemix sl dns zone-list
```
Questo comando elenca tutte le zone nell'account corrente.

### bluemix sl dns zone-print
{: #sl_dns_zone_print}

Stampa i record di risorsa e zona in formato BIND.
```
bluemix sl dns zone-print ZONA
```


**Esempi**:
```
bluemix sl dns zone-print bluemix.net
```
Questo comando stampa la zona denominata bluemix.net in formato BIND.

### bluemix sl globalip create
{: #sl_globalip_create}

Crea un IP globale.
```
bluemix sl globalip create [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--v6</dt>
<dd>Ordina un indirizzo IP IPv6.</dd>
<dt>--test</dt>
<dd>Verifica l'ordine.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl globalip create --v6
```
Questo comando crea un indirizzo IP V6.

### bluemix sl globalip assign
{: #sl_globalip_assign}

Assegna un IP globale a un router o a un dispositivo di destinazione.
```
bluemix sl globalip assign IDENTIFICATIVO DESTINAZIONE
```


**Esempi**:
```
bluemix sl globalip assign 12345678 9.111.123.456
```
Questo comando assegna l'indirizzo IP con ID 12345678 a un dispositivo di destinazione il cui indirizzo IP è 9.111.123.456.

### bluemix sl globalip cancel
{: #sl_globalip_cancel}

Annulla un IP globale.
```
bluemix sl globalip cancel IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl globalip cancel 12345678
```
Questo comando annulla l'indirizzo IP con ID 12345678.

### bluemix sl globalip list
{: #sl_globalip_list}

Elenca tutti gli IP globali nel tuo account.
```
bluemix sl globalip list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--v4</dt>
<dd>Visualizza solo gli IP IPv4.</dd>
<dt>--v6</dt>
<dd>Visualizza solo gli IP IPv6.</dd>
<dt>--order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato questo indirizzo IP.</dd>
</dl>

**Esempi**:
```
bluemix sl globalip list --v4
```
Questo comando elenca tutti gli indirizzi IP V4 sull'account corrente.

### bluemix sl globalip unassign
{: #sl_globalip_unassign}

Annulla l'assegnazione di un IP globale da un router o un dispositivo di destinazione.
```
bluemix sl globalip unassign IDENTIFICATIVO
```


**Esempi**:
```
bluemix sl globalip unassign 12345678
```
Questo comando annulla l'assegnazione dell'indirizzo IP con ID 12345678 dal dispositivo di destinazione.

### bluemix sl image delete
{: #sl_image_delete}

Elimina un'immagine.
```
bluemix sl image delete IDENTIFICATIVO
```
**Esempi**:
```
   bluemix sl image delete 12345678
```
Questo comando elimina l'immagine con ID `12345678`.

### bluemix sl image detail
{: #sl_image_detail}

Ottiene i dettagli per un'immagine.
```
bluemix sl image detail IDENTIFICATIVO
```
**Esempi**:
```
 bluemix sl image detail 12345678
```
Questo comando ottiene i dettagli per l'immagine con ID 12345678.

### bluemix sl image edit
{: #sl_image_edit}

Modifica i dettagli di un'immagine.
```
bluemix sl image edit IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--name</dt>
<dd>Nome dell'immagine.</dd>
<dt>--note</dt>
<dd>Nota supplementare per l'immagine.</dd>
<dt>--tag</dt>
<dd>Le tag per l'immagine.</dd>
</dl>

*Esempi**:
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
Questo comando modifica l'immagine con ID `12345678` e imposta il suo nome su `ubuntu16`, la nota su `testing` e la tag su `staging`.

### bluemix sl image list
{: #sl_image_list}

Elenca tutte le immagini nel tuo account.
```
bluemix sl image list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--name</dt>
<dd>Filtra il nome dell'immagine.</dd>
<dt>--public</dt>
<dd>Visualizza solo le immagini pubbliche.</dd>
<dt>--private</dt>
<dd>Visualizza solo le immagini private.</dd>
</dl>

### bluemix sl ipsec cancel
{: #sl_ipsec_cancel}

Annulla un contesto tunnel IPSec VPN.
```
bluemix sl ipsec cancel ID_CONTESTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--immediate</dt>
<dd>Annulla l'IPSec immediatamente invece che a una ricorrenza di fatturazione.</dd>
<dt>--reason</dt>
<dd>Un motivo facoltativo per l'annullamento.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl ipsec config
{: #sl_ipsec_config}

Richiede la configurazione di un contesto tunnel.
```
bluemix sl ipsec config ID_CONTESTO [OPZIONI]
```

### bluemix sl ipsec detail
{: #sl_ipsec_detail}

Elenca i dettagli del contesto tunnel IPSec VPN.
```
bluemix sl ipsec detail ID_CONTESTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-i, --include</dt>
<dd>Include risorse aggiuntive; le opzioni sono: at,is,rs,sr,ss.</dd>
</dl>
### bluemix sl ipsec list
{: #sl_ipsec_list}

Elenca i contesti tunnel IPSec VPN.
```
bluemix sl ipsec list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato l'IPSEC.</dd>
</dl>
### bluemix sl ipsec order
{: #sl_ipsec_order}

Ordina un tunnel IPSec VPN.
```
bluemix sl ipsec order [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter per l'IPSEC, ad es. dal09.</dd>
</dl>

### bluemix sl ipsec subnet-add
{: #sl_ipsec_subnet_add}

Aggiunge una sottorete a un contesto tunnel IPSec.
```
bluemix sl ipsec subnet-add ID_CONTESTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --subnet-id</dt>
<dd>Identificativo di sottorete da aggiungere (obbligatorio).</dd>
<dt>-t, --subnet-type</dt>
<dd>Tipo di sottorete da aggiungere (obbligatorio); le opzioni sono: internal,remote,service.</dd>
<dt>-n, --network</dt>
<dd>Identificativo di rete della sottorete da creare.</dd>
</dl>

### bluemix sl ipsec subnet-remove
{: #sl_ipsec_subnet_remove}

Rimuove una sottorete da un contesto tunnel IPSEC.
```
bluemix sl ipsec subnet-remove ID_CONTESTO ID_SOTTORETE TIPO_SOTTORETE [OPZIONI]
```

### bluemix sl ipsec translation-add
{: #sl_ipsec_translation_add}

Aggiunge una conversione di indirizzo a un tunnel IPSec.
```
bluemix sl ipsec translation-add ID_CONTESTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Indirizzo IP statico (obbligatorio).</dd>
<dt>-r, --remote-ip</dt>
<dd>Indirizzo IP remoto (obbligatorio).</dd>
<dt>-n, --note</dt>
<dd>Nota.</dd>
</dl>
### bluemix sl ipsec translation-remove
{: #sl_ipsec_translation_remove}

Rimuove una voce di conversione da un IPSec.
```
bluemix sl ipsec translation-remove ID_CONTESTO ID_CONVERSIONE [OPZIONI]
```

### bluemix sl ipsec translation-update
{: #sl_ipsec_translation_update}

Aggiorna una conversione di indirizzo per un IPSec.
```
bluemix sl ipsec translation-update ID_CONTESTO ID_CONVERSIONE [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Indirizzo IP statico (obbligatorio).</dd>
<dt>-r, --remote-ip</dt>
<dd>Indirizzo IP remoto (obbligatorio).</dd>
<dt>-n, --note</dt>
<dd>Nota.</dd>
</dl>
### bluemix sl ipsec update
{: #sl_ipsec_update}

Aggiorna proprietà del contesto tunnel.
```
bluemix sl ipsec update ID_CONTESTO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Nome descrittivo.</dd>
<dt>-r, --remote-peer</dt>
<dd>Indirizzo IP peer remoto.</dd>
<dt>-k, --preshared-key</dt>
<dd>Chiave precondivisa.</dd>
<dt>-a, --phase1-auth</dt>
<dd>Autenticazione fase 1; le opzioni sono: MD5,SHA1,SHA256.</dd>
<dt>-c, --phase1-crypto</dt>
<dd>Crittografia fase 1; le opzioni sono: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-d, --phase1-dh</dt>
<dd>Gruppo diffie hellman fase 1; le opzioni sono: 0,1,2,5.</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>Durata chiave fase 1; l'intervallo è 120-172800.</dd>
<dt>-u, --phase2-auth</dt>
<dd>Autenticazione fase 2; le opzioni sono: MD5,SHA1,SHA256.</dd>
<dt>-y, --phase2-crypto</dt>
<dd>Crittografia fase 2; le opzioni sono: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-e, --phase2-dh</dt>
<dd>Gruppo diffie hellman fase 2; le opzioni sono: 0,1,2,5.</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>PFC (perfect forward secrecy) fase 2; l'intervallo è 0-1.</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>Durata chiave fase 2; l'intervallo è 120-172800.</dd>
</dl>

### bluemix sl loadbal cancel
{: #sl_loadbal_cancel}

Annulla un programma di bilanciamento del carico esistente.
```
bluemix sl loadbal cancel ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl loadbal create
{: #sl_loadbal_create}

Aggiunge un programma di bilanciamento del carico con l'ID restituito da create-options.
```
bluemix sl loadbal create ID_PREZZO UBICAZIONE [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl loadbal create-options
{: #sl_loadbal_create_options}

Ottiene le opzioni di prezzo con cui creare un programma di bilanciamento del carico.
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail
{: #sl_loadbal_detail}

Ottiene i dettagli del programma di bilanciamento del carico.
```
bluemix sl loadbal detail ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO
```

### bluemix sl loadbal group-add
{: #sl_loadbal_group_add}

Aggiunge un nuovo servizio di programma di bilanciamento del carico (load_balancer).
```
bluemix sl loadbal group-add ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Obbligatorio. La percentuale allocata di connessioni.</dd>
<dt>-p, --port</dt>
<dd>Obbligatorio. Il numero di porta.</dd>
<dt>-t, --routing-type</dt>
<dd>Obbligatorio. L'ID del tipo di instradamento. Esegui 'bluemix sl loadbal routing-types' per trovare un ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Obbligatorio. L'ID del metodo di instradamento. Esegui 'bluemix sl loadbal routing-methods' per trovare un ID.</dd>
</dl>

### bluemix sl loadbal group-delete
{: #sl_loadbal_group_delete}

Elimina un gruppo di servizi di programma di bilanciamento del carico esistente.
```
bluemix sl loadbal group-delete ID_GRUPPO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl loadbal group-edit
{: #sl_loadbal_group_edit}

Modifica un gruppo di servizi di programma di bilanciamento del carico esistente.
```
bluemix sl loadbal group-edit ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO ID_GRUPPO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Modifica la percentuale allocata di connessioni.</dd>
<dt>-p, --port</dt>
<dd>Modifica il numero di porta.</dd>
<dt>-t, --routing-type</dt>
<dd>Modifica l'ID del tipo di instradamento. Esegui 'bluemix sl loadbal routing-types' per trovare un ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Modifica l'ID del metodo di instradamento. Esegui 'bluemix sl loadbal routing-methods' per trovare un ID.</dd>
</dl>

### bluemix sl loadbal group-reset
{: #sl_loadbal_group_reset}

Reimposta le connessioni su uno specifico gruppo di servizi.
```
bluemix sl loadbal group-reset ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO ID_GRUPPO
```

### bluemix sl loadbal health-checks
{: #sl_loadbal_health_checks}

Elenca i tipi di controllo di integrità.
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list
{: #sl_loadbal_list}

Elenca i programmi di bilanciamento del carico attivi.
```
bluemix sl loadbal list
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Filtra per nome breve del datacenter.</dd>
<dt>-o, --order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato il programma di bilanciamento del carico.</dd>
<dt>-p, --ip-address</dt>
<dd>Filtra in base all'indirizzo IP.</dd>
</dl>
### bluemix sl loadbal routing-methods
{: #sl_loadbal_routing_methods}

Elenca i metodi di instradamento.
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types
{: #sl_loadbal_routing_types}

Elenca i tipi di instradamento.
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add
{: #sl_loadbal_service_add}

Aggiunge un nuovo servizio di programma di bilanciamento del carico.
```
bluemix sl loadbal service-add ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO ID_GRUPPO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--disabled</dt>
<dd>Facoltativo. Crea il servizio come disabilitato; se non viene specificato, il valore predefinito è abilitato.</dd>
<dt>-p, --port</dt>
<dd>Obbligatorio. Il numero di porta per il servizio.</dd>
<dt>-w, --weight</dt>
<dd>Obbligatorio. Il peso del servizio.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Obbligatorio. Il tipo di controllo di integrità.</dd>
<dt>-i, --ip-address</dt>
<dd>Obbligatorio. L'indirizzo IP del servizio.</dd>
</dl>

### bluemix sl loadbal service-delete
{: #sl_loadbal_service_delete}

Elimina un servizio di programma di bilanciamento del carico esistente.
```
bluemix sl loadbal service-delete ID_SERVIZIO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl loadbal service-edit
{: #sl_loadbal_service_edit}

Modifica le proprietà di un gruppo di servizi.
```
bluemix sl loadbal service-edit ID_PROGRAMMA_DI_BILANCIAMENTO_DEL_CARICO ID_SERVIZIO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--disabled</dt>
<dd>Disabilita il servizio.</dd>
<dt>--enabled</dt>
<dd>Abilita il servizio.</dd>
<dt>-p, --port</dt>
<dd>Modifica il numero di porta per il servizio.</dd>
<dt>-w, --weight</dt>
<dd>Modifica il peso del servizio.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Modifica il tipo di controllo di integrità.</dd>
<dt>-i, --ip-address</dt>
<dd>Modifica l'indirizzo IP del servizio.</dd>
</dl>

### bluemix sl loadbal service-toggle
{: #sl_loadbal_service_toggle}

Alterna lo stato di un servizio di programma di bilanciamento del carico esistente.
```
bluemix sl loadbal service-toggle ID_SERVIZIO
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

### bluemix sl security sshkey-add
{: #sl_security_sshkey_add}

Aggiunge una nuova chiave SSH.
```
bluemix sl security sshkey-add ETICHETTA [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --in-file</dt>
<dd>Il file id_rsa.pub da importare per questa chiave.</dd>
<dt>-k, --key</dt>
<dd>La chiave SSH effettiva.</dd>
<dt>--note</dt>
<dd>Nota aggiuntiva che verrà associata alla chiave.</dd>
</dl>

**Esempi**:
```
bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
Questo comando aggiunge una chiave SSH dal file: ~/.ssh/id_rsa.pub con una nota "mykey".

### bluemix sl security sshkey-edit
{: #sl_security_sshkey_edit}

Modifica una chiave SSH.
```
bluemix sl security sshkey-edit IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--label</dt>
<dd>La nuova etichetta per la chiave.</dd>
<dt>--note</dt>
<dd>Nuove note per la chiave.</dd>
</dl>

**Esempi**:
```
bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
Questo comando aggiorna la chiave SSH con ID 12345678 e imposta l'etichetta su "Bluemix" e la nota su "testing".

### bluemix sl security sshkey-list
{: #sl_security_sshkey_list}

Elenca le chiavi SSH sul tuo account.
```
bluemix sl security sshkey-list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,label,fingerprint,notes.</dd>
</dl>

**Esempi**:
```
bluemix sl security sshkey-list --sortby label
```
Questo comando elenca tutte le chiavi SSH sull'account corrente e le ordina per etichetta.

### bluemix sl security sshkey-print
{: #sl_security_sshkey_print}

Stampa una chiave SSH a schermo.
```
bluemix sl security sshkey-print IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --out-file</dt>
<dd>La chiave SSH pubblica verrà scritta in questo file.</dd>
</dl>

**Esempi**:
```
bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
Questo comando mostra l'ID, l'etichetta e le note della chiave SSH con ID 12345678 e scrive la chiave pubblica nel file: ~/mykey.pub.

### bluemix sl security sshkey-remove
{: #sl_security_sshkey_remove}

Rimuove in modo permanente una chiave SSH.
```
bluemix sl security sshkey-remove IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl security sshkey-remove 12345678 -f
```
Questo comando rimuove la chiave SSH con ID 12345678 senza richiedere conferma.

### bluemix sl security cert-add
{: #sl_security_cert_add}

Aggiunge e carica i dettagli del certificato SSL.
```
bluemix sl security cert-add [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--crt</dt>
<dd>File del certificato.</dd>
<dt>--csr</dt>
<dd>File di richiesta di firma certificato.</dd>
<dt>--icc</dt>
<dd>File del certificato intermedio.</dd>
<dt>--key</dt>
<dd>File della chiave privata</dd>
<dt>--notes</dt>
<dd>Note aggiuntive.</dd>
</dl>

**Esempi**:
```
bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key
```
Questo comando aggiunge il file del certificato: ~/bluemix.net.cert e il file della chiave privata  ~/bluemix.net.key per il dominio bluemix.net.

### bluemix sl security cert-edit
{: #sl_security_cert_edit}

Modifica il certificato SSL.
```
bluemix sl security cert-edit IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--crt</dt>
<dd>File del certificato.</dd>
<dt>--csr</dt>
<dd>File di richiesta di firma certificato.</dd>
<dt>--icc</dt>
<dd>File del certificato intermedio.</dd>
<dt>--key</dt>
<dd>File della chiave privata</dd>
<dt>--notes</dt>
<dd>Note aggiuntive.</dd>
</dl>

**Esempi**:
```
bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
Questo comando modifica il certificato con ID 12345678 e aggiorna la sua chiave privata con il file: ~/bluemix.net.key.

### bluemix sl security cert-download
{: #sl_security_cert_download}

Scarica il certificato SSL e i file chiave.
```
bluemix sl security cert-download IDENTIFICATIVO
```


**Esempi**:
```
bluemix sl security cert-download 12345678
```
Questo comando scarica 4 file nella directory corrente per il certificato con ID 12345678. I 4 file sono: il file del certificato, il file della richiesta di firma del certificato, il file del certificato intermedio e il file della chiave privata.

### bluemix sl security cert-list
{: #sl_security_cert_list}

Elenca i certificati SSL sul tuo account.
```
bluemix sl security cert-list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--status</dt>
<dd>Mostra i certificati con questo stato; il valore predefinito è: all; le opzioni sono: all,valid,expired.</dd>
<dt>--sortby</dt>
<dd>Colonna in base a cui ordinare; le opzioni sono: id,common_name,days_until_expire,notes.</dd>
</dl>

**Esempi**:
```
bluemix sl security cert-list --status valid --sortby days_until_expire
```
Questo comando elenca tutti i certificati validi sull'account corrente e li ordina per giorni di validità.

### bluemix sl security cert-remove
{: #sl_security_cert_remove}

Rimuove il certificato SSL.
```
bluemix sl security cert-remove IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl security cert-remove 12345678
```
Questo comando rimuove il certificato con ID 12345678.

### bluemix sl subnet cancel
{: #sl_subnet_cancel}

Annulla una sottorete.
```
bluemix sl subnet cancel IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl subnet cancel 12345678 -f
```
Questo comando annulla la sottorete con ID 12345678 senza richiedere conferma.

### bluemix sl subnet create
{: #sl_subnet_create}

Aggiunge una nuova sottorete al tuo account.
```
bluemix sl subnet create QUANTITÀ RETE ID_VLAN [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--v6, --ipv6</dt>
<dd>Ordina indirizzi IPv6.</dd>
<dt>--test</dt>
<dd>Non ordinare la sottorete; ottieni solo un preventivo.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl subnet create public 16 567
```
Questo comando crea una sottorete pubblica con 16 indirizzi IP v4 e la posiziona nella vlan con ID 567.

### bluemix sl subnet detail
{: #sl_subnet_detail}

Ottiene i dettagli di una sottorete.
```
bluemix sl subnet detail IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Nascondi elenco server virtuali.</dd>
<dt>--no-hardware</dt>
<dd>Nascondi elenco hardware.</dd>
</dl>

**Esempi**:
```
bluemix sl subnet detail 12345678
```
Questo comando mostra informazioni dettagliate sulla sottorete con ID 12345678, incluse le informazioni sui server virtuali e i server hardware.

### bluemix sl subnet list
{: #sl_subnet_list}

Elenca tutte le sottoreti sul tuo account.
```
bluemix sl subnet list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna da ordinare. Le opzioni sono: id,identifier,type,network_space,datacenter,vlan_id,IPs,hardware,vs.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtra per nome breve del datacenter.</dd>
<dt>--identifier</dt>
<dd>Filtra per identificativo di rete.</dd>
<dt>-t, --subnet-type</dt>
<dd>Filtra per tipo di sottorete.</dd>
<dt>--network-space</dt>
<dd>Filtra per spazio di rete.</dd>
<dt>--v4, --ipv4</dt>
<dd>Visualizza solo le sottoreti IPv4.</dd>
<dt>--v6, --ipv6</dt>
<dd>Visualizza solo le sottoreti IPv6.</dd>
<dt>--order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato le sottoreti.</dd>
</dl>

**Esempi**:
```
bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
Questo comando elenca le sottoreti IP V4 sull'account corrente eseguendo il filtro per il datacenter dal09, il tipo di sottorete è PRIMARY e lo spazio di rete è PUBLIC.

### bluemix sl subnet lookup
{: #sl_subnet_lookup}

Trova un indirizzo IP e visualizza le relative informazioni su sottorete e dispositivo.
```
bluemix sl subnet lookup INDIRIZZO_IP
```


**Esempi**:
```
bluemix sl subnet lookup 9.125.235.255
```
Questo comando trova il record dell'indirizzo IP con indirizzo 9.125.235.255 e ne visualizza le informazioni su sottorete e dispositivo.

### bluemix sl vlan create
{: #sl_vlan_create}

Crea una nuova VLAN.
```
bluemix sl vlan create [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-t, --vlan-type</dt>
<dd>Il tipo della VLAN, pubblica o privata.</dd>
<dt>-r, --router</dt>
<dd>Il nome host del router.</dd>
<dt>-d, --datacenter</dt>
<dd>Il nome breve del datacenter.</dd>
<dt>-s, --size</dt>
<dd>La dimensione delle sottoreti, le opzioni sono: 8 (5 IP utilizzabili), 16 (13 IP utilizzabili) o 32 (29 IP utilizzabili).</dd>
<dt>-n, --name</dt>
<dd>Il nome della VLAN.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
Questo comando crea una vlan pubblica ubicata nel datacenter dal09 con 16 indirizzi IP e con il nome myvlan.

### bluemix sl vlan cancel
{: #sl_vlan_cancel}

Annulla una VLAN.
```
bluemix sl vlan cancel IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vlan cancel 12345678 -f
```
Questo comando annulla la vlan con ID 12345678 senza richiedere conferma.

### bluemix sl vlan detail
{: #sl_vlan_detail}

Ottiene i dettagli relativi a una VLAN.
```
bluemix sl vlan detail IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Nascondi elenco server virtuali.</dd>
<dt>--no-hardware</dt>
<dd>Nascondi elenco hardware.</dd>
</dl>

**Esempi**:
```
bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
Questo comando mostra i dettagli della vlan con ID 12345678 e non elenca il server virtuale o il server hardware.

### bluemix sl vlan edit
{: #sl_vlan_edit}

Modifica i dettagli relativi a una VLAN.
```
bluemix sl vlan edit IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Il nome della VLAN.</dd>
</dl>

**Esempi**:
```
bluemix sl vlan edit 12345678 -n myvlan-rename
```
Questo comando aggiorna la vlan con ID 12345678 e le fornisce un nuovo nome "myvlan-rename".

### bluemix sl vlan list
{: #sl_vlan_list}

Elenca tutte le VLAN sul tuo account.
```
bluemix sl vlan list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--sortby</dt>
<dd>Colonna da ordinare, le opzioni sono: id, number, name, firewall, datacenter, hardware, virtual_servers, public_ips.</dd>
<dt>-d, --datacenter</dt>
<dd>Filtra per nome breve del datacenter.</dd>
<dt>-n, --number</dt>
<dd>Filtra in base al numero della VLAN.</dd>
<dt>--name</dt>
<dd>Filtra in base al nome della VLAN.</dd>
<dt>--order</dt>
<dd>Filtra in base all'ID dell'ordine che ha acquistato la VLAN.</dd>
</dl>

**Esempi**:
```
bluemix sl vlan list -d dal09 --sortby number
```
Questo comando elenca tutte le vlan sull'account corrente eseguendo il filtro per un datacenter uguale a dal09 e le ordina per numero di vlan.

### bluemix sl vlan options
{: #sl_vlan_options}

Elenca tutte le opzioni per creare la VLAN.
```
bluemix sl vlan options
```


**Esempi**:
```
bluemix sl vlan options
```
Questo comando elenca tutte le opzioni per creare una VLAN, ad es. tipo di vlan, datacenter, dimensione della sottorete, router ecc.

### bluemix sl vs cancel
{: #sl_vs_cancel}

Annulla l'istanza del server virtuale.
```
bluemix sl vs cancel IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs cancel 12345678
```
Questo comando annulla l'istanza del server virtuale con ID 12345678.

### bluemix sl vs capture
{: #sl_vs_capture}

Acquisisce l'istanza del server virtuale in un'immagine.
```
bluemix sl vs capture IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Obbligatorio. Nome dell'immagine.</dd>
<dt>--all</dt>
<dd>Acquisisce tutti i dischi appartenenti al server virtuale.</dd>
<dt>--note</dt>
<dd>Aggiunge una nota da associare all'immagine.</dd>
</dl>

**Esempi**:
```
bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
Questo comando acquisisce l'istanza del server virtuale con ID 12345678 con tutti i dischi in un'immagine denominata "mybluemix" con la nota "testing".

### bluemix sl vs create
{: #sl_vs_create}

Crea un'istanza del server virtuale.
```
bluemix sl vs create [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-H, --hostname</dt>
<dd>Obbligatorio. Parte host dell'FQDN.</dd>
<dt>-D, --domain</dt>
<dd>Obbligatorio. Parte dominio dell'FQDN</dd>
<dt>-c, --cpu</dt>
<dd>Obbligatorio. Numero di core della CPU.</dd>
<dt>-m, --memory</dt>
<dd>Obbligatorio. Memoria in megabyte.</dd>
<dt>-d, --datacenter</dt>
<dd>Obbligatorio. Nome breve del datacenter.</dd>
<dt>-o, --os</dt>
<dd>Codice di installazione SO. Suggerimento: puoi specificare <OS>_LATEST.</dd>
<dt>--image</dt>
<dd>ID immagine. Vedi: 'bluemix sl image list' per riferimento.</dd>
<dt>--billing</dt>
<dd>Frequenza di fatturazione. Il valore predefinito è: hourly. Le opzioni sono: hourly, monthly.</dd>
<dt>--dedicated</dt>
<dd>Crea un server virtuale dedicato (nodo privato).</dd>
<dt>--san</dt>
<dd>Utilizza l'archiviazione SAN invece del disco locale.</dd>
<dt>--test</dt>
<dd>Non creare effettivamente il server virtuale.</dd>
<dt>--export</dt>
<dd>Esporta le opzioni in un file modello.</dd>
<dt>-i, --postinstall</dt>
<dd>Script di post installazione da scaricare.</dd>
<dt>-k, --key</dt>
<dd>Gli ID delle chiavi SSH da aggiungere all'utente root (più ricorrenze consentite).</dd>
<dt>--disk</dt>
<dd>Dimensioni disco (più ricorrenze consentite).</dd>
<dt>--private</dt>
<dd>Forza il server virtuale ad avere accesso solo alla rete privata.</dd>
<dt>--like</dt>
<dd>Utilizza la configurazione da un server virtuale esistente.</dd>
<dt>-n, --network</dt>
<dd>Velocità della porta di rete in Mbps.</dd>
<dt>--tag</dt>
<dd>Tag da aggiungere all'istanza (più ricorrenze consentite).</dd>
<dt>-t, --template</dt>
<dd>Un file modello che specifica i valori predefiniti delle opzioni della riga di comando.</dd>
<dt>-u, --userdata</dt>
<dd>Stringa di metadati definita dall'utente.</dd>
<dt>-F, --userfile</dt>
<dd>Leggi dati utente dal file.</dd>
<dt>--vlan-public</dt>
<dd>L'ID della VLAN pubblica in cui desideri venga posizionato il server virtuale.</dd>
<dt>--vlan-private</dt>
<dd>L'ID della VLAN privata in cui desideri venga posizionato il server virtuale-</dd>
<dt>--wait</dt>
<dd>Attendi finché il server virtuale non ha terminato il provisioning fino a X secondi prima di ritornare.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
Questo comando ordina un'istanza del server virtuale con nome host myvsi, dominio bluemix.net, 4 core della cpu, 4096M di memoria, ubicata nel datacenter: dal10,

### bluemix sl vs options
{: #sl_vs_options}

Elenca le opzioni per creare l'istanza del server virtuale.
```
bluemix sl vs options [OPZIONI]
```


**Esempi**:
```
bluemix sl vs options
```
Questo comando elenca tutte le opzioni per creare un'istanza del server virtuale, ad es. datacenter, cpu, memoria, sistema operativo, disco, velocità della rete ecc.

### bluemix sl vs credentials
{: #sl_vs_credentials}

Elenca le credenziali dell'istanza del server virtuale.
```
bluemix sl vs credentials IDENTIFICATIVO [OPZIONI]
```


**Esempi**:
```
bluemix sl vs credentials 12345678
```
Questo comando elenca tutte le coppie di nome utente e password dell'istanza del server virtuale con ID 12345678.

### bluemix sl vs detail
{: #sl_vs_detail}

Ottiene i dettagli per un'istanza del server virtuale.
```
bluemix sl vs detail IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--passwords</dt>
<dd>Mostra le password (fai attenzione a occhi indiscreti)..</dd>
<dt>--price</dt>
<dd>Mostra i prezzi associati.</dd>
</dl>

**Esempi**:
```
bluemix sl vs details 12345678
```
Questo comando elenca informazioni dettagliate sull'istanza del server virtuale con ID 12345678.

### bluemix sl vs dns-sync
{: #sl_vs_dns_sync}

Sincronizza i record DNS per un'istanza del server virtuale.
```
bluemix sl vs dns-sync IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-a, --a-record</dt>
<dd>Sincronizza il record A per l'host</dd>
<dt>--aaaa-record</dt>
<dd>Sincronizza il record AAAA per l'host.</dd>
<dt>--ptr</dt>
<dd>Sincronizza il record PTR per l'host.</dd>
<dt>--ttl</dt>
<dd>Imposta il TTL per i record A e/o PTR; il valore predefinito è: 7200.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
Questo comando sincronizza il record A (indirizzo IP V4) dell'istanza del server virtuale con ID 12345678 con il server DNS e imposta il ttl di questo record A su 3600.

### bluemix sl vs edit
{: #sl_vs_edit}

Modifica i dettagli di un'istanza del server virtuale.
```
bluemix sl vs edit IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-D, --domain</dt>
<dd>Parte dominio dell'FQDN</dd>
<dt>-H, --hostname</dt>
<dd>Parte host dell'FQDN. Esempio: server.</dd>
<dt>--tag</dt>
<dd>Tag da impostare o stringa vuota per rimuovere tutto.</dd>
<dt>-u, --userdata</dt>
<dd>Stringa di metadati definita dall'utente.</dd>
<dt>-F, --userfile</dt>
<dd>Leggi dati utente dal file.</dd>
<dt>--public-speed</dt>
<dd>Velocità della porta pubblica; le opzioni sono: 0,10,100,1000,10000.</dd>
<dt>--private-speed</dt>
<dd>Velocità della porta privata; le opzioni sono: 0,10,100,1000,10000.</dd>
</dl>

**Esempi**:
```
bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
Questo comando aggiorna l'istanza del server virtuale con ID 12345678 e ne imposta il dominio su "bluemix.net", il nome host su "myapp" e la tag su "testcli",

### bluemix sl vs list
{: #sl_vs_list}

Elenca le istanze del server virtuale sul tuo account.
```
bluemix sl vs list [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Numero di core della CPU.</dd>
<dt>-D, --domain</dt>
<dd>Parte dominio dell'FQDN</dd>
<dt>-d, --datacenter</dt>
<dd>Nome breve del datacenter.</dd>
<dt>-H, --hostname</dt>
<dd>Parte host dell'FQDN.</dd>
<dt>-m, --memory</dt>
<dd>Memoria in megabyte.</dd>
<dt>-n, --network</dt>
<dd>Velocità della porta di rete in Mbps.</dd>
<dt>--hourly</dt>
<dd>Mostra solo le istanze orarie.</dd>
<dt>--monthly</dt>
<dd>Mostra solo le istanze mensili.</dd>
<dt>--tag</dt>
<dd>Filtra in base alle tag (sono consentite più ricorrenze).</dd>
<dt>--sortby</dt>
<dd>Colonna da ordinare, le opzioni sono: id, hostname, domain, datacenter, cpu, memory, primary_ip, backend_ip. Il valore predefinito è: hostname.</dd>
<dt>--columns</dt>
<dd>Colonne da visualizzare, le opzioni sono: guid, primary_ip, backend_ip, datacenter, action, power_state, created_by, tags. Il valore predefinito è: id,hostname,primary_ip,backend_ip,datacenter,action.</dd>
</dl>

**Esempi**:
```
bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
Questo comando elenca tutte le istanze del server virtuale con fatturazione oraria sull'account corrente filtrando per dominio uguale a "bluemix.net" e ordinandole per memoria.

### bluemix sl vs pause
{: #sl_vs_pause}

Mette in pausa un'istanza del server virtuale attiva.
```
bluemix sl vs pause IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs pause 12345678 -f
```
Questo comando mette in pausa l'istanza del server virtuale con ID 12345678 senza richiedere conferma.

### bluemix sl vs power-off
{: #sl_vs_power_off}

Spegne un'istanza del server virtuale attiva.
```
bluemix sl vs power-off IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--hard</dt>
<dd>Esegue un arresto forzato.</dd>
<dt>--soft</dt>
<dd>Esegue un arresto non forzato.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs power-off 12345678 --soft
```
Questo comando esegue un arresto semplice dell'istanza del server virtuale con ID 12345678.

### bluemix sl vs power-on
{: #sl_vs_power_on}

Accende un'istanza del server virtuale.
```
bluemix sl vs power-on IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs power-on 12345678
```
Questo comando esegue un avvio dell'istanza del server virtuale con ID 12345678.

### bluemix sl vs ready
{: #sl_vs_ready}

Controlla se un'istanza del server virtuale è pronta per l'uso.
```
bluemix sl vs ready IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--wait</dt>
<dd>Attendi finché il server virtuale non ha terminato il provisioning fino a X secondi prima di ritornare.</dd>
</dl>

**Esempi**:
```
bluemix sl vs ready 12345678 --wait 30
```
Questo comando verifica lo stato dell'istanza del server virtuale con ID 12345678 per vedere se è pronta per l'utilizzo continuo e attende fino a 30 secondi.

### bluemix sl vs reboot
{: #sl_vs_reboot}

Riavvia un'istanza del server virtuale attiva.
```
bluemix sl vs reboot IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>--hard</dt>
<dd>Esegue un riavvio forzato.</dd>
<dt>--soft</dt>
<dd>Esegue un riavvio forzato.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs reboot 12345678 --hard
```
Questo comando esegue un riavvio forzato dell'istanza del server virtuale con ID 12345678.

### bluemix sl vs reload
{: #sl_vs_reload}

Ricarica il sistema operativo su un'istanza del server virtuale.
```
bluemix sl vs reload IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-i, --postinstall</dt>
<dd>Script di post installazione da scaricare.</dd>
<dt>--image</dt>
<dd>ID immagine. L'impostazione predefinita è l'utilizzo del sistema operativo corrente.</dd>
<dt>Vedi:</dt>
<dd>'bluemix sl image list' per riferimento.</dd>
<dt>-k, --key</dt>
<dd>Gli ID delle chiavi SSH da aggiungere all'utente root (più ricorrenze consentite).</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs reload 12345678
```
Questo comando ricarica il sistema operativo corrente per l'istanza del server virtuale con ID 12345678.

### bluemix sl vs rescue
{: #sl_vs_rescue}

Riavvia un'istanza del server virtuale in un'immagine di salvataggio.
```
bluemix sl vs rescue IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs rescue 12345678
```
Questo comando riavvia l'istanza del server virtuale con ID 12345678 in un'immagine di salvataggio.

### bluemix sl vs resume
{: #sl_vs_resume}

Ripristina un'istanza del server virtuale messa in pausa.
```
bluemix sl vs resume IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs resume 12345678
```
Questo comando riprende l'istanza del server virtuale con ID 12345678.

### bluemix sl vs upgrade
{: #sl_vs_upgrade}

Aggiorna un'istanza del server virtuale.
```
bluemix sl vs upgrade IDENTIFICATIVO [OPZIONI]
```

<strong>Opzioni comando</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Numero di core della CPU.</dd>
<dt>--private</dt>
<dd>Il core della CPU sarà su un server host dedicato</dd>
<dt>-m, --memory</dt>
<dd>Memoria in megabyte.</dd>
<dt>--network</dt>
<dd>Velocità della porta di rete in Mbps.</dd>
<dt>-f, --force</dt>
<dd>Forza l'operazione senza conferma.</dd>
</dl>

**Esempi**:
```
bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
Questo comando aggiorna l'istanza del server virtuale con ID 12345678 e imposta il numero di core della CPU su 8, la memoria su 8192M e la velocità della porta di rete su 1000 Mbps.

