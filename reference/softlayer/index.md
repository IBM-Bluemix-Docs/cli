---

copyright:

  years: 2016,2017

lastupdated: "2017-11-10"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) commands
{: #softlayer_cli}

The {{site.data.keyword.BluSoftlayer}} plugin has been merged into the {{site.data.keyword.Bluemix_notm}} CLI. You no longer need to install the plug-in.

Use {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands in the {{site.data.keyword.Bluemix_notm}} command line interface (CLI) to configure and manage SoftLayer services.


To get started, install the IBM {{site.data.keyword.Bluemix_notm}} CLI. See
[Bluemix CLI ![External link icon](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window} for details.

For a complete list of {{site.data.keyword.Bluemix_notm}} commands, see: [{{site.data.keyword.Bluemix_notm}} (bx) commands](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)


## General {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands

The following commands are supported. Use the `bluemix sl` command to see the list of available commands:

<table summary="Alphabetically ordered general commands that have links that bring you to more info for the command">
<caption>Table 1. General {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands</caption>
 <thead>
 <th colspan="6">General {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## {{site.data.keyword.BluSoftlayer_notm}} infrastructure Block storage commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 2. {{site.data.keyword.BluSoftlayer_notm}} infrastructure Block storage</caption>
 <thead>
 <th colspan="6">Softlayer Block storage</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} infrastructure CDN commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 3. {{site.data.keyword.BluSoftlayer_notm}} infrastructure CDN</caption>
 <thead>
 <th colspan="6">Softlayer CDN</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure File stoarge commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 4. {{site.data.keyword.BluSoftlayer_notm}} infrastructure File storage</caption>
 <thead>
 <th colspan="6">Softlayer File storage</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure DNS commands

<table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 5. {{site.data.keyword.BluSoftlayer_notm}} infrastructure DNS commands</caption>
 <thead>
 <th colspan="6">Softlayer DNS commands</th>
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

<table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 6. {{site.data.keyword.BluSoftlayer_notm}} infrastructure Global IP commands</caption>
 <thead>
 <th colspan="6">Softlayer Global IP commands</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure image commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 7. {{site.data.keyword.BluSoftlayer_notm}} infrastructure image commands</caption>
 <thead>
 <th colspan="6">Softlayer image commands</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} infrastructure IPSec VPN commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 7. {{site.data.keyword.BluSoftlayer_notm}} infrastructure IPSec VPN commands</caption>
 <thead>
 <th colspan="6">Softlayer IPSec VPN commands</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} infrastructure Load Balancer commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 8. {{site.data.keyword.BluSoftlayer_notm}} infrastructure Load Balancer commands</caption>
 <thead>
 <th colspan="6">Softlayer Load Balancer commands</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure security commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 9. {{site.data.keyword.BluSoftlayer_notm}} infrastructure security commands</caption>
 <thead>
 <th colspan="5">Softlayer security commands</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure subnet commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 10. {{site.data.keyword.BluSoftlayer_notm}} infrastructure subnet commands</caption>
 <thead>
 <th colspan="5">Softlayer subnet commands</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure virtual server commands

 <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 11. {{site.data.keyword.BluSoftlayer_notm}} infrastructure virtual server commands</caption>
 <thead>
 <th colspan="6">Softlayer virtual server commands</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} infrastructure VLAN commands

  <table summary="Alphabetically ordered general {{site.data.keyword.BluSoftlayer_notm}} infrastructure commands that have links that bring you to more info for the command">
<caption>Table 12. {{site.data.keyword.BluSoftlayer_notm}} infrastructure VLAN commands</caption>
 <thead>
 <th colspan="6">Softlayer VLAN commands</th>
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

### Command usage
To view help information for the commands, run: `bluemix sl [command] -h`.

### bluemix sl init
{: #sl_init}

Initialize the configuration settings that are used to connect to the SoftLayer environment. The configuration includes user name, API key or password, account and endpoint.
```
bluemix sl init [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-a, --api-endpoint</dt>
<dd>Softlayer API endpoint URL, default is: https://api.softlayer.com/rest/v3.1 for {{site.data.keyword.BluSoftlayer_notm}} infrastructure API key authentication, https://api.softlayer.com/mobile/v3.1 for IBMid authentication.</dd>
<dt>-u, --sl-user</dt>
<dd>Softlayer user name.</dd>
<dt>-p, --sl-password</dt>
<dd>Softlayer password or API key.</dd>
<dt>-c, --account-id</dt>
<dd>Softlayer account ID.</dd>
<dt>-q, --security-question-id</dt>
<dd>Security question Id used to authenticate, ask your account owner if you do not know.</dd>
<dt>-w, --security-question-answer</dt>
<dd>Security question answer used to authenticate, ask your account owner if you do not know.</dd>
<dt>-s, --security-code</dt>
<dd>Security code generated by security vendor when 2-factor authentication is enabled.</dd>
<dt>-v, --security-vendor</dt>
<dd>Security vendor that provides security code for authentication, options are: VERISIGN,TOTP,PHONE_FACTOR.</dd>
<dt>-t, --auth-token</dt>
<dd>Authentication token when phone authentication is enabled.</dd>
</dl>

For example, login with {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name and password/API key
```
$ bluemix sl config
Choose how to configure {{site.data.keyword.BluSoftlayer_notm}} infrastructure authentication:
1. Login with {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name and password/API key
2. Use {{site.data.keyword.Bluemix_notm}} Single-Sign-On
Enter a number>1
Softlayer API endpoint URL: [https://api.softlayer.com/rest/v3.1]>
Username: []> wangjunl@cn.ibm.com
API key or password: []> abcd

Softlayer API endpoint:    https://api.softlayer.com/rest/v3.1   
Account ID:                278444   
User ID:                   wangjunl@cn.ibm.com   
API Key:                   xxxxxxxxxx
```
For example, use {{site.data.keyword.Bluemix_notm}} Single-Sign-On to login Softlayer
```
$ bx login -a api.ng.bluemix.net -u wangjunl@cn.ibm.com -p xxxxxxx -c 65ce8074c6c62b5
API endpoint: api.ng.bluemix.net
Authenticating...
OK

Targeted account Wilma's Account (65ce8074c6c62b5)

API endpoint:   https://api.ng.bluemix.net (API version: 2.54.0)   
Region:         us-south   
User:           wangjunl@cn.ibm.com   
Account:        Wilma's Account (65ce8074c6c62b5)   
No org or space targeted, use 'bx target --cf or bx target -o ORG -s SPACE'

Tip: use 'bx cf <command>' to run the Cloud Foundry CLI with {{site.data.keyword.Bluemix_notm}} CLI context.
```

$ bx sl init
Choose how to configure {{site.data.keyword.BluSoftlayer_notm}} infrastructure authentication:
1. Login with {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name and password/API key
2. Use {{site.data.keyword.Bluemix_notm}} Single-Sign-On
Enter a number> 2
Softlayer API endpoint URL: [https://api.softlayer.com/mobile/v3.1]> 
Setting account to: 278444
OK
                              
Softlayer API endpoint:    https://api.softlayer.com/mobile/v3.1   
Account ID:                278444   
User ID:                   12345678   
IMS token:                 xxxxxxxxxx
```

### bluemix sl help
{: #sl_help}

View help information for all commands to operate {{site.data.keyword.BluSoftlayer_notm}} infrastructure environment.
```
bluemix sl help

```

### bluemix sl block access-authorize 
{: #sl_block_access_authorize} 

Authorize hosts to access a given volume.
```
bluemix sl block access-authorize VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>The ID of one hardware server to authorize.</dd>
<dt>-v, --virtual-id</dt>
<dd>The ID of one virtual server to authorize.</dd>
<dt>-i, --ip-address-id</dt>
<dd>The ID of one IP address to authorize.</dd>
<dt>-p, --ip-address</dt>
<dd>An IP address to authorize.</dd>
</dl>

**Examples**:
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
This command authorizes virtual server with ID 87654321 to access volume with ID 12345678.

### bluemix sl block access-list 
{: #sl_block_access_list} 

List ACLs.
```
bluemix sl block access-list VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Columns to display, options are: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Examples**:
```
bluemix sl block access-list 12345678 --sortby id
```
This command lists all hosts that are authorized to access volume with ID 12345678 and sorts them by ID.

### bluemix sl block access-revoke 
{: #sl_block_access_revoke} 

Revoke authorization for hosts accessing a given volume.
```
bluemix sl block access-revoke VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>The ID of one hardware server to revoke.</dd>
<dt>-v, --virtual-id</dt>
<dd>The ID of one virtual server to revoke.</dd>
<dt>-i, --ip-address-id</dt>
<dd>The ID of one IP address to revoke.</dd>
<dt>-p, --ip-address</dt>
<dd>An IP address to revoke.</dd>
</dl>

**Examples**:
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
This command revokes access of virtual server with ID 87654321 to volume with ID 12345678.

### bluemix sl block replica-failback 
{: #sl_block_replica_failback} 

Failback a block volume from replica.
```
bluemix sl block replica-failback VOLUME_ID
```


**Examples**:
```
bluemix sl block replica-failback 12345678
```
This command performs failback operation for volume with ID 12345678.

### bluemix sl block replica-failover 
{: #sl_block_replica_failover} 

Failover a block volume to the given replica volume.
```
bluemix sl block replica-failover VOLUME_ID REPLICA_ID
```


**Examples**:
```
bluemix sl block replica-failover 12345678 87654321
```
This command performs failover operation for volume with ID 12345678 to replica volume with ID 87654321.

### bluemix sl block replica-locations 
{: #sl_block_replica_locations} 

List suitable replication datacenters for the given volume.
```
bluemix sl block replica-locations VOLUME_ID
```


**Examples**:
```
bluemix sl block replica-locations 12345678
```
This command lists suitable replication data centers for block volume with ID 12345678.

### bluemix sl block replica-order 
{: #sl_block_replica_order} 

Order a block storage replica volume.
```
bluemix sl block replica-order VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Required. Snapshot schedule to use for replication, options are: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Required. Short name of the datacenter for the replica, eg. dal09 .</dd>
<dt>-t, --tier</dt>
<dd>Optional. Endurance Storage Tier (IOPS per GB) of the primary volume for which a replica is ordered , options are: 0.25,2,4,10,if no tier is specified, the tier of the original volume will be used.</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100,if no IOPS  is specified, the IOPS  of the original volume will be used.</dd>
<dt>-o, --os-type</dt>
<dd>Optional. Operating System Type (eg. LINUX) of the primary volume for which a replica is ordered , options are: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
This command orders a replica for volume with ID 12345678, which performs DAILY replication, is located at dal09, tier level is 4, OS type is Linux.

### bluemix sl block replica-partners 
{: #sl_block_replica_partners} 

List existing replicant volumes for a block volume.
```
bluemix sl block replica-partners VOLUME_ID [OPTIONS]
```


**Examples**:
```
bluemix sl block replica-partners 12345678
```
This command lists existing replicant volumes for block volume with ID 12345678.

### bluemix sl block snapshot-cancel 
{: #sl_block_snapshot_cancel} 

Cancel existing snapshot space for a given volume.
```
bluemix sl block snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--reason</dt>
<dd>An optional reason for cancellation.</dd>
<dt>--immediate</dt>
<dd>Cancel the snapshot space immediately instead of on the billing anniversary.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-cancel 12345678 --immediate -f
```
This command cancels snapshot with ID 12345678 immediately without asking for confirmation.

### bluemix sl block snapshot-create 
{: #sl_block_snapshot_create} 

Create a snapshot on a given volume.
```
bluemix sl block snapshot-create VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Notes to set on the new snapshot.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
This command creates a snapshot for volume with ID 12345678 and with addition note as snapshotforbluemix.

### bluemix sl block snapshot-disable 
{: #sl_block_snapshot_disable} 

Disable snapshots on the specified schedule for a given volume.
```
bluemix sl block snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Required. Snapshot schedule , options are: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-disable 12345678 -s DAILY
```
This command disables daily snapshot for volume with ID 12345678.

### bluemix sl block snapshot-enable 
{: #sl_block_snapshot_enable} 

Enable snapshots for a given volume on the specified schedule.
```
bluemix sl block snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Required. Snapshot schedule , options are: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Required. Number of snapshots to retain .</dd>
<dt>-m, --minute</dt>
<dd>Minute of the hour when snapshots should be taken, integer between 0 to 59.</dd>
<dt>-r, --hour</dt>
<dd>Hour of the day when snapshots should be taken, integer between 0 to 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Day of the week when snapshots should be taken, integer between 0 to 6. 0 means Sunday,1 means Monday,2 means Tuesday,3 means Wendesday,4 means Thursday,5 means Friday,6 means Saturday.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
This command enables snapshot for volume with ID 12345678, snapshot is taken weekly on every Sunday at 2:00, and up to 5 snapshots are retained.

### bluemix sl block snapshot-delete 
{: #sl_block_snapshot_delete} 

Delete a snapshot on a given volume.
```
bluemix sl block snapshot-delete SNAPSHOT_ID
```


**Examples**:
```
bluemix sl block snapshot-delete 12345678
```
This command deletes snapshot with ID 12345678.

### bluemix sl block snapshot-list 
{: #sl_block_snapshot_list} 

List block storage snapshots.
```
bluemix sl block snapshot-list VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,name,created,size_bytes.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-list 12345678 --sortby id
```
This command lists all snapshots of volume with ID 12345678 and sorts them by ID.

### bluemix sl block snapshot-order 
{: #sl_block_snapshot_order} 

Order snapshot space for a block storage volume.
```
bluemix sl block snapshot-order VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Required. Size of snapshot space to create in GB  .</dd>
<dt>-t, --tier</dt>
<dd>Optional. Endurance Storage Tier (IOPS per GB) of the block volume for which space is ordered , options are: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Flag to indicate that the order is an upgrade.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
This command orders snapshot space for volume with ID 12345678, the size is 1000GB, the tier level is 4 IOPS per GB.

### bluemix sl block snapshot-restore 
{: #sl_block_snapshot_restore} 

Restore block volume using a given snapshot.
```
bluemix sl block snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**Examples**:
```
bluemix sl block snapshot-restore 12345678 87654321
```
This command restores volume with ID 12345678 from snapshot with ID 87654321.

### bluemix sl block volume-cancel 
{: #sl_block_volume_cancel} 

Cancel an existing block storage volume.
```
bluemix sl block volume-cancel VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--reason</dt>
<dd>An optional reason for cancellation.</dd>
<dt>--immediate</dt>
<dd>Cancel the block storage volume immediately instead of on the billing anniversary.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block volume-cancel 12345678 --immediate -f
```
This command cancels volume with ID 12345678 immediately and without asking for confirmation.

### bluemix sl block volume-list 
{: #sl_block_volume_list} 

List block storage.
```
bluemix sl block volume-list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filter by volume username.</dd>
<dt>-d, --datacenter</dt>
<dd>Filter by datacenter shortname.</dd>
<dt>-t, --storage-type</dt>
<dd>Filter by type of storage volume, options are: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filter by ID of the order that purchased the block storage.</dd>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,active_transactions,created_by.</dd>
<dt>--columns</dt>
<dd>Columns to display, options are: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,created_by.</dd>
</dl>

**Examples**:
```
bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
This command lists all endurance volumes on current account that are located at dal09, and sorts them by capacity.

### bluemix sl block volume-detail 
{: #sl_block_volume_detail} 

Display details for a specified volume.
```
bluemix sl block volume-detail VOLUME_ID
```


**Examples**:
```
bluemix sl block volume-detail 12345678
```
This command shows details of volume with ID 12345678.

### bluemix sl block volume-duplicate 
{: #sl_block_volume_duplicate} 

Order a block volume by duplicating an existing volume.
```
bluemix sl block volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID of an origin volume snapshot to use for duplication.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Size of duplicate block volume in GB, if no size is specified, the size of the original volume will be used.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>Performance Storage IOPS, between 100 and 6000 in multiples of 100, if no IOPS  is specified, the IOPS  of the original volume will be used.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Endurance Storage Tier, if no tier is specified, the tier of the original volume will be used.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>The size of snapshot space to order for the duplicate, if no snapshot space size is specified, the snapshot space size of the origin volume will be used.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block volume-duplicate 12345678
```
This command shows order a new volume by duplicating the volume with ID 12345678.

### bluemix sl block volume-order 
{: #sl_block_volume_order} 

Order a block storage volume.
```
bluemix sl block volume-order [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Required. Type of storage volume , options are: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Required. Size of storage volume in GB .</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100 [required for storage-type performance].</dd>
<dt>-e, --tier</dt>
<dd>Endurance Storage Tier (IOP per GB) [required for storage-type endurance], options are: 0.25,2,4,10.</dd>
<dt>-o, --os-type</dt>
<dd>Required. Operating System , options are: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-d, --datacenter</dt>
<dd>Required. Datacenter short name .</dd>
<dt>-n, --snapshot-size</dt>
<dd>Optional parameter for ordering snapshot space along with endurance block storage; specifies the size (in GB) of snapshot space to order.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
This command orders a performance volume with size is 1000GB, IOPS is 4000, OS type is LINUX, located at dal09.

### bluemix sl block volume-options 
{: #sl_block_volume_options} 

List all options for ordering a block storage.
```
bluemix sl block volume-options
```


**Examples**:
```
bluemix sl block volume-options
```
This command lists all options for creating a block storage volume, including storage type, volume size, OS type, IOPS, tier level, datacenter, and snapshot size.

### bluemix sl cdn cancel 
{: #sl_cdn_cancel} 

Cancel a CDN account.
```
bluemix sl cdn cancel ACCOUNT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>
### bluemix sl cdn detail 
{: #sl_cdn_detail} 

Detail a CDN Account.
```
bluemix sl cdn detail ACCOUNT_ID
```

### bluemix sl cdn list 
{: #sl_cdn_list} 

List all CDN accounts.
```
bluemix sl cdn list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id, name, type, created.</dd>
<dt>--order</dt>
<dd>Filter by order ID.</dd>
</dl>
### bluemix sl cdn load 
{: #sl_cdn_load} 

Cache one or more files on all edge nodes.
```
bluemix sl cdn load ACCOUNT_ID CONTENT_URL [CONTENT_URL...]
```

### bluemix sl cdn order 
{: #sl_cdn_order} 

Order a CDN account.
```
bluemix sl cdn order [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-b, --bandwidth</dt>
<dd>CDN bandwidth, 'Pay as You Go' price will be used if not specified.</dd>
<dt>-s, --storage</dt>
<dd>CDN storage, 'Pay as You Go' price will be used if not specified.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>
### bluemix sl cdn options 
{: #sl_cdn_options} 

Bandwidth and storage options for ordering CDN account.
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add 
{: #sl_cdn_origin_add} 

Create an origin pull mapping.
```
bluemix sl cdn origin-add ACCOUNT_ID CONTENT_URL [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-t, --type</dt>
<dd>The media type for this mapping (http, flash, wm, ...), default is: http.</dd>
<dt>-c, --cname</dt>
<dd>An optional CNAME to attach to the mapping.</dd>
</dl>
### bluemix sl cdn origin-list 
{: #sl_cdn_origin_list} 

List origin pull mappings.
```
bluemix sl cdn origin-list ACCOUNT_ID
```

### bluemix sl cdn origin-remove 
{: #sl_cdn_origin_remove} 

Remove an origin pull mapping.
```
bluemix sl cdn origin-remove ACCOUNT_ID ORIGIN_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>
### bluemix sl cdn purge 
{: #sl_cdn_purge} 

Purge cached files from all edge nodes.
```
bluemix sl cdn purge ACCOUNT_ID CONTENT_URL [CONTENT_URL...] [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>
### bluemix sl file access-authorize 
{: #sl_file_access_authorize} 

Authorize hosts to access a given volume.
```
bluemix sl file access-authorize VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>The ID of one hardware server to authorize.</dd>
<dt>-v, --virtual-id</dt>
<dd>The ID of one virtual server to authorize.</dd>
<dt>-i, --ip-address-id</dt>
<dd>The ID of one IP address to authorize.</dd>
<dt>-p, --ip-address</dt>
<dd>An IP address to authorize.</dd>
<dt>-s, --subnet-id</dt>
<dd>An ID of one subnet to authorize.</dd>
</dl>

**Examples**:
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
This command authorizes virtual server with ID 87654321 to access volume with ID 12345678.

### bluemix sl file access-list 
{: #sl_file_access_list} 

List ACLs.
```
bluemix sl file access-list VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>Columns to display, options are: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**Examples**:
```
bluemix sl file access-list 12345678 --sortby id
```
This command lists all hosts that are authorized to access volume with ID 12345678 and sorts them by ID.

### bluemix sl file access-revoke 
{: #sl_file_access_revoke} 

Revoke authorization for hosts accessing a given volume.
```
bluemix sl file access-revoke VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-d, --hardware-id</dt>
<dd>The ID of one hardware server to revoke.</dd>
<dt>-v, --virtual-id</dt>
<dd>The ID of one virtual server to revoke.</dd>
<dt>-i, --ip-address-id</dt>
<dd>The ID of one IP address to revoke.</dd>
<dt>-p, --ip-address</dt>
<dd>An IP address to revoke.</dd>
<dt>-s, --subnet-id</dt>
<dd>An ID of one subnet to revoke.</dd>
</dl>

**Examples**:
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
This command revokes access of virtual server with ID 87654321 to volume with ID 12345678.

### bluemix sl file replica-failback 
{: #sl_file_replica_failback} 

Failback a file volume from replica.
```
bluemix sl file replica-failback VOLUME_ID
```


**Examples**:
```
bluemix sl file replica-failback 12345678
```
This command performs failback operation for volume with ID 12345678.

### bluemix sl file replica-failover 
{: #sl_file_replica_failover} 

Failover a file volume to the given replica volume.
```
bluemix sl file replica-failover VOLUME_ID REPLICA_ID
```


**Examples**:
```
bluemix sl file replica-failover 12345678 87654321
```
This command performs failover operation for volume with ID 12345678 to replica volume with ID 87654321.

### bluemix sl file replica-locations 
{: #sl_file_replica_locations} 

List suitable replication datacenters for the given volume.
```
bluemix sl file replica-locations VOLUME_ID
```


**Examples**:
```
bluemix sl file replica-locations 12345678
```
This command lists suitable replication data centers for file volume with ID 12345678.

### bluemix sl file replica-order 
{: #sl_file_replica_order} 

Order a file storage replica volume.
```
bluemix sl file replica-order VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>Required. Snapshot schedule to use for replication, , options are: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>Required. Short name of the datacenter for the replica, eg. dal09 .</dd>
<dt>-t, --tier</dt>
<dd>Optional. Endurance Storage Tier (IOPS per GB) of the primary volume for which a replica is ordered , options are: 0.25,2,4,10,if no tier is specified, the tier of the original volume will be used.</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100,if no IOPS  is specified, the IOPS  of the original volume will be used.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
This command orders a replica for volume with ID 12345678, which performs DAILY replication, is located at dal09, tier level is 4.

### bluemix sl file replica-partners 
{: #sl_file_replica_partners} 

List existing replicant volumes for a file volume.
```
bluemix sl file replica-partners VOLUME_ID [OPTIONS]
```


**Examples**:
```
bluemix sl file replica-partners 12345678
```
This command lists existing replicant volumes for file volume with ID 12345678.

### bluemix sl file snapshot-cancel 
{: #sl_file_snapshot_cancel} 

Cancel existing snapshot space for a given volume.
```
bluemix sl file snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--reason</dt>
<dd>An optional reason for cancellation.</dd>
<dt>--immediate</dt>
<dd>Cancel the snapshot space immediately instead of on the billing anniversary.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
This command cancels snapshot with ID 12345678 immediately without asking for confirmation.

### bluemix sl file snapshot-create 
{: #sl_file_snapshot_create} 

Create a snapshot on a given volume.
```
bluemix sl file snapshot-create VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-n, --note</dt>
<dd>Notes to set on the new snapshot.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
This command creates a snapshot for volume with ID 12345678 and with addition note as snapshotforbluemix.

### bluemix sl file snapshot-disable 
{: #sl_file_snapshot_disable} 

Disable snapshots on the specified schedule for a given volume.
```
bluemix sl file snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Required. Snapshot schedule , options are: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
This command disables daily snapshot for volume with ID 12345678.

### bluemix sl file snapshot-enable 
{: #sl_file_snapshot_enable} 

Enable snapshots for a given volume on the specified schedule.
```
bluemix sl file snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --schedule-type</dt>
<dd>Required. Snapshot schedule , options are: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>Required. Number of snapshots to retain .</dd>
<dt>-m, --minute</dt>
<dd>Minute of the hour when snapshots should be taken, integer between 0 to 59.</dd>
<dt>-r, --hour</dt>
<dd>Hour of the day when snapshots should be taken, integer between 0 to 23.</dd>
<dt>-d, --day-of-week</dt>
<dd>Day of the week when snapshots should be taken, integer between 0 to 6. 0 means Sunday,1 means Monday,2 means Tuesday,3 means Wendesday,4 means Thursday,5 means Friday,6 means Saturday.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
This command enables snapshot for volume with ID 12345678, snapshot is taken weekly on every Sunday at 2:00, and up to 5 snapshots are retained.

### bluemix sl file snapshot-delete 
{: #sl_file_snapshot_delete} 

Delete a snapshot on a given volume.
```
bluemix sl file snapshot-delete SNAPSHOT_ID
```


**Examples**:
```
bluemix sl file snapshot-delete 12345678
```
This command deletes snapshot with ID 12345678.

### bluemix sl file snapshot-list 
{: #sl_file_snapshot_list} 

List file storage snapshots.
```
bluemix sl file snapshot-list VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,name,created,size_bytes.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-list 12345678 --sortby id
```
This command lists all snapshots of volume with ID 12345678 and sorts them by ID.

### bluemix sl file snapshot-order 
{: #sl_file_snapshot_order} 

Order snapshot space for a file storage volume.
```
bluemix sl file snapshot-order VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --size</dt>
<dd>Required. Size of snapshot space to create in GB  .</dd>
<dt>-t, --tier</dt>
<dd>Optional. Endurance Storage Tier (IOPS per GB) of the file volume for which space is ordered , options are: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100.</dd>
<dt>-u, --upgrade</dt>
<dd>Flag to indicate that the order is an upgrade.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
This commands order snapshot space for volume with ID 12345678, the size is 1000GB, the tier level is 4 IOPS per GB.

### bluemix sl file snapshot-restore 
{: #sl_file_snapshot_restore} 

Restore file volume using a given snapshot.
```
bluemix sl file snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**Examples**:
```
bluemix sl file snapshot-restore 12345678 87654321
```
This command restores volume with ID 12345678 from snapshot with ID 87654321.

### bluemix sl file volume-cancel 
{: #sl_file_volume_cancel} 

Cancel an existing file storage volume.
```
bluemix sl file volume-cancel VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--reason</dt>
<dd>An optional reason for cancellation.</dd>
<dt>--immediate</dt>
<dd>Cancel the file storage volume immediately instead of on the billing anniversary.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
This command cancels volume with ID 12345678 immediately and without asking for confirmation.

### bluemix sl file volume-list 
{: #sl_file_volume_list} 

List file storage.
```
bluemix sl file volume-list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-u, --username</dt>
<dd>Filter by volume username.</dd>
<dt>-d, --datacenter</dt>
<dd>Filter by datacenter shortname.</dd>
<dt>-t, --storage-type</dt>
<dd>Filter by type of storage volume, options are: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>Filter by ID of the order that purchased the file storage.</dd>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,active_transactions,mount_addr.</dd>
<dt>--columns</dt>
<dd>Columns to display, options are: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,mount_addr.</dd>
</dl>

**Examples**:
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
This command lists all endurance volumes on current account that are located at dal09, and sorts them by capacity.

### bluemix sl file volume-detail 
{: #sl_file_volume_detail} 

Display details for a specified volume.
```
bluemix sl file volume-detail VOLUME_ID
```


**Examples**:
```
bluemix sl file volume-detail 12345678
```
This command shows details of volume with ID 12345678.

### bluemix sl file volume-duplicate 
{: #sl_file_volume_duplicate} 

Order a file volume by duplicating an existing volume.
```
bluemix sl file volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>ID of an original volume snapshot to use for duplication.</dd>
<dt>-s, --duplicate-size</dt>
<dd>Size of duplicate file volume in GB, if no size is specified, the size of the original volume will be used.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>Performance Storage IOPS, between 100 and 6000 in multiples of 100, if no IOPS  is specified, the IOPS  of the original volume will be used.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Endurance Storage Tier, if no tier is specified, the tier of the original volume will be used.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>The size of snapshot space to order for the duplicate, if no snapshot space size is specified, the snapshot space size of the original volume will be used.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file volume-duplicate 12345678
```
This command shows order a new volume by duplicating the volume with ID 12345678.

### bluemix sl file volume-order 
{: #sl_file_volume_order} 

Order a file storage volume.
```
bluemix sl file volume-order [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-t, --storage-type</dt>
<dd>Required. Type of storage volume , options are: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>Required. Size of storage volume in GB .</dd>
<dt>-i, --iops</dt>
<dd>Performance Storage IOPs, between 100 and 6000 in multiples of 100 [required for storage-type performance].</dd>
<dt>-e, --tier</dt>
<dd>Endurance Storage Tier (IOP per GB) [required for storage-type endurance], options are: 0.25,2,4,10.</dd>
<dt>-d, --datacenter</dt>
<dd>Required. Datacenter short name .</dd>
<dt>-n, --snapshot-size</dt>
<dd>Optional parameter for ordering snapshot space along with the volume.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
This command orders a performance volume with size is 1000GB, IOPS is 4000, located at dal09.

### bluemix sl file volume-options 
{: #sl_file_volume_options} 

List all options for ordering a file storage.
```
bluemix sl file volume-options
```


**Examples**:
```
bluemix sl file volume-options
```
This command lists all options for creating a file storage volume, including storage type, volume size, IOPS, tier level, datacenter, and snapshot size.

### bluemix sl dns import 
{: #sl_dns_import} 

Import a zone based off a BIND zone file.
```
bluemix sl dns import ZONEFILE [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--dry-run</dt>
<dd>Don't actually create records.</dd>
</dl>

**Examples**:
```
bluemix sl dns import ~/blumix.net.txt
```
This command imports zone and its resource records from file: ~/blumix.net.txt.

### bluemix sl dns record-add 
{: #sl_dns_record_add} 

Add resource record in a zone.
```
bluemix sl dns record-add ZONE RECORD TYPE DATA [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--ttl</dt>
<dd>TTL(Time-To-Live)  in seconds, such as: 86400, default is: 7200.</dd>
</dl>

**Examples**:
```
bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
This command adds an A record to zone: bluemix.net, its host is "ftp", data is "127.0.0.1" and ttl is 86400 seconds.

### bluemix sl dns record-edit 
{: #sl_dns_record_edit} 

Update resource records in a zone.
```
bluemix sl dns record-edit ZONE [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--by-record</dt>
<dd>Edit by host record, such as www.</dd>
<dt>--by-id</dt>
<dd>Edit a single record by its ID.</dd>
<dt>--data</dt>
<dd>Record data, such as an IP address.</dd>
<dt>--ttl</dt>
<dd>TTL value in seconds, such as: 86400.</dd>
</dl>

**Examples**:
```
bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
This command edits records under zone: bluemix.net, whose ID is 12345678, and set its data to "127.0.0.2" and ttl to 3600.

### bluemix sl dns record-list 
{: #sl_dns_record_list} 

List all the resource records in a zone.
```
bluemix sl dns record-list ZONE [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--data</dt>
<dd>Filter by record data, such as an IP address.</dd>
<dt>--record</dt>
<dd>Filter by host record, such as www.</dd>
<dt>--ttl</dt>
<dd>Filter by TTL value in seconds, such as 86400.</dd>
<dt>--type</dt>
<dd>Filter by record type, such as A or CNAME.</dd>
</dl>

**Examples**:
```
bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
This command lists all A records under zone: bluemix.net,filtered by host is elasticsearch and ttl is 900 seconds.

### bluemix sl dns record-remove 
{: #sl_dns_record_remove} 

Remove resource record from a zone.
```
bluemix sl dns record-remove RECORD_ID
```


**Examples**:
```
bluemix sl dns record-remove 12345678
```
This command removes resource record with ID 12345678.

### bluemix sl dns zone-create 
{: #sl_dns_zone_create} 

Create a zone.
```
bluemix sl dns zone-create ZONE
```


**Examples**:
```
bluemix sl dns zone-create bluemix.net
```
This command creates a zone named bluemix.net.

### bluemix sl dns zone-delete 
{: #sl_dns_zone_delete} 

Delete a zone.
```
bluemix sl dns zone-delete ZONE
```


**Examples**:
```
bluemix sl dns zone-delete bluemix.net
```
This command deletes a zone named bluemix.net.

### bluemix sl dns zone-list 
{: #sl_dns_zone_list} 

List all zones on your account.
```
bluemix sl dns zone-list
```


**Examples**:
```
bluemix sl dns zone-list
```
This command lists all zones under current account.

### bluemix sl dns zone-print 
{: #sl_dns_zone_print} 

Print zone and resource records in BIND format.
```
bluemix sl dns zone-print ZONE
```


**Examples**:
```
bluemix sl dns zone-print bluemix.net
```
This command prints zone named bluemix.net in BIND format.

### bluemix sl globalip create 
{: #sl_globalip_create} 

Create a global IP.
```
bluemix sl globalip create [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--v6</dt>
<dd>Order a IPv6 IP address.</dd>
<dt>--test</dt>
<dd>Test order.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl globalip create --v6
```
This command creates an IP V6 address.

### bluemix sl globalip assign 
{: #sl_globalip_assign} 

Assign a global IP to a target router or device.
```
bluemix sl globalip assign IDENTIFIER TARGET
```


**Examples**:
```
bluemix sl globalip assign 12345678 9.111.123.456
```
This command assigns IP address with ID 12345678 to a target device whose IP address is 9.111.123.456.

### bluemix sl globalip cancel 
{: #sl_globalip_cancel} 

Cancel a global IP.
```
bluemix sl globalip cancel IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl globalip cancel 12345678
```
This command cancels IP address with ID 12345678.

### bluemix sl globalip list 
{: #sl_globalip_list} 

List all global IPs on your account.
```
bluemix sl globalip list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--v4</dt>
<dd>Display IPv4 IPs only.</dd>
<dt>--v6</dt>
<dd>Display IPv6 IPs only.</dd>
<dt>--order</dt>
<dd>Filter by the ID of order that purchased this IP address.</dd>
</dl>

**Examples**:
```
bluemix sl globalip list --v4
```
This command lists all IP V4 addresses on current account.

### bluemix sl globalip unassign 
{: #sl_globalip_unassign} 

Unassign a global IP from a target router or device.
```
bluemix sl globalip unassign IDENTIFIER
```


**Examples**:
```
bluemix sl globalip unassign 12345678
```
This command unassigns IP address with ID 12345678 from target device.

### bluemix sl image delete 
{: #sl_image_delete} 

Delete an image.
```
bluemix sl image delete IDENTIFIER
```
**Examples**:
```
   bluemix sl image delete 12345678
```
This command deletes image with ID `12345678`.

### bluemix sl image detail 
{: #sl_image_detail} 

Get details for an image.
```
bluemix sl image detail IDENTIFIER
```
**Examples**:
```
 bluemix sl image detail 12345678
```
This command gets details for image with ID 12345678.

### bluemix sl image edit 
{: #sl_image_edit} 

Edit details of an image.
```
bluemix sl image edit IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--name</dt>
<dd>Name of the image.</dd>
<dt>--note</dt>
<dd>Additional note for the image.</dd>
<dt>--tag</dt>
<dd>Tags for the image.</dd>
</dl>

*Examples**:
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
This command edits image with ID `12345678` and set its name to `ubuntu16`, note to `testing`, and tag to `staging`.

### bluemix sl image list 
{: #sl_image_list} 

List all images on your account.
```
bluemix sl image list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--name</dt>
<dd>Filter on image name.</dd>
<dt>--public</dt>
<dd>Display only public images.</dd>
<dt>--private</dt>
<dd>Display only private images.</dd>
</dl>

### bluemix sl ipsec cancel 
{: #sl_ipsec_cancel} 

Cancel a IPSec VPN tunnel context.
```
bluemix sl ipsec cancel CONTEXT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--immediate</dt>
<dd>Cancel the IPSec immediately instead of on the billing anniversary.</dd>
<dt>--reason</dt>
<dd>An optional reason for cancellation.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl ipsec config 
{: #sl_ipsec_config} 

Request configuration of a tunnel context.
```
bluemix sl ipsec config CONTEXT_ID [OPTIONS]
```

### bluemix sl ipsec detail 
{: #sl_ipsec_detail} 

List IPSec VPN tunnel context details.
```
bluemix sl ipsec detail CONTEXT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-i, --include</dt>
<dd>Include additional resources, options are: at,is,rs,sr,ss.</dd>
</dl>
### bluemix sl ipsec list 
{: #sl_ipsec_list} 

List IPSec VPN tunnel contexts.
```
bluemix sl ipsec list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--order</dt>
<dd>Filter by ID of the order that purchased the IPSEC.</dd>
</dl>
### bluemix sl ipsec order 
{: #sl_ipsec_order} 

Order a IPSec VPN tunnel.
```
bluemix sl ipsec order [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Required. Short name of the datacenter for the IPSEC, eg. dal09 .</dd>
</dl>

### bluemix sl ipsec subnet-add 
{: #sl_ipsec_subnet_add} 

Add a subnet to an IPSec tunnel context.
```
bluemix sl ipsec subnet-add CONTEXT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --subnet-id</dt>
<dd>Subnet identifier to add, required.</dd>
<dt>-t, --subnet-type</dt>
<dd>Subnet type to add, required, options are: internal,remote,service.</dd>
<dt>-n, --network</dt>
<dd>Subnet network identifier to create.</dd>
</dl>

### bluemix sl ipsec subnet-remove 
{: #sl_ipsec_subnet_remove} 

Remove a subnet from an IPSEC tunnel context.
```
bluemix sl ipsec subnet-remove CONTEXT_ID SUBNET_ID SUBNET_TYPE [OPTIONS]
```

### bluemix sl ipsec translation-add 
{: #sl_ipsec_translation_add} 

Add an address translation to an IPSec tunnel.
```
bluemix sl ipsec translation-add CONTEXT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Static IP address,required.</dd>
<dt>-r, --remote-ip</dt>
<dd>Remote IP address,required.</dd>
<dt>-n, --note</dt>
<dd>Note.</dd>
</dl>
### bluemix sl ipsec translation-remove 
{: #sl_ipsec_translation_remove} 

Remove a translation entry from an IPSec.
```
bluemix sl ipsec translation-remove CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

### bluemix sl ipsec translation-update 
{: #sl_ipsec_translation_update} 

Update an address translation for an IPSec.
```
bluemix sl ipsec translation-update CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-s, --static-ip</dt>
<dd>Static IP address,required.</dd>
<dt>-r, --remote-ip</dt>
<dd>Remote IP address,required.</dd>
<dt>-n, --note</dt>
<dd>Note.</dd>
</dl>
### bluemix sl ipsec update 
{: #sl_ipsec_update} 

Update tunnel context properties.
```
bluemix sl ipsec update CONTEXT_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Friendly name.</dd>
<dt>-r, --remote-peer</dt>
<dd>Remote peer IP address.</dd>
<dt>-k, --preshared-key</dt>
<dd>Preshared key.</dd>
<dt>-a, --phase1-auth</dt>
<dd>Phase 1 authentication,options are: MD5,SHA1,SHA256.</dd>
<dt>-c, --phase1-crypto</dt>
<dd>Phase 1 encryption,options are: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-d, --phase1-dh</dt>
<dd>Phase 1 diffie hellman group,options are: 0,1,2,5.</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>Phase 1 key life,range is 120-172800.</dd>
<dt>-u, --phase2-auth</dt>
<dd>Phase 2 authentication,options are: MD5,SHA1,SHA256.</dd>
<dt>-y, --phase2-crypto</dt>
<dd>Phase 2 encryption,options are: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-e, --phase2-dh</dt>
<dd>Phase 2 diffie hellman group,options are: 0,1,2,5.</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>Phase 2 perfect forward secrecy,range is 0-1.</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>Phase 2 key life,range is 120-172800.</dd>
</dl>

### bluemix sl loadbal cancel 
{: #sl_loadbal_cancel} 

Cancel an existing load balancer.
```
bluemix sl loadbal cancel LOADBAL_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl loadbal create 
{: #sl_loadbal_create} 

Adds a load balancer given the id returned from create-options.
```
bluemix sl loadbal create PRICE_ID LOCATION [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl loadbal create-options 
{: #sl_loadbal_create_options} 

Get price options to create a load balancer with.
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail 
{: #sl_loadbal_detail} 

Get Load balancer details.
```
bluemix sl loadbal detail LOADBAL_ID
```

### bluemix sl loadbal group-add 
{: #sl_loadbal_group_add} 

Adds a new load_balancer service.
```
bluemix sl loadbal group-add LOADBAL_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Required. The allocated percent of connections .</dd>
<dt>-p, --port</dt>
<dd>Required. The port number .</dd>
<dt>-t, --routing-type</dt>
<dd>Required. The ID of routing type . Run 'bluemix sl loadbal routing-types' to find an ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Required. The ID of routing method . Run 'bluemix sl loadbal routing-methods' to find an ID.</dd>
</dl>

### bluemix sl loadbal group-delete 
{: #sl_loadbal_group_delete} 

Deletes an existing load balancer service group.
```
bluemix sl loadbal group-delete GROUP_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl loadbal group-edit 
{: #sl_loadbal_group_edit} 

Edit an existing load balancer service group.
```
bluemix sl loadbal group-edit LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-a, --allocation</dt>
<dd>Change the allocated percent of connections.</dd>
<dt>-p, --port</dt>
<dd>Change the port number.</dd>
<dt>-t, --routing-type</dt>
<dd>Change the ID of routing type. Run 'bluemix sl loadbal routing-types' to find an ID.</dd>
<dt>-m, --routing-method</dt>
<dd>Change the ID of routing method. Run 'bluemix sl loadbal routing-methods' to find an ID.</dd>
</dl>

### bluemix sl loadbal group-reset 
{: #sl_loadbal_group_reset} 

Reset connections on a certain service group.
```
bluemix sl loadbal group-reset LOADBAL_ID GROUP_ID
```

### bluemix sl loadbal health-checks 
{: #sl_loadbal_health_checks} 

List health check types.
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list 
{: #sl_loadbal_list} 

List active load balancers.
```
bluemix sl loadbal list
```

<strong>Command options</strong>:
<dl>
<dt>-d, --datacenter</dt>
<dd>Filter by datacenter shortname.</dd>
<dt>-o, --order</dt>
<dd>Filter by ID of the order that purchased the load balancer.</dd>
<dt>-p, --ip-address</dt>
<dd>Filter by IP address.</dd>
</dl>
### bluemix sl loadbal routing-methods 
{: #sl_loadbal_routing_methods} 

List routing methods.
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types 
{: #sl_loadbal_routing_types} 

List routing types.
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add 
{: #sl_loadbal_service_add} 

Adds a new load balancer service.
```
bluemix sl loadbal service-add LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--disabled</dt>
<dd>Optional. Create the service as disabled,default is enabled if not specified .</dd>
<dt>-p, --port</dt>
<dd>Required. The port number for the service .</dd>
<dt>-w, --weight</dt>
<dd>Required. The weight of the service .</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Required. The health check type .</dd>
<dt>-i, --ip-address</dt>
<dd>Required. The IP address of the service .</dd>
</dl>

### bluemix sl loadbal service-delete 
{: #sl_loadbal_service_delete} 

Deletes an existing load balancer service.
```
bluemix sl loadbal service-delete SERVICE_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl loadbal service-edit 
{: #sl_loadbal_service_edit} 

Edit the properties of a service group.
```
bluemix sl loadbal service-edit LOADBAL_ID SERVICE_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--disabled</dt>
<dd>Disable the service.</dd>
<dt>--enabled</dt>
<dd>Enable the service.</dd>
<dt>-p, --port</dt>
<dd>Change the port number for the service.</dd>
<dt>-w, --weight</dt>
<dd>Change the weight of the service.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>Change the health check type.</dd>
<dt>-i, --ip-address</dt>
<dd>Change the IP address of the service.</dd>
</dl>

### bluemix sl loadbal service-toggle 
{: #sl_loadbal_service_toggle} 

Toggle the status of an existing load balancer service.
```
bluemix sl loadbal service-toggle SERVICE_ID
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

### bluemix sl security sshkey-add 
{: #sl_security_sshkey_add} 

Add a new SSH key.
```
bluemix sl security sshkey-add LABEL [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --in-file</dt>
<dd>The id_rsa.pub file to import for this key.</dd>
<dt>-k, --key</dt>
<dd>The actual SSH key.</dd>
<dt>--note</dt>
<dd>Extra note that will be associated with key.</dd>
</dl>

**Examples**:
```
bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
This command adds a SSH key from file: ~/.ssh/id_rsa.pub with a note "mykey".

### bluemix sl security sshkey-edit 
{: #sl_security_sshkey_edit} 

Edit an SSH key.
```
bluemix sl security sshkey-edit IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--label</dt>
<dd>The new label for the key.</dd>
<dt>--note</dt>
<dd>New notes for the key.</dd>
</dl>

**Examples**:
```
bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
This command updates the SSH key with ID 12345678 and sets label to "Bluemix" and note to "testing".

### bluemix sl security sshkey-list 
{: #sl_security_sshkey_list} 

List SSH keys on your account.
```
bluemix sl security sshkey-list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,label,fingerprint,notes.</dd>
</dl>

**Examples**:
```
bluemix sl security sshkey-list --sortby label
```
This command lists all SSH keys on current account and sorts them by label.

### bluemix sl security sshkey-print 
{: #sl_security_sshkey_print} 

Prints out an SSH key to the screen.
```
bluemix sl security sshkey-print IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --out-file</dt>
<dd>The public SSH key will be written to this file.</dd>
</dl>

**Examples**:
```
bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
This command shows the ID, label and notes of SSH key with ID 12345678 and write the public key to file: ~/mykey.pub.

### bluemix sl security sshkey-remove 
{: #sl_security_sshkey_remove} 

Permanently removes an SSH key.
```
bluemix sl security sshkey-remove IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl security sshkey-remove 12345678 -f
```
This command removes the SSH key with ID 12345678 without asking for confirmation.

### bluemix sl security cert-add 
{: #sl_security_cert_add} 

Add and upload SSL certificate details.
```
bluemix sl security cert-add [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--crt</dt>
<dd>Certificate file.</dd>
<dt>--csr</dt>
<dd>Certificate Signing Request file.</dd>
<dt>--icc</dt>
<dd>Intermediate Certificate file.</dd>
<dt>--key</dt>
<dd>Private Key file.</dd>
<dt>--notes</dt>
<dd>Additional notes.</dd>
</dl>

**Examples**:
```
bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key
```
This command adds certificate file: ~/bluemix.net.cert and private key file ~/bluemix.net.key for domain bluemix.net.

### bluemix sl security cert-edit 
{: #sl_security_cert_edit} 

Edit SSL certificate.
```
bluemix sl security cert-edit IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--crt</dt>
<dd>Certificate file.</dd>
<dt>--csr</dt>
<dd>Certificate Signing Request file.</dd>
<dt>--icc</dt>
<dd>Intermediate Certificate file.</dd>
<dt>--key</dt>
<dd>Private Key file.</dd>
<dt>--notes</dt>
<dd>Additional notes.</dd>
</dl>

**Examples**:
```
bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
This command edits certificate with ID 12345678 and updates its private key with file: ~/bluemix.net.key.

### bluemix sl security cert-download 
{: #sl_security_cert_download} 

Download SSL certificate and key files.
```
bluemix sl security cert-download IDENTIFIER
```


**Examples**:
```
bluemix sl security cert-download 12345678
```
This command downloads 4 files to current directory for certificate with ID 12345678. The 4 files are: certificate file, certificate signing request file, intermediate certificate file and private key file.

### bluemix sl security cert-list 
{: #sl_security_cert_list} 

List SSL certificates on your account.
```
bluemix sl security cert-list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--status</dt>
<dd>Show certificates with this status, default is: all, options are: all,valid,expired.</dd>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,common_name,days_until_expire,notes.</dd>
</dl>

**Examples**:
```
bluemix sl security cert-list --status valid --sortby days_until_expire
```
This command lists all valid certificates on current account and sort them by validity days.

### bluemix sl security cert-remove 
{: #sl_security_cert_remove} 

Remove SSL certificate.
```
bluemix sl security cert-remove IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl security cert-remove 12345678
```
This command removes certificate with ID 12345678.

### bluemix sl subnet cancel 
{: #sl_subnet_cancel} 

Cancel a subnet.
```
bluemix sl subnet cancel IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl subnet cancel 12345678 -f
```
This command cancels subnet with ID 12345678 without asking for confirmation.

### bluemix sl subnet create 
{: #sl_subnet_create} 

Add a new subnet to your account.
```
bluemix sl subnet create NETWORK QUANTITY VLAN_ID [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--v6, --ipv6</dt>
<dd>Order IPv6 Addresses.</dd>
<dt>--test</dt>
<dd>Do not order the subnet; just get a quote.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl subnet create public 16 567
```
This command creates a public subnet with 16 IP v4 addresses and places it on vlan with ID 567.

### bluemix sl subnet detail 
{: #sl_subnet_detail} 

Get details of a subnet.
```
bluemix sl subnet detail IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Hide virtual server listing.</dd>
<dt>--no-hardware</dt>
<dd>Hide hardware listing.</dd>
</dl>

**Examples**:
```
bluemix sl subnet detail 12345678
```
This command shows detailed information about subnet with ID 12345678, including virtual servers and hardware servers information.

### bluemix sl subnet list 
{: #sl_subnet_list} 

List all subnets on your account.
```
bluemix sl subnet list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by. Options are: id,identifier,type,network_space,datacenter,vlan_id,IPs,hardware,vs.</dd>
<dt>-d, --datacenter</dt>
<dd>Filter by datacenter shortname.</dd>
<dt>--identifier</dt>
<dd>Filter by network identifier.</dd>
<dt>-t, --subnet-type</dt>
<dd>Filter by subnet type.</dd>
<dt>--network-space</dt>
<dd>Filter by network space.</dd>
<dt>--v4, --ipv4</dt>
<dd>Display only IPv4 subnets.</dd>
<dt>--v6, --ipv6</dt>
<dd>Display only IPv6 subnets.</dd>
<dt>--order</dt>
<dd>Filter by the ID of order that purchased the subnets.</dd>
</dl>

**Examples**:
```
bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
This command lists IP V4 subnets on current account filtering by datacenter is dal09, subnet type is PRIMARY, and network space is PUBLIC.

### bluemix sl subnet lookup 
{: #sl_subnet_lookup} 

Find an IP address and display its subnet and device information.
```
bluemix sl subnet lookup IP_ADDRESS
```


**Examples**:
```
bluemix sl subnet lookup 9.125.235.255
```
This command finds the IP address record with address 9.125.235.255 and display its subnet and device information.

### bluemix sl vlan create 
{: #sl_vlan_create} 

Create a new VLAN.
```
bluemix sl vlan create [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-t, --vlan-type</dt>
<dd>The type of the VLAN, either public or private.</dd>
<dt>-r, --router</dt>
<dd>The hostname of the router.</dd>
<dt>-d, --datacenter</dt>
<dd>The short name of the datacenter.</dd>
<dt>-s, --size</dt>
<dd>The size of the subnets, options are: 8 (5 usable IPs) or 16 (13 usable IPs) or 32 (29 usable IPs).</dd>
<dt>-n, --name</dt>
<dd>The name of the VLAN.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
This command creates a public vlan located at datacenter dal09 with 16 IP addresses and name is myvlan.

### bluemix sl vlan cancel 
{: #sl_vlan_cancel} 

Cancel a VLAN.
```
bluemix sl vlan cancel IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vlan cancel 12345678 -f
```
This command cancels vlan with ID 12345678 without asking for confirmation.

### bluemix sl vlan detail 
{: #sl_vlan_detail} 

Get details about a VLAN.
```
bluemix sl vlan detail IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--no-vs</dt>
<dd>Hide virtual server listing.</dd>
<dt>--no-hardware</dt>
<dd>Hide hardware listing.</dd>
</dl>

**Examples**:
```
bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
This command shows details of vlan with ID 12345678, and not list virtual server or hardware server.

### bluemix sl vlan edit 
{: #sl_vlan_edit} 

Edit the details about a VLAN.
```
bluemix sl vlan edit IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-n, --name</dt>
<dd>The name of the VLAN.</dd>
</dl>

**Examples**:
```
bluemix sl vlan edit 12345678 -n myvlan-rename
```
This command updates vlan with ID 12345678 and gives it a new name "myvlan-rename".

### bluemix sl vlan list 
{: #sl_vlan_list} 

List all the VLANs on your account.
```
bluemix sl vlan list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,number,name,firewall,datacenter,hardware,virtual_servers,public_ips.</dd>
<dt>-d, --datacenter</dt>
<dd>Filter by datacenter shortname.</dd>
<dt>-n, --number</dt>
<dd>Filter by VLAN number.</dd>
<dt>--name</dt>
<dd>Filter by VLAN name.</dd>
<dt>--order</dt>
<dd>Filter by ID of the order that purchased the VLAN.</dd>
</dl>

**Examples**:
```
bluemix sl vlan list -d dal09 --sortby number
```
This commands lists all vlans on current account filtering by datacenter equals to dal09, and sort them by vlan number.

### bluemix sl vlan options 
{: #sl_vlan_options} 

List all the options for creating VLAN.
```
bluemix sl vlan options
```


**Examples**:
```
bluemix sl vlan options
```
This command lists all options for creating a vlan, eg. vlan type, datacenters, subnet size, routers, etc.

### bluemix sl vs cancel 
{: #sl_vs_cancel} 

Cancel virtual server instance.
```
bluemix sl vs cancel IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs cancel 12345678
```
This command cancels virtual server instance with ID of 12345678.

### bluemix sl vs capture 
{: #sl_vs_capture} 

Capture virtual server instance into an image.
```
bluemix sl vs capture IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-n, --name</dt>
<dd>Required. Name of the image .</dd>
<dt>--all</dt>
<dd>Capture all disks belonging to the VS.</dd>
<dt>--note</dt>
<dd>Add a note to be associated with the image.</dd>
</dl>

**Examples**:
```
bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
This command captures virtual server instance with ID of 12345678 with all disks into an image named "mybluemix" with note "testing".

### bluemix sl vs create 
{: #sl_vs_create} 

Create virtual server instance.
```
bluemix sl vs create [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-H, --hostname</dt>
<dd>Required. Host portion of the FQDN .</dd>
<dt>-D, --domain</dt>
<dd>Required. Domain portion of the FQDN .</dd>
<dt>-c, --cpu</dt>
<dd>Required. Number of CPU cores .</dd>
<dt>-m, --memory</dt>
<dd>Required. Memory in megabytes .</dd>
<dt>-d, --datacenter</dt>
<dd>Required. Datacenter shortname .</dd>
<dt>-o, --os</dt>
<dd>OS install code. Tip: you can specify <OS>_LATEST.</dd>
<dt>--image</dt>
<dd>Image ID. See: 'bluemix sl image list' for reference.</dd>
<dt>--billing</dt>
<dd>Billing rate. Default is: hourly. Options are: hourly, monthly.</dd>
<dt>--dedicated</dt>
<dd>Create a dedicated Virtual Server (Private Node).</dd>
<dt>--san</dt>
<dd>Use SAN storage instead of local disk.</dd>
<dt>--test</dt>
<dd>Do not actually create the virtual server.</dd>
<dt>--export</dt>
<dd>Exports options to a template file.</dd>
<dt>-i, --postinstall</dt>
<dd>Post-install script to download.</dd>
<dt>-k, --key</dt>
<dd>The IDs of the SSH keys to add to the root user (multiple occurrence permitted).</dd>
<dt>--disk</dt>
<dd>Disk sizes (multiple occurrence permitted).</dd>
<dt>--private</dt>
<dd>Forces the virtual server to only have access the private network.</dd>
<dt>--like</dt>
<dd>Use the configuration from an existing virtual server.</dd>
<dt>-n, --network</dt>
<dd>Network port speed in Mbps.</dd>
<dt>--tag</dt>
<dd>Tags to add to the instance (multiple occurrence permitted).</dd>
<dt>-t, --template</dt>
<dd>A template file that defaults the command-line options.</dd>
<dt>-u, --userdata</dt>
<dd>User defined metadata string.</dd>
<dt>-F, --userfile</dt>
<dd>Read userdata from file.</dd>
<dt>--vlan-public</dt>
<dd>The ID of the public VLAN on which you want the virtual server placed.</dd>
<dt>--vlan-private</dt>
<dd>The ID of the private VLAN on which you want the virtual server placed.</dd>
<dt>--wait</dt>
<dd>Wait until the virtual server is finished provisioning for up to X seconds before returning.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
This command orders a virtual server instance with hostname is myvsi, domain is bluemix.net, 4 cpu cores, 4096M memory, located at datacenter: dal10,

### bluemix sl vs options 
{: #sl_vs_options} 

List options for creating virtual server instance.
```
bluemix sl vs options [OPTIONS]
```


**Examples**:
```
bluemix sl vs options
```
This command lists all the options for creating a virtual server instance, eg.datacenters, cpu, memory, os, disk, network speed, etc.

### bluemix sl vs credentials 
{: #sl_vs_credentials} 

List virtual server instance credentials.
```
bluemix sl vs credentials IDENTIFIER [OPTIONS]
```


**Examples**:
```
bluemix sl vs credentials 12345678
```
This command lists all username and password pairs of virtual server instance with ID 12345678.

### bluemix sl vs detail 
{: #sl_vs_detail} 

Get details for a virtual server instance.
```
bluemix sl vs detail IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--passwords</dt>
<dd>Show passwords (check over your shoulder!).</dd>
<dt>--price</dt>
<dd>Show associated prices.</dd>
</dl>

**Examples**:
```
bluemix sl vs details 12345678
```
This command lists detailed information about virtual server instance with ID 12345678.

### bluemix sl vs dns-sync 
{: #sl_vs_dns_sync} 

Synchronize DNS records for a virtual server instance.
```
bluemix sl vs dns-sync IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-a, --a-record</dt>
<dd>Sync the A record for the host.</dd>
<dt>--aaaa-record</dt>
<dd>Sync the AAAA record for the host.</dd>
<dt>--ptr</dt>
<dd>Sync the PTR record for the host.</dd>
<dt>--ttl</dt>
<dd>Sets the TTL for the A and/or PTR records, default is: 7200.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
This command synchronizes A record(IP V4 address) of virtual server instance with ID 12345678 to DNS server and sets ttl of this A record to 3600.

### bluemix sl vs edit 
{: #sl_vs_edit} 

Edit a virtual server instance's details.
```
bluemix sl vs edit IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-D, --domain</dt>
<dd>Domain portion of the FQDN.</dd>
<dt>-H, --hostname</dt>
<dd>Host portion of the FQDN. example: server.</dd>
<dt>--tag</dt>
<dd>Tags to set or empty string to remove all.</dd>
<dt>-u, --userdata</dt>
<dd>User defined metadata string.</dd>
<dt>-F, --userfile</dt>
<dd>Read userdata from file.</dd>
<dt>--public-speed</dt>
<dd>Public port speed, options are: 0,10,100,1000,10000.</dd>
<dt>--private-speed</dt>
<dd>Private port speed, options are: 0,10,100,1000,10000.</dd>
</dl>

**Examples**:
```
bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
This command updates virtual server instance with ID 12345678 and set its domain to be "bluemix.net", hostname to "myapp", tag to "testcli",

### bluemix sl vs list 
{: #sl_vs_list} 

List virtual server instances on your account.
```
bluemix sl vs list [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Number of CPU cores.</dd>
<dt>-D, --domain</dt>
<dd>Domain portion of the FQDN.</dd>
<dt>-d, --datacenter</dt>
<dd>Datacenter shortname.</dd>
<dt>-H, --hostname</dt>
<dd>Host portion of the FQDN.</dd>
<dt>-m, --memory</dt>
<dd>Memory in megabytes.</dd>
<dt>-n, --network</dt>
<dd>Network port speed in Mbps.</dd>
<dt>--hourly</dt>
<dd>Show only hourly instances.</dd>
<dt>--monthly</dt>
<dd>Show only monthly instances.</dd>
<dt>--tag</dt>
<dd>Filter by tags (multiple occurrence permitted).</dd>
<dt>--sortby</dt>
<dd>Column to sort by, options are: id,hostname,domain,datacenter,cpu,memory,primary_ip,backend_ip. Default is: hostname.</dd>
<dt>--columns</dt>
<dd>Columns to display, options are: guid,primary_ip,backend_ip,datacenter,action,power_state,created_by,tags. Default is: id,hostname,primary_ip,backend_ip,datacenter,action.</dd>
</dl>

**Examples**:
```
bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
This command lists all hourly-billing virtual server instances on current account filtering domain equals to "bluemix.net" and sort them by memory.

### bluemix sl vs pause 
{: #sl_vs_pause} 

Pause an active virtual server instance.
```
bluemix sl vs pause IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs pause 12345678 -f
```
This command pauses virtual server instance with ID 12345678 without asking for confirmation.

### bluemix sl vs power-off 
{: #sl_vs_power_off} 

Power off an active virtual server instance.
```
bluemix sl vs power-off IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--hard</dt>
<dd>Perform a hard shutdown.</dd>
<dt>--soft</dt>
<dd>Perform a soft shutdown.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs power-off 12345678 --soft
```
This command performs a soft power off for virtual server instance with ID 12345678.

### bluemix sl vs power-on 
{: #sl_vs_power_on} 

Power on a virtual server instance.
```
bluemix sl vs power-on IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs power-on 12345678
```
This command performs a power on for virtual server instance with ID 12345678.

### bluemix sl vs ready 
{: #sl_vs_ready} 

Check if a virtual server instance is ready for use.
```
bluemix sl vs ready IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--wait</dt>
<dd>Wait until the virtual server is finished provisioning for up to X seconds before returning.</dd>
</dl>

**Examples**:
```
bluemix sl vs ready 12345678 --wait 30
```
This command checks virtual server instance with ID 12345678 status to see if it is ready for use continuously and waits up to 30 seconds.

### bluemix sl vs reboot 
{: #sl_vs_reboot} 

Reboot an active virtual server instance.
```
bluemix sl vs reboot IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>--hard</dt>
<dd>Perform a hard reboot.</dd>
<dt>--soft</dt>
<dd>Perform a hard reboot.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs reboot 12345678 --hard
```
This command performs a hard reboot for virtual server instance with ID 12345678.

### bluemix sl vs reload 
{: #sl_vs_reload} 

Reload operating system on a virtual server instance.
```
bluemix sl vs reload IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-i, --postinstall</dt>
<dd>Post-install script to download.</dd>
<dt>--image</dt>
<dd>Image ID. The default is to use the current operating system.</dd>
<dt>See:</dt>
<dd>'bluemix sl image list' for reference.</dd>
<dt>-k, --key</dt>
<dd>The IDs of the SSH keys to add to the root user (multiple occurrence permitted).</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs reload 12345678
```
This command reloads current operating system for virtual server instance with ID 12345678.

### bluemix sl vs rescue 
{: #sl_vs_rescue} 

Reboot a virtual server instance into a rescue image.
```
bluemix sl vs rescue IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs rescue 12345678
```
This command reboots virtual server instance with ID 12345678 into a rescue image.

### bluemix sl vs resume 
{: #sl_vs_resume} 

Resume a paused virtual server instance.
```
bluemix sl vs resume IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs resume 12345678
```
This command resumes virtual server instance with ID 12345678.

### bluemix sl vs upgrade 
{: #sl_vs_upgrade} 

Upgrade a virtual server instance.
```
bluemix sl vs upgrade IDENTIFIER [OPTIONS]
```

<strong>Command options</strong>:
<dl>
<dt>-c, --cpu</dt>
<dd>Number of CPU cores.</dd>
<dt>--private</dt>
<dd>CPU core will be on a dedicated host server.</dd>
<dt>-m, --memory</dt>
<dd>Memory in megabytes.</dd>
<dt>--network</dt>
<dd>Network port speed in Mbps.</dd>
<dt>-f, --force</dt>
<dd>Force operation without confirmation.</dd>
</dl>

**Examples**:
```
bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
This commands upgrades virtual server instance with ID 12345678 and set number of CPU cores to 8, memory to 8192M, network port speed to 1000 Mbps.

