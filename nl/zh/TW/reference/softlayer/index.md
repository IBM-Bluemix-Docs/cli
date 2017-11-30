---

copyright:

  years: 2016,2017

lastupdated: "2017-09-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) 指令
{: #softlayer_cli}

{{site.data.keyword.BluSoftlayer}} 外掛程式已合併至 {{site.data.keyword.Bluemix_notm}} CLI。您不再需要安裝外掛程式。

在 {{site.data.keyword.Bluemix_notm}} 指令行介面 (CLI) 中使用 {{site.data.keyword.BluSoftlayer_notm}} 指令，以配置及管理 SoftLayer 服務。


若要開始使用，請安裝 IBM {{site.data.keyword.Bluemix_notm}} CLI。如需詳細資料，請參閱 [Bluemix CLI ![外部鏈結圖示](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window}。

如需完整 {{site.data.keyword.Bluemix_notm}} 指令清單，請參閱：[{{site.data.keyword.Bluemix_notm:}} (bx) 指令](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)


## 一般 {{site.data.keyword.BluSoftlayer_notm}} 指令

支援下列指令。使用 `bluemix sl` 指令，以查看可用的指令清單：

<table summary="按字母順序排序的一般指令，其鏈結提供指令的相關資訊">
<caption>表 1. 一般 Softlayer 指令</caption>
 <thead>
 <th colspan="6">一般 Softlayer 指令</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## {{site.data.keyword.BluSoftlayer_notm}} Block Storage 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 2. Softlayer Block Storage</caption>
 <thead>
 <th colspan="6">Softlayer Block Storage</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} CDN 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 3. Softlayer CDN</caption>
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

## {{site.data.keyword.BluSoftlayer_notm}} File Stoarge 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 4. Softlayer File Storage</caption>
 <thead>
 <th colspan="6">Softlayer File Storage</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} DNS 指令

<table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 5. Softlayer DNS 指令</caption>
 <thead>
 <th colspan="6">Softlayer DNS 指令</th>
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

<table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 6. Softlayer 廣域 IP 指令</caption>
 <thead>
 <th colspan="6">Softlayer 廣域 IP 指令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} image 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 7. Softlayer image 指令</caption>
 <thead>
 <th colspan="6">Softlayer image 指令</th>
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
 
 ## {{site.data.keyword.BluSoftlayer_notm}} IPSec VPN 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 7. Softlayer IPSec VPN 指令</caption>
 <thead>
 <th colspan="6">Softlayer IPSec VPN 指令</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} 負載平衡器指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 8. Softlayer 負載平衡器指令</caption>
 <thead>
 <th colspan="6">Softlayer 負載平衡器指令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} security 指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 9. Softlayer security 指令</caption>
 <thead>
 <th colspan="5">Softlayer security 指令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} subnet 指令
 
 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 10. Softlayer subnet 指令</caption>
 <thead>
 <th colspan="5">Softlayer subnet 指令</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} 虛擬伺服器指令

 <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 11. Softlayer 虛擬伺服器指令</caption>
 <thead>
 <th colspan="6">Softlayer 虛擬伺服器指令</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} VLAN 指令

  <table summary="按字母順序排序的一般 Softlayer 指令，其鏈結提供指令的相關資訊">
<caption>表 12. Softlayer VLAN 指令</caption>
 <thead>
 <th colspan="6">Softlayer VLAN 指令</th>
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

### 指令用法
若要檢視指令的說明資訊，請執行：`bluemix sl [command] -h`。

### bluemix sl init
{: #sl_init}

起始設定用來連接至 SoftLayer 環境的配置設定。配置包括使用者名稱、API 金鑰或密碼、帳戶及端點。
```
bluemix sl init [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-a, --api-endpoint</dt>
<dd>Softlayer API 端點 URL，預設值為：https://api.softlayer.com/rest/v3.1（適用於 Softlayer API 金鑰鑑別）、https://api.softlayer.com/mobile/v3.1（適用於 IBM ID 鑑別）。</dd>
<dt>-u, --sl-user</dt>
<dd>Softlayer 使用者名稱。</dd>
<dt>-p, --sl-password</dt>
<dd>Softlayer 密碼或 API 金鑰。</dd>
<dt>-c, --account-id</dt>
<dd>Softlayer 帳戶 ID。</dd>
<dt>-q, --security-question-id</dt>
<dd>用來鑑別的安全問題 ID，如果您不知道，請詢問帳戶擁有者。</dd>
<dt>-w, --security-question-answer</dt>
<dd>用來鑑別的安全問題回答，如果您不知道，請詢問帳戶擁有者。</dd>
<dt>-s, --security-code</dt>
<dd>啟用雙因子鑑別時，安全供應商所產生的安全程式碼。</dd>
<dt>-v, --security-vendor</dt>
<dd>提供安全程式碼以進行鑑別的安全供應商，選項包含：VERISIGN、TOTP、PHONE_FACTOR。</dd>
<dt>-t, --auth-token</dt>
<dd>啟用電話鑑別時的鑑別記號。</dd>
</dl>

例如，使用 Softlayer 使用者名稱及密碼/API 金鑰登入
```
$ bluemix sl config
Choose how to configure Softlayer authentication: 
1. Login with Softlayer user name and password/API key
2. Use Bluemix Single-Sign-On
Enter a number>1
Softlayer API endpoint URL: [https://api.softlayer.com/rest/v3.1]>
Username: []> wangjunl@cn.ibm.com
API key or password: []> abcd

Softlayer API endpoint:    https://api.softlayer.com/rest/v3.1   
Account ID:                278444   
User ID:                   wangjunl@cn.ibm.com   
API Key:                   xxxxxxxxxx
```
例如，使用 Bluemix Single-Sign-On 登入 Softlayer
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
```
提示：使用 'bx cf <command>'，以搭配 Bluemix CLI 環境定義執行 Cloud Foundry CLI 。
```

$ bx sl init
Choose how to configure Softlayer authentication: 
1. Login with Softlayer user name and password/API key
2. Use Bluemix Single-Sign-On
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

檢視運作 Softlayer 環境的所有指令說明資訊。
```
bluemix sl help

```

### bluemix sl block access-authorize 
{: #sl_block_access_authorize} 

授權主機存取給定的磁區。
```
bluemix sl block access-authorize VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --hardware-id</dt>
<dd>要授權的某部硬體伺服器的 ID。</dd>
<dt>-v, --virtual-id</dt>
<dd>要授權的某部虛擬伺服器的 ID。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要授權的某個 IP 位址的 ID。</dd>
<dt>-p, --ip-address</dt>
<dd>要授權的 IP 位址。</dd>
</dl>

**範例**：
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
這個指令會授權 ID 為 87654321 的虛擬伺服器存取 ID 為 12345678 的磁區。

### bluemix sl block access-list 
{: #sl_block_access_list} 

列出 ACL。
```
bluemix sl block access-list VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、name、type、private_ip_address、host_iqn、username、password。</dd>
<dt>--columns</dt>
<dd>要顯示的直欄，選項包含：id、name、type、private_ip_address、host_iqn、username、password。</dd>
</dl>

**範例**：
```
bluemix sl block access-list 12345678 --sortby id
```
這個指令會列出獲授權存取 ID 為 12345678 的磁區的所有主機，並依 ID 排序。

### bluemix sl block access-revoke 
{: #sl_block_access_revoke} 

撤銷主機存取給定磁區的授權。
```
 bluemix sl block access-revoke VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --hardware-id</dt>
<dd>要撤銷的某部硬體伺服器的 ID。</dd>
<dt>-v, --virtual-id</dt>
<dd>要撤銷的某部虛擬伺服器的 ID。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要撤銷的某個 IP 位址的 ID。</dd>
<dt>-p, --ip-address</dt>
<dd>要撤銷的 IP 位址。</dd>
</dl>

**範例**：
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
這個指令會撤銷 ID 為 87654321 的虛擬伺服器對 ID 為 12345678 的磁區的存取權。

### bluemix sl block replica-failback 
{: #sl_block_replica_failback} 

從抄本進行區塊磁區失效回復。
```
 bluemix sl block replica-failback VOLUME_ID
```


**範例**：
```
 bluemix sl block replica-failback 12345678
```
這個指令會針對 ID 為 12345678 的磁區執行失效回復作業。

### bluemix sl block replica-failover 
{: #sl_block_replica_failover} 

將區塊磁區失效接手至給定的抄本磁區。
```
bluemix sl block replica-failover VOLUME_ID REPLICA_ID
```


**範例**：
```
 bluemix sl block replica-failover 12345678 87654321
```
這個指令會執行將 ID 為 12345678 的磁區失效接手至 ID 為 87654321 的抄本磁區的作業。

### bluemix sl block replica-locations 
{: #sl_block_replica_locations} 

列出給定磁區的適當抄寫資料中心。
```
bluemix sl block replica-locations VOLUME_ID
```


**範例**：
```
bluemix sl block replica-locations 12345678
```
這個指令會列出 ID 為 12345678 的區塊磁區的適當抄寫資料中心。

### bluemix sl block replica-order 
{: #sl_block_replica_order} 

訂購區塊儲存空間抄本磁區。
```
 bluemix sl block replica-order VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>必要。要用於抄寫的 Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
<dt>-d, --datacenter</dt>
<dd>必要。抄本資料中心的簡稱，例如：dal09。</dd>
<dt>-t, --tier</dt>
<dd>選用。已訂購抄本之主要磁區的耐久性儲存空間層級（每 GB 的 IOPS），選項包含：0.25、2、4、10，如果未指定層級，將會使用原始磁區的層級。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間，如果未指定 IOPS，將會使用原始磁區的 IOPS。</dd>
<dt>-o, --os-type</dt>
<dd>選用。已訂購抄本之主要磁區的作業系統類型（例如：LINUX），選項包含：HYPER_V、LINUX、VMWARE、WINDOWS_2008、WINDOWS_GPT、WINDOWS、XEN。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
這個指令會訂購 ID 為 12345678 的磁區的抄本，此抄本會執行 DAILY 抄寫、位於 dal09、層級層次為 4、OS 類型為 Linux。

### bluemix sl block replica-partners 
{: #sl_block_replica_partners} 

列出區塊磁區的現有抄本磁區。
```
bluemix sl block replica-partners VOLUME_ID [OPTIONS]
```


**範例**：
```
bluemix sl block replica-partners 12345678
```
這個指令會列出 ID 為 12345678 的區塊磁區的現有抄本磁區。

### bluemix sl block snapshot-cancel 
{: #sl_block_snapshot_cancel} 

取消給定磁區的現有 Snapshot 空間。
```
 bluemix sl block snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--reason</dt>
<dd>選用性的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消 Snapshot 空間，而不是在計費週年日取消。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl block snapshot-cancel 12345678 --immediate -f
```
這個指令會立即取消 ID 為 12345678 的 Snapshot，而不要求確認。

### bluemix sl block snapshot-create 
{: #sl_block_snapshot_create} 

在給定的磁區上建立 Snapshot。
```
 bluemix sl block snapshot-create VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-n, --note</dt>
<dd>要設定於新 Snapshot 的附註。</dd>
</dl>

**範例**：
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
這個指令會針對 ID 為 12345678 的磁區建立 Snapshot，並新增附註 snapshotforbluemix。

### bluemix sl block snapshot-disable 
{: #sl_block_snapshot_disable} 

依給定磁區的指定排程停用 Snapshot。
```
 bluemix sl block snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --schedule-type</dt>
<dd>必要。Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
</dl>

**範例**：
```
 bluemix sl block snapshot-disable 12345678 -s DAILY
```
這個指令會針對 ID 為 12345678 的磁區停用每日 Snapshot。

### bluemix sl block snapshot-enable 
{: #sl_block_snapshot_enable} 

依指定的排程為給定磁區啟用 Snapshot。
```
 bluemix sl block snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --schedule-type</dt>
<dd>必要。Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
<dt>-c, --retention-count</dt>
<dd>必要。要保留的 Snapshot 數目。</dd>
<dt>-m, --minute</dt>
<dd>應該在幾分擷取 Snapshot，選項為 0 到 59 之間的整數。</dd>
<dt>-r, --hour</dt>
<dd>應該在幾點擷取 Snapshot，選項為 0 到 23 之間的整數。</dd>
<dt>-d, --day-of-week</dt>
<dd>應該在星期幾擷取 Snapshot，選項為 0 到 6 之間的整數。0 表示星期日、1 表示星期一、2 表示星期二、3 表示星期三、4 表示星期四、5 表示星期五、6 表示星期六。</dd>
</dl>

**範例**：
```
 bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
這個指令會針對 ID 為 12345678 的磁區啟用 Snapshot、在每週的星期日 2:00 擷取 Snapshot，且最多保留 5 個 Snapshot。

### bluemix sl block snapshot-delete 
{: #sl_block_snapshot_delete} 

在給定的磁區上刪除 Snapshot。
```
  bluemix sl block snapshot-delete SNAPSHOT_ID
```


**範例**：
```
 bluemix sl block snapshot-delete 12345678
```
這個指令會刪除 ID 為 12345678 的 Snapshot。

### bluemix sl block snapshot-list 
{: #sl_block_snapshot_list} 

列出區塊儲存空間 Snapshot。
```
 bluemix sl block snapshot-list VOLUME_ID [OPTIONS]

```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、name、created、size_bytes。</dd>
</dl>

**範例**：
```
 bluemix sl block snapshot-list 12345678 --sortby id
```
這個指令會列出 ID 為 12345678 的磁區的所有 Snapshot，並依 ID 排序。

### bluemix sl block snapshot-order 
{: #sl_block_snapshot_order} 

訂購區塊儲存空間磁區的 Snapshot 空間。
```
 bluemix sl block snapshot-order VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --size</dt>
<dd>必要。要建立的 Snapshot 空間大小（以 GB 為單位）。</dd>
<dt>-t, --tier</dt>
<dd>選用。已訂購空間之區塊磁區的耐久性儲存空間層級（每 GB 的 IOPS），選項包含：0.25、2、4、10。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間。</dd>
<dt>-u, --upgrade</dt>
<dd>該旗標指出訂單為升級。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
   bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
這個指令會針對 ID 為 12345678 的磁區訂購 Snapshot 空間、大小為 1000GB、層級層次為每 GB 4 個 IOPS。

### bluemix sl block snapshot-restore 
{: #sl_block_snapshot_restore} 

使用給定的 Snapshot 還原區塊磁區。
```
 bluemix sl block snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**範例**：
```
 bluemix sl block snapshot-restore 12345678 87654321
```
這個指令會從 ID 為 87654321 的 Snapshot 還原 ID 為 12345678 的磁區。

### bluemix sl block volume-cancel 
{: #sl_block_volume_cancel} 

取消現有的區塊儲存空間磁區。
```
 bluemix sl block volume-cancel VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--reason</dt>
<dd>選用性的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消區塊儲存空間磁區，而不是在計費週年日取消。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl block volume-cancel 12345678 --immediate -f
```
這個指令會立即取消 ID 為 12345678 的磁區，而不要求確認。

### bluemix sl block volume-list 
{: #sl_block_volume_list} 

列出區塊儲存空間。
```
 bluemix sl block volume-list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-u, --username</dt>
<dd>依磁區使用者名稱過濾。</dd>
<dt>-d, --datacenter</dt>
<dd>依資料中心簡稱過濾。</dd>
<dt>-t, --storage-type</dt>
<dd>依儲存空間磁區的類型過濾，選項包含：performance、endurance。</dd>
<dt>-o, --order</dt>
<dd>依購買區塊儲存空間的訂單 ID 過濾。</dd>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、active_transactions、created_by。</dd>
<dt>--columns</dt>
<dd>要顯示的直欄，選項包含：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、created_by。</dd>
</dl>

**範例**：
```
 bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
這個指令會列出現行帳戶中位於 dal09 的所有耐久性磁區，並依容量排序。


### bluemix sl block volume-detail 
{: #sl_block_volume_detail} 

顯示指定磁區的詳細資料。
```
 bluemix sl block volume-detail VOLUME_ID
```


**範例**：
```
 bluemix sl block volume-detail 12345678
```
這個指令會顯示 ID 為 12345678 的磁區的詳細資料。

### bluemix sl block volume-duplicate 
{: #sl_block_volume_duplicate} 

複製現有磁區，以訂購區塊磁區。
```
bluemix sl block volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>要用於複製的原始磁區 Snapshot 的 ID。</dd>
<dt>-s, --duplicate-size</dt>
<dd>複製區塊磁區的大小（以 GB 為單位），如果未指定大小，將會使用原始磁區的大小。</dd>
<dt>-i, --duplicate-iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間，如果未指定 IOPS，將會使用原始磁區的 IOPS。</dd>
<dt>-t, --duplicate-tier</dt>
<dd>耐久性儲存空間層級，如果未指定層級，將會使用原始磁區的層級。</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>要針對複製項目訂購的 Snapshot 空間大小，如果未指定 Snapshot 空間大小，將會使用原始磁區的 Snapshot 空間大小。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl block volume-duplicate 12345678
```
這個指令會顯示如何複製 ID 為 12345678 的磁區來訂購新磁區。

### bluemix sl block volume-order 
{: #sl_block_volume_order} 

訂購區塊儲存空間磁區。
```
   bluemix sl block volume-order [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-t, --storage-type</dt>
<dd>必要。儲存空間磁區的類型，選項包含：performance、endurance。</dd>
<dt>-s, --size</dt>
<dd>必要。儲存空間磁區的大小（以 GB 為單位）。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間 [storage-type performance 的必要項目]。</dd>
<dt>-e, --tier</dt>
<dd>耐久性儲存空間層級（每 GB 的 IOP）[storage-type endurance 的必要項目]，選項包含：0.25、2、4、10。</dd>
<dt>-o, --os-type</dt>
<dd>必要。作業系統，選項包含：HYPER_V、LINUX、VMWARE、WINDOWS_2008、WINDOWS_GPT、WINDOWS、XEN。</dd>
<dt>-d, --datacenter</dt>
<dd>必要。資料中心簡稱。</dd>
<dt>-n, --snapshot-size</dt>
<dd>隨耐久性區塊儲存空間訂購 Snapshot 空間的選用參數；指定要訂購的 Snapshot 空間大小（以 GB 為單位）。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
這個指令會訂購效能磁區：大小為 1000GB、IOPS 為 4000、OS 類型為 LINUX、位於 dal09。

### bluemix sl block volume-options 
{: #sl_block_volume_options} 

列出用來訂購區塊儲存空間的所有選項。
```
 bluemix sl block volume-options
```


**範例**：
```
 bluemix sl block volume-options
```
這個指令會列出用來建立區塊儲存空間磁區的所有選項，包括儲存空間類型、磁區大小、OS 類型、IOPS、層級層次、資料中心和 Snapshot 大小。


### bluemix sl cdn cancel 
{: #sl_cdn_cancel} 

取消 CDN 帳戶。
```
bluemix sl cdn cancel ACCOUNT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>
### bluemix sl cdn detail 
{: #sl_cdn_detail} 

詳述 CDN 帳戶。
```
bluemix sl cdn detail ACCOUNT_ID
```

### bluemix sl cdn list 
{: #sl_cdn_list} 

列出所有 CDN 帳戶。
```
bluemix sl cdn list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、name、type、created。</dd>
<dt>--order</dt>
<dd>依訂單 ID 過濾。</dd>
</dl>
### bluemix sl cdn load 
{: #sl_cdn_load} 

在所有邊緣節點上快取一個以上的檔案。
```
bluemix sl cdn load ACCOUNT_ID CONTENT_URL [CONTENT_URL...]
```

### bluemix sl cdn order 
{: #sl_cdn_order} 

訂購 CDN 帳戶。
```
bluemix sl cdn order [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-b, --bandwidth</dt>
<dd>如果未指定，將會使用 CDN 頻寬「隨收隨付制」價格。</dd>
<dt>-s, --storage</dt>
<dd>如果未指定，將會使用 CDN 儲存空間「隨收隨付制」價格。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>
### bluemix sl cdn options 
{: #sl_cdn_options} 

訂購 CDN 帳戶的頻寬及儲存空間選項。
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add 
{: #sl_cdn_origin_add} 

建立原始取回對映。
```
bluemix sl cdn origin-add ACCOUNT_ID CONTENT_URL [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-t, --type</dt>
<dd>此對映的媒體類型（http、flash、wm 等），預設值為：http。</dd>
<dt>-c, --cname</dt>
<dd>要連接至對映的選用 CNAME。</dd>
</dl>
### bluemix sl cdn origin-list 
{: #sl_cdn_origin_list} 

列出原始取回對映。
```
bluemix sl cdn origin-list ACCOUNT_ID
```

### bluemix sl cdn origin-remove 
{: #sl_cdn_origin_remove} 

移除原始取回對映。
```
bluemix sl cdn origin-remove ACCOUNT_ID ORIGIN_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>
### bluemix sl cdn purge 
{: #sl_cdn_purge} 

從所有邊緣節點清除快取的檔案。
```
bluemix sl cdn purge ACCOUNT_ID CONTENT_URL [CONTENT_URL...] [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>
### bluemix sl file access-authorize 
{: #sl_file_access_authorize} 

授權主機存取給定的磁區。
```
bluemix sl file access-authorize VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --hardware-id</dt>
<dd>要授權的某部硬體伺服器的 ID。</dd>
<dt>-v, --virtual-id</dt>
<dd>要授權的某部虛擬伺服器的 ID。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要授權的某個 IP 位址的 ID。</dd>
<dt>-p, --ip-address</dt>
<dd>要授權的 IP 位址。</dd>
<dt>-s, --subnet-id</dt>
<dd>要授權的某個子網路的 ID。</dd>
</dl>

**範例**：
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
這個指令會授權 ID 為 87654321 的虛擬伺服器存取 ID 為 12345678 的磁區。

### bluemix sl file access-list 
{: #sl_file_access_list} 

列出 ACL。
```
bluemix sl file access-list VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、name、type、private_ip_address、host_iqn、username、password。</dd>
<dt>--columns</dt>
<dd>要顯示的直欄，選項包含：id、name、type、private_ip_address、host_iqn、username、password。</dd>
</dl>

**範例**：
```
bluemix sl file access-list 12345678 --sortby id
```
這個指令會列出獲授權存取 ID 為 12345678 的磁區的所有主機，並依 ID 排序。

### bluemix sl file access-revoke 
{: #sl_file_access_revoke} 

撤銷主機存取給定磁區的授權。
```
bluemix sl file access-revoke VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --hardware-id</dt>
<dd>要撤銷的某部硬體伺服器的 ID。</dd>
<dt>-v, --virtual-id</dt>
<dd>要撤銷的某部虛擬伺服器的 ID。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要撤銷的某個 IP 位址的 ID。</dd>
<dt>-p, --ip-address</dt>
<dd>要撤銷的 IP 位址。</dd>
<dt>-s, --subnet-id</dt>
<dd>要撤銷的某個子網路的 ID。</dd>
</dl>

**範例**：
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
這個指令會撤銷 ID 為 87654321 的虛擬伺服器對 ID 為 12345678 的磁區的存取權。

### bluemix sl file replica-failback 
{: #sl_file_replica_failback} 

從抄本進行檔案磁區失效回復。
```
bluemix sl file replica-failback VOLUME_ID
```


**範例**：
```
bluemix sl file replica-failback 12345678
```
這個指令會針對 ID 為 12345678 的磁區執行失效回復作業。

### bluemix sl file replica-failover 
{: #sl_file_replica_failover} 

將檔案磁區失效接手至給定的抄本磁區。
```
bluemix sl file replica-failover VOLUME_ID REPLICA_ID
```


**範例**：
```
bluemix sl file replica-failover 12345678 87654321
```
這個指令會執行將 ID 為 12345678 的磁區失效接手至 ID 為 87654321 的抄本磁區的作業。

### bluemix sl file replica-locations 
{: #sl_file_replica_locations} 

列出給定磁區的適當抄寫資料中心。
```
bluemix sl file replica-locations VOLUME_ID
```


**範例**：
```
bluemix sl file replica-locations 12345678
```
這個指令會列出 ID 為 12345678 的檔案磁區的適當抄寫資料中心。

### bluemix sl file replica-order 
{: #sl_file_replica_order} 

訂購檔案儲存空間抄本磁區。
```
bluemix sl file replica-order VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --snapshot-schedule</dt>
<dd>必要。要用於抄寫的 Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
<dt>-d, --datacenter</dt>
<dd>必要。抄本資料中心的簡稱，例如：dal09。</dd>
<dt>-t, --tier</dt>
<dd>選用。已訂購抄本之主要磁區的耐久性儲存空間層級（每 GB 的 IOPS），選項包含：0.25、2、4、10，如果未指定層級，將會使用原始磁區的層級。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間，如果未指定 IOPS，將會使用原始磁區的 IOPS。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
這個指令會訂購 ID 為 12345678 的磁區的抄本，此抄本會執行 DAILY 抄寫、位於 dal09、層級層次為 4。

### bluemix sl file replica-partners 
{: #sl_file_replica_partners} 

列出檔案磁區的現有抄本磁區。
```
bluemix sl file replica-partners VOLUME_ID [OPTIONS]
```


**範例**：
```
bluemix sl file replica-partners 12345678
```
這個指令會列出 ID 為 12345678 的檔案磁區的現有抄本磁區。

### bluemix sl file snapshot-cancel 
{: #sl_file_snapshot_cancel} 

取消給定磁區的現有 Snapshot 空間。
```
bluemix sl file snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--reason</dt>
<dd>選用性的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消 Snapshot 空間，而不是在計費週年日取消。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
這個指令會立即取消 ID 為 12345678 的 Snapshot，而不要求確認。

### bluemix sl file snapshot-create 
{: #sl_file_snapshot_create} 

在給定的磁區上建立 Snapshot。
```
bluemix sl file snapshot-create VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-n, --note</dt>
<dd>要設定於新 Snapshot 的附註。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
這個指令會針對 ID 為 12345678 的磁區建立 Snapshot，並新增附註 snapshotforbluemix。

### bluemix sl file snapshot-disable 
{: #sl_file_snapshot_disable} 

依給定磁區的指定排程停用 Snapshot。
```
bluemix sl file snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --schedule-type</dt>
<dd>必要。Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
這個指令會針對 ID 為 12345678 的磁區停用每日 Snapshot。

### bluemix sl file snapshot-enable 
{: #sl_file_snapshot_enable} 

依指定的排程為給定磁區啟用 Snapshot。
```
bluemix sl file snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --schedule-type</dt>
<dd>必要。Snapshot 排程，選項包含：HOURLY、DAILY、WEEKLY。</dd>
<dt>-c, --retention-count</dt>
<dd>必要。要保留的 Snapshot 數目。</dd>
<dt>-m, --minute</dt>
<dd>應該在幾分擷取 Snapshot，選項為 0 到 59 之間的整數。</dd>
<dt>-r, --hour</dt>
<dd>應該在幾點擷取 Snapshot，選項為 0 到 23 之間的整數。</dd>
<dt>-d, --day-of-week</dt>
<dd>應該在星期幾擷取 Snapshot，選項為 0 到 6 之間的整數。0 表示星期日、1 表示星期一、2 表示星期二、3 表示星期三、4 表示星期四、5 表示星期五、6 表示星期六。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
這個指令會針對 ID 為 12345678 的磁區啟用 Snapshot、在每週的星期日 2:00 擷取 Snapshot，且最多保留 5 個 Snapshot。

### bluemix sl file snapshot-delete 
{: #sl_file_snapshot_delete} 

在給定的磁區上刪除 Snapshot。
```
bluemix sl file snapshot-delete SNAPSHOT_ID
```


**範例**：
```
bluemix sl file snapshot-delete 12345678
```
這個指令會刪除 ID 為 12345678 的 Snapshot。

### bluemix sl file snapshot-list 
{: #sl_file_snapshot_list} 

列出檔案儲存空間 Snapshot。
```
bluemix sl file snapshot-list VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、name、created、size_bytes。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-list 12345678 --sortby id
```
這個指令會列出 ID 為 12345678 的磁區的所有 Snapshot，並依 ID 排序。

### bluemix sl file snapshot-order 
{: #sl_file_snapshot_order} 

訂購檔案儲存空間磁區的 Snapshot 空間。
```
bluemix sl file snapshot-order VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --size</dt>
<dd>必要。要建立的 Snapshot 空間大小（以 GB 為單位）。</dd>
<dt>-t, --tier</dt>
<dd>選用。已訂購空間之檔案磁區的耐久性儲存空間層級（每 GB 的 IOPS），選項包含：0.25、2、4、10。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間。</dd>
<dt>-u, --upgrade</dt>
<dd>該旗標指出訂單為升級。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
這個指令會針對 ID 為 12345678 的磁區訂購 Snapshot 空間、大小為 1000GB、層級層次為每 GB 4 個 IOPS。

### bluemix sl file snapshot-restore 
{: #sl_file_snapshot_restore} 

使用給定的 Snapshot 還原檔案磁區。
```
bluemix sl file snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**範例**：
```
bluemix sl file snapshot-restore 12345678 87654321
```
這個指令會從 ID 為 87654321 的 Snapshot 還原 ID 為 12345678 的磁區。

### bluemix sl file volume-cancel 
{: #sl_file_volume_cancel} 

取消現有的檔案儲存空間磁區。
```
bluemix sl file volume-cancel VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--reason</dt>
<dd>選用性的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消檔案儲存空間磁區，而不是在計費週年日取消。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
這個指令會立即取消 ID 為 12345678 的磁區，而不要求確認。

### bluemix sl file volume-list 
{: #sl_file_volume_list} 

列出檔案儲存空間。
```
bluemix sl file volume-list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-u, --username</dt>
<dd>依磁區使用者名稱過濾。</dd>
<dt>-d, --datacenter</dt>
<dd>依資料中心簡稱過濾。</dd>
<dt>-t, --storage-type</dt>
<dd>依儲存空間磁區的類型過濾，選項包含：performance、endurance。</dd>
<dt>-o, --order</dt>
<dd>依購買檔案儲存空間的訂單 ID 過濾。</dd>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、active_transactions、mount_addr。</dd>
<dt>--columns</dt>
<dd>要顯示的直欄，選項包含：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、mount_addr。</dd>
</dl>

**範例**：
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
這個指令會列出現行帳戶中位於 dal09 的所有耐久性磁區，並依容量排序。


### bluemix sl file volume-detail 
{: #sl_file_volume_detail} 

顯示指定磁區的詳細資料。
```
bluemix sl file volume-detail VOLUME_ID
```


**範例**：
```
bluemix sl file volume-detail 12345678
```
這個指令會顯示 ID 為 12345678 的磁區的詳細資料。

### bluemix sl file volume-duplicate 
{: #sl_file_volume_duplicate} 

複製現有磁區，以訂購檔案磁區。
```
bluemix sl file volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>要用於複製的原始磁區 Snapshot 的 ID。</dd>
<dt>-s, --duplicate-size</dt>
<dd>複製檔案磁區的大小（以 GB 為單位），如果未指定大小，將會使用原始磁區的大小。</dd>
<dt>-i, --duplicate-iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間，如果未指定 IOPS，將會使用原始磁區的 IOPS。</dd>
<dt>-t, --duplicate-tier</dt>
<dd>耐久性儲存空間層級，如果未指定層級，將會使用原始磁區的層級。</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>要針對複製項目訂購的 Snapshot 空間大小，如果未指定 Snapshot 空間大小，將會使用原始磁區的 Snapshot 空間大小。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file volume-duplicate 12345678
```
這個指令會顯示如何複製 ID 為 12345678 的磁區來訂購新磁區。

### bluemix sl file volume-order 
{: #sl_file_volume_order} 

訂購檔案儲存空間磁區。
```
bluemix sl file volume-order [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-t, --storage-type</dt>
<dd>必要。儲存空間磁區的類型，選項包含：performance、endurance。</dd>
<dt>-s, --size</dt>
<dd>必要。儲存空間磁區的大小（以 GB 為單位）。</dd>
<dt>-i, --iops</dt>
<dd>效能儲存空間 IOPS，此值為 100 的倍數，介於 100 與 6000 之間 [storage-type performance 的必要項目]。</dd>
<dt>-e, --tier</dt>
<dd>耐久性儲存空間層級（每 GB 的 IOP）[storage-type endurance 的必要項目]，選項包含：0.25、2、4、10。</dd>
<dt>-d, --datacenter</dt>
<dd>必要。資料中心簡稱。</dd>
<dt>-n, --snapshot-size</dt>
<dd>隨磁區訂購 Snapshot 空間的選用參數。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
這個指令會訂購效能磁區：大小為 1000GB、IOPS 為 4000、位於 dal09。

### bluemix sl file volume-options 
{: #sl_file_volume_options} 

列出用來訂購檔案儲存空間的所有選項。
```
bluemix sl file volume-options
```


**範例**：
```
bluemix sl file volume-options
```
這個指令會列出用來建立檔案儲存空間磁區的所有選項，包括儲存空間類型、磁區大小、IOPS、層級層次、資料中心及 Snapshot 大小。

### bluemix sl dns import 
{: #sl_dns_import} 

以 BIND 區域檔案為基礎匯入區域。
```
bluemix sl dns import ZONEFILE [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--dry-run</dt>
<dd>不要實際建立記錄。</dd>
</dl>

**範例**：
```
 bluemix sl dns import ~/blumix.net.txt
```
這個指令會從 ~/blumix.net.txt 檔案匯入區域及其資源記錄。

### bluemix sl dns record-add 
{: #sl_dns_record_add} 

在區域中新增資源記錄。
```
bluemix sl dns record-add ZONE RECORD TYPE DATA [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--ttl</dt>
<dd>TTL（存活時間）（以秒為單位），例如：86400，預設值為：7200。</dd>
</dl>

**範例**：
```
 bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
這個指令會將 A 記錄新增至 bluemix.net 區域，其主機為 "ftp"、資料為 "127.0.0.1"，而 ttl 為 86400 秒。

### bluemix sl dns record-edit 
{: #sl_dns_record_edit} 

更新區域中的資源記錄。
```
   bluemix sl dns record-edit ZONE [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--by-record</dt>
<dd>依主機記錄編輯，例如 www。</dd>
<dt>--by-id</dt>
<dd>依 ID 編輯單一記錄。</dd>
<dt>--data</dt>
<dd>記錄資料，例如 IP 位址。</dd>
<dt>--ttl</dt>
<dd>TTL 值（以秒為單位），例如：86400。</dd>
</dl>

**範例**：
```
 bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
這個指令會編輯 bluemix.net 區域下 ID 為 12345678 的記錄、將其資料設為 "127.0.0.2"，並將 ttl 設為 3600。

### bluemix sl dns record-list 
{: #sl_dns_record_list} 

列出區域中的所有資源記錄。
```
   bluemix sl dns record-list ZONE [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--data</dt>
<dd>依記錄資料過濾，例如 IP 位址。</dd>
<dt>--record</dt>
<dd>依主機記錄過濾，例如 www。</dd>
<dt>--ttl</dt>
<dd>依 TTL 值（以秒為單位）過濾，例如 86400。</dd>
<dt>--type</dt>
<dd>依記錄類型過濾，例如 A 或 CNAME。</dd>
</dl>

**範例**：
```
 bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
這個指令會列出 bluemix.net 區域下的所有 A 記錄、用來過濾的主機為 elasticsearch，而 ttl 為 900 秒。

### bluemix sl dns record-remove 
{: #sl_dns_record_remove} 

移除區域中的資源記錄。
```
 bluemix sl dns record-remove RECORD_ID
```


**範例**：
```
 bluemix sl dns record-remove 12345678
```
這個指令會移除 ID 為 12345678 的資源記錄。

### bluemix sl dns zone-create 
{: #sl_dns_zone_create} 

建立區域。
```
 bluemix sl dns zone-create ZONE
```


**範例**：
```
 bluemix sl dns zone-create bluemix.net
```
這個指令會建立名為 bluemix.net 的區域。

### bluemix sl dns zone-delete 
{: #sl_dns_zone_delete} 

刪除區域。
```
 bluemix sl dns zone-delete ZONE
```


**範例**：
```
 bluemix sl dns zone-delete bluemix.net
```
這個指令會刪除名為 bluemix.net 的區域。

### bluemix sl dns zone-list 
{: #sl_dns_zone_list} 

列出您帳戶上的所有區域。
```
   bluemix sl dns zone-list
```


**範例**：
```
   bluemix sl dns zone-list
```
這個指令會列出現行帳戶下的所有區域。

### bluemix sl dns zone-print 
{: #sl_dns_zone_print} 

以 BIND 格式列印區域及資源記錄。
```
 bluemix sl dns zone-print ZONE
```


**範例**：
```
 bluemix sl dns zone-print bluemix.net
```
這個指令會以 BIND 格式列印名為 bluemix.net 的區域。


### bluemix sl globalip create 
{: #sl_globalip_create} 

建立廣域 IP。
```
bluemix sl globalip create [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--v6</dt>
<dd>訂購 IPv6 IP 位址。</dd>
<dt>--test</dt>
<dd>測試訂購。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
     bluemix sl globalip create --v6
```
 這個指令會建立 IP V6 位址。

### bluemix sl globalip assign 
{: #sl_globalip_assign} 

將廣域 IP 指派給目標路由器或裝置。
```
bluemix sl globalip assign IDENTIFIER TARGET
```


**範例**：
```
 bluemix sl globalip assign 12345678 9.111.123.456
```
這個指令會將 ID 為 12345678 的 IP 位址指派給 IP 位址為 9.111.123.456 的目標裝置。


### bluemix sl globalip cancel 
{: #sl_globalip_cancel} 

取消廣域 IP。
```
bluemix sl globalip cancel IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl globalip cancel 12345678
```
這個指令會取消 ID 為 12345678 的 IP 位址。

### bluemix sl globalip list 
{: #sl_globalip_list} 

列出您帳戶上的所有廣域 IP。
```
bluemix sl globalip list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--v4</dt>
<dd>僅顯示 IPv4 IP。</dd>
<dt>--v6</dt>
<dd>僅顯示 IPv6 IP。</dd>
<dt>--order</dt>
<dd>依購買此 IP 位址的訂單 ID 過濾。</dd>
</dl>

**範例**：
```
bluemix sl globalip list --v4
```
這個指令會列出現行帳戶上的所有 IPV4 位址。

### bluemix sl globalip unassign 
{: #sl_globalip_unassign} 

取消指派目標路由器或裝置中的廣域 IP。
```
 bluemix sl globalip unassign IDENTIFIER
```


**範例**：
```
 bluemix sl globalip unassign 12345678
```
這個指令會取消指派目標裝置中 ID 為 12345678 的 IP 位址。

### bluemix sl image delete 
{: #sl_image_delete} 

刪除映像檔。
```
   bluemix sl image delete IDENTIFIER
```
**範例**：
```
   bluemix sl image delete 12345678
```
這個指令會刪除 ID 為 `12345678` 的映像檔。


### bluemix sl image detail 
{: #sl_image_detail} 

取得映像檔的詳細資料。
```
 bluemix sl image detail IDENTIFIER
```
**範例**：
```
 bluemix sl image detail 12345678
```
這個指令會取得 ID 為 12345678 的映像檔的詳細資料。

### bluemix sl image edit 
{: #sl_image_edit} 

編輯映像檔的詳細資料。
```
   bluemix sl image edit IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--name</dt>
<dd>映像檔的名稱。</dd>
<dt>--note</dt>
<dd>映像檔的其他附註。</dd>
<dt>--tag</dt>
<dd>映像檔的標籤。</dd>
</dl>

*範例**：
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
這個指令會編輯 ID 為 `12345678` 的映像檔、將名稱設為 `ubuntu16`、將附註設為 `testing`，並將標籤設為 `staging`。


### bluemix sl image list 
{: #sl_image_list} 

列出您帳戶上的所有映像檔。
```
   bluemix sl image list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--name</dt>
<dd>依映像檔名稱過濾。</dd>
<dt>--public</dt>
<dd>僅顯示公用映像檔。</dd>
<dt>--private</dt>
<dd>僅顯示專用映像檔。</dd>
</dl>

### bluemix sl ipsec cancel 
{: #sl_ipsec_cancel} 

取消 IPSec VPN 通道環境定義。
```
bluemix sl ipsec cancel CONTEXT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--immediate</dt>
<dd>立即取消 IPSec，而不是在計費週年日取消。</dd>
<dt>--reason</dt>
<dd>選用性的取消原因。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl ipsec config 
{: #sl_ipsec_config} 

通道環境定義的要求配置。
```
bluemix sl ipsec config CONTEXT_ID [OPTIONS]
```

### bluemix sl ipsec detail 
{: #sl_ipsec_detail} 

列出 IPSec VPN 通道環境定義詳細資料。
```
bluemix sl ipsec detail CONTEXT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-i, --include</dt>
<dd>包括其他資源，選項包含：at、is、rs、sr、ss。</dd>
</dl>
### bluemix sl ipsec list 
{: #sl_ipsec_list} 

列出 IPSec VPN 通道環境定義。
```
bluemix sl ipsec list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--order</dt>
<dd>依購買 IPSEC 的訂單 ID 過濾。</dd>
</dl>
### bluemix sl ipsec order 
{: #sl_ipsec_order} 

訂購 IPSec VPN 通道。
```
bluemix sl ipsec order [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --datacenter</dt>
<dd>必要。IPSEC 資料中心的簡稱，例如：dal09。</dd>
</dl>

### bluemix sl ipsec subnet-add 
{: #sl_ipsec_subnet_add} 

將子網路新增至 IPSec 通道環境定義。
```
bluemix sl ipsec subnet-add CONTEXT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --subnet-id</dt>
<dd>要新增的子網路 ID，必要項目。</dd>
<dt>-t, --subnet-type</dt>
<dd>要新增的子網路類型，必要項目，選項包含：internal、remote、service。</dd>
<dt>-n, --network</dt>
<dd>要建立的子網路 ID。</dd>
</dl>

### bluemix sl ipsec subnet-remove 
{: #sl_ipsec_subnet_remove} 

從 IPSEC 通道環境定義移除子網路。
```
bluemix sl ipsec subnet-remove CONTEXT_ID SUBNET_ID SUBNET_TYPE [OPTIONS]
```

### bluemix sl ipsec translation-add 
{: #sl_ipsec_translation_add} 

將位址轉換新增至 IPSec 通道。
```
bluemix sl ipsec translation-add CONTEXT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --static-ip</dt>
<dd>靜態 IP 位址，必要項目。</dd>
<dt>-r, --remote-ip</dt>
<dd>遠端 IP 位址，必要項目。</dd>
<dt>-n, --note</dt>
<dd>附註。</dd>
</dl>
### bluemix sl ipsec translation-remove 
{: #sl_ipsec_translation_remove} 

從 IPSec 移除轉換項目。
```
bluemix sl ipsec translation-remove CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

### bluemix sl ipsec translation-update 
{: #sl_ipsec_translation_update} 

更新 IPSec 的位址轉換。
```
bluemix sl ipsec translation-update CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-s, --static-ip</dt>
<dd>靜態 IP 位址，必要項目。</dd>
<dt>-r, --remote-ip</dt>
<dd>遠端 IP 位址，必要項目。</dd>
<dt>-n, --note</dt>
<dd>附註。</dd>
</dl>
### bluemix sl ipsec update 
{: #sl_ipsec_update} 

更新通道環境定義內容。
```
bluemix sl ipsec update CONTEXT_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-n, --name</dt>
<dd>一般名稱。</dd>
<dt>-r, --remote-peer</dt>
<dd>遠端對等節點 IP 位址。</dd>
<dt>-k, --preshared-key</dt>
<dd>預先共用金鑰。</dd>
<dt>-a, --phase1-auth</dt>
<dd>階段 1 鑑別，選項包含：MD5、SHA1、SHA256。</dd>
<dt>-c, --phase1-crypto</dt>
<dd>階段 1 加密，選項包含：DES、3DES、AES128、AES192、AES256。</dd>
<dt>-d, --phase1-dh</dt>
<dd>階段 1 Diffie Hellman 群組，選項包含：0、1、2、5。</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>階段 1 金鑰使用期限，範圍為 120-172800。</dd>
<dt>-u, --phase2-auth</dt>
<dd>階段 2 鑑別，選項包含：MD5、SHA1、SHA256。</dd>
<dt>-y, --phase2-crypto</dt>
<dd>階段 2 加密，選項包含：DES、3DES、AES128、AES192、AES256。</dd>
<dt>-e, --phase2-dh</dt>
<dd>階段 2 Diffie Hellman 群組，選項包含：0、1、2、5。</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>階段 2 完全秘密轉遞，範圍為 0-1。</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>階段 2 金鑰使用期限，範圍為 120-172800。</dd>
</dl>

### bluemix sl loadbal cancel 
{: #sl_loadbal_cancel} 

取消現有負載平衡器。
```
bluemix sl loadbal cancel LOADBAL_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl loadbal create 
{: #sl_loadbal_create} 

提供從 create-options 傳回的 ID，以新增負載平衡器。
```
bluemix sl loadbal create PRICE_ID LOCATION [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl loadbal create-options 
{: #sl_loadbal_create_options} 

取得用來建立負載平衡器的價格選項。
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail 
{: #sl_loadbal_detail} 

取得負載平衡器詳細資料。
```
bluemix sl loadbal detail LOADBAL_ID
```

### bluemix sl loadbal group-add 
{: #sl_loadbal_group_add} 

新增 load_balancer 服務。
```
bluemix sl loadbal group-add LOADBAL_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-a, --allocation</dt>
<dd>必要。已配置的連線百分比。</dd>
<dt>-p, --port</dt>
<dd>必要。埠號。</dd>
<dt>-t, --routing-type</dt>
<dd>必要。遞送類型的 ID。請執行 'bluemix sl loadbal routing-types' 以尋找 ID。</dd>
<dt>-m, --routing-method</dt>
<dd>必要。遞送方法的 ID。請執行 'bluemix sl loadbal routing-methods' 以尋找 ID。</dd>
</dl>

### bluemix sl loadbal group-delete 
{: #sl_loadbal_group_delete} 

刪除現有負載平衡器服務群組。
```
bluemix sl loadbal group-delete GROUP_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl loadbal group-edit 
{: #sl_loadbal_group_edit} 

編輯現有負載平衡器服務群組。
```
bluemix sl loadbal group-edit LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-a, --allocation</dt>
<dd>變更已配置的連線百分比。</dd>
<dt>-p, --port</dt>
<dd>變更埠號。</dd>
<dt>-t, --routing-type</dt>
<dd>變更遞送類型的 ID。請執行 'bluemix sl loadbal routing-types' 以尋找 ID。</dd>
<dt>-m, --routing-method</dt>
<dd>變更遞送方法的 ID。請執行 'bluemix sl loadbal routing-methods' 以尋找 ID。</dd>
</dl>

### bluemix sl loadbal group-reset 
{: #sl_loadbal_group_reset} 

重設特定服務群組上的連線。
```
bluemix sl loadbal group-reset LOADBAL_ID GROUP_ID
```

### bluemix sl loadbal health-checks 
{: #sl_loadbal_health_checks} 

列出性能檢查類型。
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list 
{: #sl_loadbal_list} 

列出作用中的負載平衡器。
```
bluemix sl loadbal list
```

<strong>指令選項</strong>：
<dl>
<dt>-d, --datacenter</dt>
<dd>依資料中心簡稱過濾。</dd>
<dt>-o, --order</dt>
<dd>依購買負載平衡器的訂單 ID 過濾。</dd>
<dt>-p, --ip-address</dt>
<dd>依 IP 位址過濾。</dd>
</dl>
### bluemix sl loadbal routing-methods 
{: #sl_loadbal_routing_methods} 

列出遞送方法。
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types 
{: #sl_loadbal_routing_types} 

列出遞送類型。
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add 
{: #sl_loadbal_service_add} 

新增負載平衡器服務。
```
bluemix sl loadbal service-add LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--disabled</dt>
<dd>選用。將服務建立為 disabled，如果未指定，則預設為 enabled。</dd>
<dt>-p, --port</dt>
<dd>必要。服務的埠號。</dd>
<dt>-w, --weight</dt>
<dd>必要。服務的加權。</dd>
<dt>-t, --healthcheck-type</dt>
<dd>必要。性能檢查類型。</dd>
<dt>-i, --ip-address</dt>
<dd>必要。服務的 IP 位址。</dd>
</dl>

### bluemix sl loadbal service-delete 
{: #sl_loadbal_service_delete} 

刪除現有負載平衡器服務。
```
bluemix sl loadbal service-delete SERVICE_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl loadbal service-edit 
{: #sl_loadbal_service_edit} 

編輯服務群組的內容。
```
bluemix sl loadbal service-edit LOADBAL_ID SERVICE_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--disabled</dt>
<dd>停用服務。</dd>
<dt>--enabled</dt>
<dd>啟用服務。</dd>
<dt>-p, --port</dt>
<dd>變更服務的埠號。</dd>
<dt>-w, --weight</dt>
<dd>變更服務的加權。</dd>
<dt>-t, --healthcheck-type</dt>
<dd>變更性能檢查類型。</dd>
<dt>-i, --ip-address</dt>
<dd>變更服務的 IP 位址。</dd>
</dl>

### bluemix sl loadbal service-toggle 
{: #sl_loadbal_service_toggle} 

切換現有負載平衡器服務的狀態。
```
bluemix sl loadbal service-toggle SERVICE_ID
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

### bluemix sl security sshkey-add 
{: #sl_security_sshkey_add} 

新增 SSH 金鑰。
```
 bluemix sl security sshkey-add LABEL [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --in-file</dt>
<dd>要為此金鑰匯入的 id_rsa.pub 檔案。</dd>
<dt>-k, --key</dt>
<dd>實際 SSH 金鑰。</dd>
<dt>--note</dt>
<dd>將與金鑰相關聯的額外附註。</dd>
</dl>

**範例**：
```
 bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
這個指令會從檔案 ~/.ssh/id_rsa.pub 新增 SSH 金鑰及附註 "mykey"。


### bluemix sl security sshkey-edit 
{: #sl_security_sshkey_edit} 

編輯 SSH 金鑰。
```
 bluemix sl security sshkey-edit IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--label</dt>
<dd>金鑰的新標籤。</dd>
<dt>--note</dt>
<dd>金鑰的新附註。</dd>
</dl>

**範例**：
```
 bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
這個指令會更新 ID 為 12345678 的 SSH 金鑰、將標籤設為 "Bluemix"，並將附註設為 "testing"。

### bluemix sl security sshkey-list 
{: #sl_security_sshkey_list} 

列出您帳戶上的 SSH 金鑰。
```
 bluemix sl security sshkey-list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、label、fingerprint、notes。</dd>
</dl>

**範例**：
```
 bluemix sl security sshkey-list --sortby label
```
 這個指令會列出現行帳戶上的所有 SSH 金鑰，並依標籤排序。

### bluemix sl security sshkey-print 
{: #sl_security_sshkey_print} 

將 SSH 金鑰印出至螢幕。
```
 bluemix sl security sshkey-print IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --out-file</dt>
<dd>公用 SSH 金鑰將會寫入此檔案。</dd>
</dl>

**範例**：
```
 bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
這個指令會顯示 ID 為 12345678 的 SSH 金鑰的 ID、標籤及附註，並將公開金鑰寫入檔案：~/mykey.pub。

### bluemix sl security sshkey-remove 
{: #sl_security_sshkey_remove} 

永久移除 SSH 金鑰。
```
 bluemix sl security sshkey-remove IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl security sshkey-remove 12345678 -f
```
 這個指令會移除 ID 為 12345678 的 SSH 金鑰，而不要求確認。

### bluemix sl security cert-add 
{: #sl_security_cert_add} 

新增及上傳 SSL 憑證詳細資料。
```
 bluemix sl security cert-add [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--crt</dt>
<dd>憑證檔。</dd>
<dt>--csr</dt>
<dd>憑證簽署要求檔。</dd>
<dt>--icc</dt>
<dd>中繼憑證檔。</dd>
<dt>--key</dt>
<dd>私密金鑰檔。</dd>
<dt>--notes</dt>
<dd>其他附註。</dd>
</dl>

**範例**：
```
 bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key 
```
 這個指令會新增網域 bluemix.net 的憑證檔 ~/bluemix.net.cert 及私密金鑰檔 ~/bluemix.net.key。

### bluemix sl security cert-edit 
{: #sl_security_cert_edit} 

編輯 SSL 憑證。
```
 bluemix sl security cert-edit IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--crt</dt>
<dd>憑證檔。</dd>
<dt>--csr</dt>
<dd>憑證簽署要求檔。</dd>
<dt>--icc</dt>
<dd>中繼憑證檔。</dd>
<dt>--key</dt>
<dd>私密金鑰檔。</dd>
<dt>--notes</dt>
<dd>其他附註。</dd>
</dl>

**範例**：
```
 bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
 這個指令會編輯 ID 為 12345678 的憑證，並以檔案 ~/bluemix.net.key 來更新其私密金鑰。

### bluemix sl security cert-download 
{: #sl_security_cert_download} 

下載 SSL 憑證及金鑰檔。
```
 bluemix sl security cert-download IDENTIFIER
```


**範例**：
```
 bluemix sl security cert-download 12345678
```
  這個指令會將 4 個檔案下載至 ID 為 12345678 的憑證的現行目錄。這 4 個檔案分別為：憑證檔、憑證簽署要求檔、中繼憑證檔及私密金鑰檔。

### bluemix sl security cert-list 
{: #sl_security_cert_list} 

列出您帳戶上的 SSL 憑證。
```
 bluemix sl security cert-list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--status</dt>
<dd>顯示具有以下狀態的憑證，預設值為：all，選項包含：all、valid、expired。</dd>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、common_name、days_until_expire、notes。</dd>
</dl>

**範例**：
```
 bluemix sl security cert-list --status valid --sortby days_until_expire
```
 這個指令會列出現行帳戶上的所有有效憑證，並依有效天數排序。

### bluemix sl security cert-remove 
{: #sl_security_cert_remove} 

移除 SSL 憑證。
```
 bluemix sl security cert-remove IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl security cert-remove 12345678
```
 這個指令會移除 ID 為 12345678 的憑證。

### bluemix sl subnet cancel 
{: #sl_subnet_cancel} 

取消子網路。
```
bluemix sl subnet cancel IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl subnet cancel 12345678 -f
```
這個指令會取消 ID 為 12345678 的子網路，而不要求確認。

### bluemix sl subnet create 
{: #sl_subnet_create} 

將新子網路新增至您的帳戶。
```
   bluemix sl subnet create NETWORK QUANTITY VLAN_ID [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--v6, --ipv6</dt>
<dd>訂購 IPv6 位址。</dd>
<dt>--test</dt>
<dd>不要訂購子網路；只要取得報價。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl subnet create public 16 567
```
這個指令會建立含有 16 個 IP V4 位址的公用子網路，並將其放在 ID 為 567 的 VLAN 上。



### bluemix sl subnet detail 
{: #sl_subnet_detail} 

取得子網路的詳細資料。
```
   bluemix sl subnet detail IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--no-vs</dt>
<dd>隱藏虛擬伺服器清單。</dd>
<dt>--no-hardware</dt>
<dd>隱藏硬體清單。</dd>
</dl>

**範例**：
```
 bluemix sl subnet detail 12345678
```
這個指令會顯示 ID 為 12345678 的子網路的詳細資訊，包括虛擬伺服器及硬體伺服器資訊。


### bluemix sl subnet list 
{: #sl_subnet_list} 

列出您帳戶上的所有子網路。
```
   bluemix sl subnet list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式。選項包含：id、identifier、type、network_space、datacenter、vlan_id、IPs、hardware、vs。</dd>
<dt>-d, --datacenter</dt>
<dd>依資料中心簡稱過濾。</dd>
<dt>--identifier</dt>
<dd>依網路 ID 過濾。</dd>
<dt>-t, --subnet-type</dt>
<dd>依子網路類型過濾。</dd>
<dt>--network-space</dt>
<dd>依網路空間過濾。</dd>
<dt>--v4, --ipv4</dt>
<dd>僅顯示 IPv4 子網路。</dd>
<dt>--v6, --ipv6</dt>
<dd>僅顯示 IPv6 子網路。</dd>
<dt>--order</dt>
<dd>依購買子網路的訂單 ID 過濾。</dd>
</dl>

**範例**：
```
 bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
這個指令會列出現行帳戶上的 IP V4 子網路，用來過濾的資料中心為 dal09、子網路類型為 PRIMARY，而網路空間為 PUBLIC。



### bluemix sl subnet lookup 
{: #sl_subnet_lookup} 

尋找 IP 位址，並顯示其子網路及裝置資訊。
```
   bluemix sl subnet lookup IP_ADDRESS
```


**範例**：
```
 bluemix sl subnet lookup 9.125.235.255
```
這個指令會尋找位址為 9.125.235.255 的 IP 位址記錄，並顯示其子網路及裝置資訊。


### bluemix sl vlan create 
{: #sl_vlan_create} 

建立新的 VLAN。
```
   bluemix sl vlan create [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-t, --vlan-type</dt>
<dd>VLAN 的類型，可以是公用或專用。</dd>
<dt>-r, --router</dt>
<dd>路由器的主機名稱。</dd>
<dt>-d, --datacenter</dt>
<dd>資料中心的簡稱。</dd>
<dt>-s, --size</dt>
<dd>子網路的大小，選項包含：8（5 個可用的 IP）或 16（13 個可用的 IP）或 32（29 個可用的 IP）。</dd>
<dt>-n, --name</dt>
<dd>VLAN 的名稱。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
這個指令會建立一個公用 VLAN：位於資料中心 dal09、包含 16 個 IP 位址，且名稱為 myvlan。
### bluemix sl vlan cancel 
{: #sl_vlan_cancel} 

取消 VLAN。
```
   bluemix sl vlan cancel IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
   bluemix sl vlan cancel 12345678 -f
```
這個指令會取消 ID 為 12345678 的 VLAN，而不要求確認。



### bluemix sl vlan detail 
{: #sl_vlan_detail} 

取得 VLAN 的詳細資料。
```
   bluemix sl vlan detail IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--no-vs</dt>
<dd>隱藏虛擬伺服器清單。</dd>
<dt>--no-hardware</dt>
<dd>隱藏硬體清單。</dd>
</dl>

**範例**：
```
 bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
這個指令會顯示 ID 為 12345678 的 VLAN 詳細資料，而不會列出虛擬伺服器或硬體伺服器。


### bluemix sl vlan edit 
{: #sl_vlan_edit} 

編輯 VLAN 的詳細資料。
```
   bluemix sl vlan edit IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-n, --name</dt>
<dd>VLAN 的名稱。</dd>
</dl>

**範例**：
```
 bluemix sl vlan edit 12345678 -n myvlan-rename
```
這個指令會更新 ID 為 12345678 的 VLAN，並為其指定新名稱 "myvlan-rename"。


### bluemix sl vlan list 
{: #sl_vlan_list} 

列出您帳戶上的所有 VLAN。
```
 bluemix sl vlan list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、number、name、firewall、datacenter、hardware、virtual_servers、public_ips。</dd>
<dt>-d, --datacenter</dt>
<dd>依資料中心簡稱過濾。</dd>
<dt>-n, --number</dt>
<dd>依 VLAN 號碼過濾。</dd>
<dt>--name</dt>
<dd>依 VLAN 名稱過濾。</dd>
<dt>--order</dt>
<dd>依購買 VLAN 的訂單 ID 過濾。</dd>
</dl>

**範例**：
```
 bluemix sl vlan list -d dal09 --sortby number
```
這個指令會列出現行帳戶上的所有 VLAN，用來過濾的資料中心為 dal09，並依 VLAN 號碼排序。




### bluemix sl vlan options 
{: #sl_vlan_options} 

列出用來建立 VLAN 的所有選項。
```
 bluemix sl vlan options
```


**範例**：
```
 bluemix sl vlan options
```
這個指令會列出用來建立 VLAN 的所有選項，例如 VLAN 類型、資料中心、子網路大小、路由器等等。
### bluemix sl vs cancel 
{: #sl_vs_cancel} 

取消虛擬伺服器實例。
```
   bluemix sl vs cancel IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs cancel 12345678
```
這個指令會取消 ID 為 12345678 的虛擬伺服器實例。


### bluemix sl vs capture 
{: #sl_vs_capture} 

將虛擬伺服器實例擷取至映像檔。
```
 bluemix sl vs capture IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-n, --name</dt>
<dd>必要。映像檔的名稱。</dd>
<dt>--all</dt>
<dd>擷取屬於 VS 的所有磁碟。</dd>
<dt>--note</dt>
<dd>新增要與映像檔相關聯的附註。</dd>
</dl>

**範例**：
```
 bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
這個指令會將 ID 為 12345678 的虛擬伺服器實例及其所有磁碟都擷取至名為 "mybluemix" 且附註為 "testing" 的映像檔。



### bluemix sl vs create 
{: #sl_vs_create} 

建立虛擬伺服器實例。
```
   bluemix sl vs create [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-H, --hostname</dt>
<dd>必要。FQDN 的主機部分。</dd>
<dt>-D, --domain</dt>
<dd>必要。FQDN 的網域部分。</dd>
<dt>-c, --cpu</dt>
<dd>必要。CPU 核心數目。</dd>
<dt>-m, --memory</dt>
<dd>必要。記憶體（以 MB 為單位）。</dd>
<dt>-d, --datacenter</dt>
<dd>必要。資料中心簡稱。</dd>
<dt>-o, --os</dt>
<dd>OS 安裝程式碼。提示：您可以指定 <OS>_LATEST。</dd>
<dt>--image</dt>
<dd>映像檔 ID。如需參考資料，請參閱：'bluemix sl image list'。</dd>
<dt>--billing</dt>
<dd>計費頻率。預設值為：hourly。選項包含：hourly、monthly。</dd>
<dt>--dedicated</dt>
<dd>建立專用虛擬伺服器（專用節點）。</dd>
<dt>--san</dt>
<dd>使用 SAN 儲存空間，而不是本端磁碟。</dd>
<dt>--test</dt>
<dd>不要實際建立虛擬伺服器。</dd>
<dt>--export</dt>
<dd>將選項匯出至範本檔。</dd>
<dt>-i, --postinstall</dt>
<dd>要下載的後置安裝 Script。</dd>
<dt>-k, --key</dt>
<dd>要新增至 root 使用者的 SSH 金鑰 ID（允許多次出現的項目）。</dd>
<dt>--disk</dt>
<dd>磁碟大小（允許多次出現的項目）。</dd>
<dt>--private</dt>
<dd>強制虛擬伺服器只能存取專用網路。</dd>
<dt>--like</dt>
<dd>使用現有虛擬伺服器的配置。</dd>
<dt>-n, --network</dt>
<dd>網路埠速度 (Mbps)。</dd>
<dt>--tag</dt>
<dd>要新增至實例的標籤（允許多次出現的項目）。</dd>
<dt>-t, --template</dt>
<dd>預設指令行選項的範本檔。</dd>
<dt>-u, --userdata</dt>
<dd>使用者定義的 meta 資料字串。</dd>
<dt>-F, --userfile</dt>
<dd>從檔案讀取使用者資料。</dd>
<dt>--vlan-public</dt>
<dd>要放置虛擬伺服器的公用 VLAN 的 ID。</dd>
<dt>--vlan-private</dt>
<dd>要放置虛擬伺服器的專用 VLAN 的 ID。</dd>
<dt>--wait</dt>
<dd>等待虛擬伺服器完成佈建，最多 X 秒後才返回。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
  bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
這個指令會訂購虛擬伺服器實例，其主機名稱為 myvsi、網域為 bluemix.net、有 4 個 CPU 核心及 4096M 的記憶體，位於資料中心：dal10。

### bluemix sl vs options 
{: #sl_vs_options} 

列出用來建立虛擬伺服器實例的選項。
```
   bluemix sl vs options [OPTIONS]
```


**範例**：
```
 bluemix sl vs options
```
這個指令會列出用來建立虛擬伺服器實例的所有選項，例如資料中心、CPU、記憶體、OS、磁碟、網路速度等等。



### bluemix sl vs credentials 
{: #sl_vs_credentials} 

列出虛擬伺服器實例認證。
```
   bluemix sl vs credentials IDENTIFIER [OPTIONS]
```


**範例**：
```
 bluemix sl vs credentials 12345678
```
這個指令會列出 ID 為 12345678 的虛擬伺服器實例的所有使用者名稱及密碼配對。

### bluemix sl vs detail 
{: #sl_vs_detail} 

取得虛擬伺服器實例的詳細資料。
```
   bluemix sl vs detail IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--passwords</dt>
<dd>顯示密碼（小心背後有人偷窺！）。</dd>
<dt>--price</dt>
<dd>顯示關聯的價格。</dd>
</dl>

**範例**：
```
   bluemix sl vs details 12345678
```
這個指令會列出 ID 為 12345678 的虛擬伺服器實例的詳細資訊。


### bluemix sl vs dns-sync 
{: #sl_vs_dns_sync} 

為虛擬伺服器實例同步 DNS 記錄。
```
   bluemix sl vs dns-sync IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-a, --a-record</dt>
<dd>為主機同步 A 記錄。</dd>
<dt>--aaaa-record</dt>
<dd>為主機同步 AAAA 記錄。</dd>
<dt>--ptr</dt>
<dd>為主機同步 PTR 記錄。</dd>
<dt>--ttl</dt>
<dd>設定 A 及（或）PTR 記錄的 TTL，預設值為：7200。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
這個指令會將 ID 為 12345678 的虛擬伺服器實例的 A 記錄（IP V4 位址）同步至 DNS 伺服器，並將這個 A 記錄的 ttl 設為 3600。
### bluemix sl vs edit 
{: #sl_vs_edit} 

編輯虛擬伺服器實例的詳細資料。
```
   bluemix sl vs edit IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-D, --domain</dt>
<dd>FQDN 的網域部分。</dd>
<dt>-H, --hostname</dt>
<dd>FQDN 的主機部分。範例：server。</dd>
<dt>--tag</dt>
<dd>要設定的標籤，或使用空字串以便全部移除。</dd>
<dt>-u, --userdata</dt>
<dd>使用者定義的 meta 資料字串。</dd>
<dt>-F, --userfile</dt>
<dd>從檔案讀取使用者資料。</dd>
<dt>--public-speed</dt>
<dd>公用埠速度，選項包含：0、10、100、1000、10000。</dd>
<dt>--private-speed</dt>
<dd>專用埠速度，選項包含：0、10、100、1000、10000。</dd>
</dl>

**範例**：
```
 bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
這個指令會更新 ID 為 12345678 的虛擬伺服器實例，並將其網域設為 "bluemix.net"、將主機名稱設為 "myapp"、將標籤設為 "testcli"。

### bluemix sl vs list 
{: #sl_vs_list} 

列出您帳戶上的虛擬伺服器實例。
```
   bluemix sl vs list [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-c, --cpu</dt>
<dd>CPU 核心數目。</dd>
<dt>-D, --domain</dt>
<dd>FQDN 的網域部分。</dd>
<dt>-d, --datacenter</dt>
<dd>資料中心簡稱。</dd>
<dt>-H, --hostname</dt>
<dd>FQDN 的主機部分。</dd>
<dt>-m, --memory</dt>
<dd>記憶體（以 MB 為單位）。</dd>
<dt>-n, --network</dt>
<dd>網路埠速度 (Mbps)。</dd>
<dt>--hourly</dt>
<dd>僅顯示每小時實例。</dd>
<dt>--monthly</dt>
<dd>僅顯示每月實例。</dd>
<dt>--tag</dt>
<dd>依標籤過濾（允許多次出現的項目）。</dd>
<dt>--sortby</dt>
<dd>直欄排序方式，選項包含：id、hostname、domain、datacenter、cpu、memory、primary_ip、backend_ip。預設值為：hostname。</dd>
<dt>--columns</dt>
<dd>要顯示的直欄，選項包含：guid、primary_ip、backend_ip、datacenter、action、power_state、created_by、tags。預設值為：id、hostname、primary_ip、backend_ip、datacenter、action。</dd>
</dl>

**範例**：
```
 bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
這個指令會列出現行帳戶上所有依時數計費的虛擬伺服器實例，用來過濾的網域為 "bluemix.net"，並依記憶體排序。



### bluemix sl vs pause 
{: #sl_vs_pause} 

暫停作用中虛擬伺服器實例。
```
   bluemix sl vs pause IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs pause 12345678 -f
```
   這個指令會暫停 ID 為 12345678 的虛擬伺服器實例，而不要求確認。



### bluemix sl vs power-off 
{: #sl_vs_power_off} 

關閉作用中虛擬伺服器實例。
```
   bluemix sl vs power-off IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--hard</dt>
<dd>執行強迫關機。</dd>
<dt>--soft</dt>
<dd>執行正常關機。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
   bluemix sl vs power-off 12345678 --soft
```
這個指令會針對 ID 為 12345678 的虛擬伺服器實例執行正常關機。

### bluemix sl vs power-on 
{: #sl_vs_power_on} 

啟動虛擬伺服器實例。
```
 bluemix sl vs power-on IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs power-on 12345678
```
這個指令會針對 ID 為 12345678 的虛擬伺服器實例執行開機作業。


### bluemix sl vs ready 
{: #sl_vs_ready} 

檢查是否有虛擬伺服器實例已備妥可供使用。
```
 bluemix sl vs ready IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--wait</dt>
<dd>等待虛擬伺服器完成佈建，最多 X 秒後才返回。</dd>
</dl>

**範例**：
```
 bluemix sl vs ready 12345678 --wait 30
```
這個指令會檢查 ID 為 12345678 的虛擬伺服器實例狀態，以查看它是否準備好可繼續使用，最多等待 30 秒。

### bluemix sl vs reboot 
{: #sl_vs_reboot} 

將作用中虛擬伺服器實例重新開機。
```
 bluemix sl vs reboot IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>--hard</dt>
<dd>執行強迫重新開機。</dd>
<dt>--soft</dt>
<dd>執行正常重新開機。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs reboot 12345678 --hard
```
這個指令會針對 ID 為 12345678 的虛擬伺服器實例執行強迫重新開機。



### bluemix sl vs reload 
{: #sl_vs_reload} 

在虛擬伺服器實例上重新載入作業系統。
```
 bluemix sl vs reload IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-i, --postinstall</dt>
<dd>要下載的後置安裝 Script。</dd>
<dt>--image</dt>
<dd>映像檔 ID。預設值為使用現行作業系統。
</dd>
<dt>請參閱：</dt>
<dd>'bluemix sl image list' 以取得參考資料。</dd>
<dt>-k, --key</dt>
<dd>要新增至 root 使用者的 SSH 金鑰 ID（允許多次出現的項目）。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
   bluemix sl vs reload 12345678
```
這個指令會針對 ID 為 12345678 的虛擬伺服器實例重新載入現行作業系統。
### bluemix sl vs rescue 
{: #sl_vs_rescue} 

將虛擬伺服器實例重新開機至救援映像檔。
```
 bluemix sl vs rescue IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs rescue 12345678
```
這個指令會將 ID 為 12345678 的虛擬伺服器實例重新開機至救援映像檔。


### bluemix sl vs resume 
{: #sl_vs_resume} 

繼續已暫停的虛擬伺服器實例。
```
   bluemix sl vs resume IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs resume 12345678
```
這個指令會繼續 ID 為 12345678 的虛擬伺服器實例。


### bluemix sl vs upgrade 
{: #sl_vs_upgrade} 

升級虛擬伺服器實例。
```
   bluemix sl vs upgrade IDENTIFIER [OPTIONS]
```

<strong>指令選項</strong>：
<dl>
<dt>-c, --cpu</dt>
<dd>CPU 核心數目。</dd>
<dt>--private</dt>
<dd>CPU 核心將會在專用的主伺服器上。</dd>
<dt>-m, --memory</dt>
<dd>記憶體（以 MB 為單位）。</dd>
<dt>--network</dt>
<dd>網路埠速度 (Mbps)。</dd>
<dt>-f, --force</dt>
<dd>強制執行作業，而不進行確認。</dd>
</dl>

**範例**：
```
 bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
這個指令會升級 ID 為 12345678 的虛擬伺服器實例，並將 CPU 核心數目設為 8、將記憶體設為 8192M、將網路埠速度設為 1000 Mbps。

