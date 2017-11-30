---

copyright:

  years: 2016,2017

lastupdated: "2017-09-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) 命令
{: #softlayer_cli}

{{site.data.keyword.BluSoftlayer}} 插件已合并到 {{site.data.keyword.Bluemix_notm}} CLI 中。您不再需要安装该插件。

使用 {{site.data.keyword.Bluemix_notm}} 命令行界面 (CLI) 中的 {{site.data.keyword.BluSoftlayer_notm}} 命令来配置和管理 SoftLayer 服务。


首先，请安装 IBM {{site.data.keyword.Bluemix_notm}} CLI。有关详细信息，请参阅 [Bluemix CLI ![外部链接图标](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window}。

要获取 {{site.data.keyword.Bluemix_notm}} 命令的完整列表，请参阅：[{{site.data.keyword.Bluemix_notm:}} (bx) 命令](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)


## 常规 {{site.data.keyword.BluSoftlayer_notm}} 命令

支持以下命令。使用 `bluemix sl` 命令可查看可用命令的列表：

<table summary="按字母顺序列出的常规命令（命令具有可获取命令更多信息的链接）">
<caption>表 1. 常规 Softlayer 命令</caption>
 <thead>
 <th colspan="6">常规 Softlayer 命令</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## {{site.data.keyword.BluSoftlayer_notm}} 块存储器命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 2. Softlayer 块存储器</caption>
 <thead>
 <th colspan="6">Softlayer 块存储器</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} CDN 命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
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

## {{site.data.keyword.BluSoftlayer_notm}} 文件存储器命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 4. Softlayer 文件存储器</caption>
 <thead>
 <th colspan="6">Softlayer 文件存储器</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} DNS 命令

<table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 5. Softlayer DNS 命令</caption>
 <thead>
 <th colspan="6">Softlayer DNS 命令</th>
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

<table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 6. Softlayer 全局 IP 命令</caption>
 <thead>
 <th colspan="6">Softlayer 全局 IP 命令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 映像命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 7. Softlayer 映像命令</caption>
 <thead>
 <th colspan="6">Softlayer 映像命令</th>
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
 
 ## {{site.data.keyword.BluSoftlayer_notm}} IPSec VPN 命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 7. Softlayer IPSec VPN 命令</caption>
 <thead>
 <th colspan="6">Softlayer IPSec VPN 命令</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} 负载均衡器命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 8. Softlayer 负载均衡器命令</caption>
 <thead>
 <th colspan="6">Softlayer 负载均衡器命令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 安全命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 9. Softlayer 安全性命令</caption>
 <thead>
 <th colspan="5">Softlayer 安全命令</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 子网命令
 
 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 10. Softlayer 子网命令</caption>
 <thead>
 <th colspan="5">Softlayer 子网命令</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} 虚拟服务器命令

 <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 11. Softlayer 虚拟服务器命令</caption>
 <thead>
 <th colspan="6">Softlayer 虚拟服务器命令</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} VLAN 命令

  <table summary="按字母顺序列出的常规 Softlayer 命令（命令具有可获取命令更多信息的链接）">
<caption>表 12. Softlayer VLAN 命令</caption>
 <thead>
 <th colspan="6">Softlayer VLAN 命令</th>
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

### 命令用法
要查看命令的帮助信息，请运行：`bluemix sl [command] -h`。

### bluemix sl init
{: #sl_init}

初始化用于连接到 SoftLayer 环境的配置设置。该配置包括用户名、API 密钥或密码、帐户和端点。
```
bluemix sl init [OPTIONS]
```

<strong>命令选项</strong>：
<dl>
<dt>-a, --api-endpoint</dt>
<dd>Softlayer API 端点 URL，缺省值为 https://api.softlayer.com/rest/v3.1（对于 Softlayer API 密钥认证）或 https://api.softlayer.com/mobile/v3.1（对于 IBM 标识认证）。</dd>
<dt>-u, --sl-user</dt>
<dd>Softlayer 用户名。</dd>
<dt>-p, --sl-password</dt>
<dd>Softlayer 密码或 API 密钥。</dd>
<dt>-c, --account-id</dt>
<dd>Softlayer 帐户标识。</dd>
<dt>-q, --security-question-id</dt>
<dd>用于认证的安全问题标识，如果您不知道，请询问您的帐户所有者。</dd>
<dt>-w, --security-question-answer</dt>
<dd>用于认证的安全问题答案，如果您不知道，请询问您的帐户所有者。</dd>
<dt>-s, --security-code</dt>
<dd>启用双重认证时安全供应商生成的安全代码。</dd>
<dt>-v, --security-vendor</dt>
<dd>提供用于认证的安全代码的安全供应商，选项为 VERISIGN、TOTP 或 PHONE_FACTOR。</dd>
<dt>-t, --auth-token</dt>
<dd>启用电话认证时的认证令牌。</dd>
</dl>

例如，使用 Softlayer 用户名和密码/API 密钥登录
```
$ bluemix sl config
选择如何配置 Softlayer 认证：
1. 使用 Softlayer 用户名和密码/API 密钥登录
2. 使用 Bluemix 单点登录
输入大于 >1 的数字
Softlayer API 端点 URL：[https://api.softlayer.com/rest/v3.1]>
用户名：[]> wangjunl@cn.ibm.com
API 密钥或密码：[]> abcd

Softlayer API 端点：    https://api.softlayer.com/rest/v3.1
帐户标识：              278444
用户标识：              wangjunl@cn.ibm.com
API 密钥：              xxxxxxxxxx
```
例如，使用 Bluemix Single-Sign-On 登录 Softlayer
```
$ bx login -a api.ng.bluemix.net -u wangjunl@cn.ibm.com -p xxxxxxx -c 65ce8074c6c62b5
API 端点：api.ng.bluemix.net
正在进行认证...
确定

目标帐户 Wilma's Account (65ce8074c6c62b5)

API 端点：   https://api.ng.bluemix.net (API version: 2.54.0)
区域：       us-south
用户：       wangjunl@cn.ibm.com
帐户：       Wilma's Account (65ce8074c6c62b5)
没有目标组织或空间，请使用“bx target --cf or bx target -o ORG -s SPACE”

提示：在 Bluemix CLI 上下文中，使用“bx cf <command>”来运行 Cloud Foundry CLI。
```

$ bx sl init
选择如何配置 Softlayer 认证： 
1. 使用 Softlayer 用户名和密码/API 密钥登录
2. 使用 Bluemix 单点登录
输入大于 >2 的数字
Softlayer API 端点 URL：[https://api.softlayer.com/mobile/v3.1]>
将帐户设置为：278444
确定


                              
Softlayer API 端点：   https://api.softlayer.com/mobile/v3.1   
帐户标识：                278444   
用户标识：                12345678   
IMS 令牌：                xxxxxxxxxx
```

### bluemix sl help
{: #sl_help}

查看所有命令的帮助信息以操作 Softlayer 环境。
```
bluemix sl help

```

### bluemix sl block access-authorize
{: #sl_block_access_authorize}

授权主机访问给定卷。
```
bluemix sl block access-authorize VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --hardware-id</dt>
<dd>要授权的一个硬件服务器的标识。</dd>
<dt>-v, --virtual-id</dt>
<dd>要授权的一个虚拟服务器的标识。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要授权的一个 IP 地址的标识。</dd>
<dt>-p, --ip-address</dt>
<dd>要授权的 IP 地址。</dd>
</dl>

**示例**：
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
此命令授权标识为 87654321 的虚拟服务器访问标识为 12345678 的卷。

### bluemix sl block access-list
{: #sl_block_access_list}

列出 ACL。
```
bluemix sl block access-list VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、name、type、private_ip_address、host_iqn、username 或 password。</dd>
<dt>--columns</dt>
<dd>要显示的列，选项为：id、name、type、private_ip_address、host_iqn、username 或 password。</dd>
</dl>

**示例**：
```
bluemix sl block access-list 12345678 --sortby id
```
此命令列出有权访问标识为 12345678 的卷的所有主机，并按标识对其排序。

### bluemix sl block access-revoke
{: #sl_block_access_revoke}

撤销主机访问给定卷的授权。
```
 bluemix sl block access-revoke VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --hardware-id</dt>
<dd>要撤销的一个硬件服务器的标识。</dd>
<dt>-v, --virtual-id</dt>
<dd>要撤销的一个虚拟服务器的标识。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要撤销的一个 IP 地址的标识。</dd>
<dt>-p, --ip-address</dt>
<dd>要撤销的 IP 地址。</dd>
</dl>

**示例**：
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
此命令撤销标识为 87654321 的虚拟服务器对标识为 12345678 的卷的访问权。

### bluemix sl block replica-failback
{: #sl_block_replica_failback}

从副本对块卷执行故障恢复操作。
```
 bluemix sl block replica-failback VOLUME_ID
```


**示例**：
```
 bluemix sl block replica-failback 12345678
```
此命令对标识为 12345678 的卷执行故障恢复操作。

### bluemix sl block replica-failover
{: #sl_block_replica_failover}

从块卷故障转移到给定的副本卷。
```
bluemix sl block replica-failover VOLUME_ID REPLICA_ID
```


**示例**：
```
 bluemix sl block replica-failover 12345678 87654321
```
此命令对标识为 12345678 的卷执行到标识为 87654321 的副本卷的故障转移操作。

### bluemix sl block replica-locations
{: #sl_block_replica_locations}

列出给定卷的适用复制数据中心。
```
bluemix sl block replica-locations VOLUME_ID
```


**示例**：
```
bluemix sl block replica-locations 12345678
```
此命令列出标识为 12345678 的块卷的适用复制数据中心。

### bluemix sl block replica-order
{: #sl_block_replica_order}

订购块存储器副本卷。
```
 bluemix sl block replica-order VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --snapshot-schedule</dt>
<dd>必需。针对复制的快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
<dt>-d, --datacenter</dt>
<dd>必需。副本的数据中心的短名称，例如 dal09。</dd>
<dt>-t, --tier</dt>
<dd>可选。为其订购副本的主卷的耐久性存储器层 (IOPS/GB)，选项为：0.25、2、4 或 10；如果未指定任何层，那么将使用原始卷的层。</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数；如果未指定 IOPS，那么将使用原始卷的 IOPS。</dd>
<dt>-o, --os-type</dt>
<dd>可选。为其订购副本的主卷的操作系统类型，选项为：HYPER_V、LINUX、VMWARE、WINDOWS_2008、WINDOWS_GPT、WINDOWS 或 XEN。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
此命令为标识为 12345678 的卷订购副本，此副本执行 DAILY 复制，位于 dal09，层级为 4，操作系统类型为 Linux。

### bluemix sl block replica-partners
{: #sl_block_replica_partners}

列出块卷的现有复制卷。
```
bluemix sl block replica-partners VOLUME_ID [OPTIONS]
```


**示例**：
```
bluemix sl block replica-partners 12345678
```
此命令列出标识为 12345678 的块卷的现有复制卷。

### bluemix sl block snapshot-cancel
{: #sl_block_snapshot_cancel}

取消给定卷的现有快照空间。
```
 bluemix sl block snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--reason</dt>
<dd>可选的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消快照空间，而不是在计费周年取消。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl block snapshot-cancel 12345678 --immediate -f
```
此命令立即取消标识为 12345678 的快照，而不要求确认。

### bluemix sl block snapshot-create
{: #sl_block_snapshot_create}

创建给定卷的快照。
```
 bluemix sl block snapshot-create VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-n, --note</dt>
<dd>要对新快照设置的注释。</dd>
</dl>

**示例**：
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
此命令创建标识为 12345678 的卷的快照，并添加注释 snapshotforbluemix。

### bluemix sl block snapshot-disable
{: #sl_block_snapshot_disable}

禁止按指定安排生成给定卷的快照。
```
 bluemix sl block snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --schedule-type</dt>
<dd>必需。快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
</dl>

**示例**：
```
 bluemix sl block snapshot-disable 12345678 -s DAILY
```
此命令禁止为标识为 12345678 的卷生成每日快照。

### bluemix sl block snapshot-enable
{: #sl_block_snapshot_enable}

允许按指定安排生成给定卷的快照。
```
 bluemix sl block snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --schedule-type</dt>
<dd>必需。快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
<dt>-c, --retention-count</dt>
<dd>必需。要保留的快照数。</dd>
<dt>-m, --minute</dt>
<dd>应生成快照的时刻（分钟，0 到 59 之间的整数）。</dd>
<dt>-r, --hour</dt>
<dd>应生成快照的时刻（小时，0 到 23 之间的整数）。</dd>
<dt>-d, --day-of-week</dt>
<dd>应生成快照的日期（星期，0 到 6 之间的整数）。0 表示周日，1 表示周一，2 表示周二，3 表示周三，4 表示周四，5 表示周五，6 表示周六。</dd>
</dl>

**示例**：
```
 bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
此命令允许为标识为 12345678 的卷生成快照。快照将在每周日 2:00 生成，最多保留 5 个快照。

### bluemix sl block snapshot-delete
{: #sl_block_snapshot_delete}

删除给定卷的快照。
```
  bluemix sl block snapshot-delete SNAPSHOT_ID
```


**示例**：
```
 bluemix sl block snapshot-delete 12345678
```
此命令删除标识为 12345678 的快照。

### bluemix sl block snapshot-list
{: #sl_block_snapshot_list}

列出块存储器快照。
```
 bluemix sl block snapshot-list VOLUME_ID [OPTIONS]

```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、name、created 或 size_bytes。</dd>
</dl>

**示例**：
```
 bluemix sl block snapshot-list 12345678 --sortby id
```
此命令列出标识为 12345678 的卷的所有快照，并按标识对其排序。

### bluemix sl block snapshot-order
{: #sl_block_snapshot_order}

为块存储卷订购快照空间。
```
 bluemix sl block snapshot-order VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --size</dt>
<dd>必需。要创建的快照空间的大小（以 GB 为单位）。</dd>
<dt>-t, --tier</dt>
<dd>可选。为其订购空间的块卷的耐久性存储器层 (IOPS/GB)，选项为：0.25、2、4 或 10。</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数。</dd>
<dt>-u, --upgrade</dt>
<dd>指示订单是升级的标志。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
   bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
此命令为标识为 12345678 的卷订购快照空间，大小为 1000 GB，层级为 4 IOPS/GB。

### bluemix sl block snapshot-restore
{: #sl_block_snapshot_restore}

使用给定快照复原块卷。
```
 bluemix sl block snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**示例**：
```
 bluemix sl block snapshot-restore 12345678 87654321
```
此命令通过标识为 87654321 的快照复原标识为 12345678 的卷。

### bluemix sl block volume-cancel
{: #sl_block_volume_cancel}

取消现有块存储卷。
```
 bluemix sl block volume-cancel VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--reason</dt>
<dd>可选的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消块存储卷，而不是在计费周年取消。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl block volume-cancel 12345678 --immediate -f
```
此命令立即取消标识为 12345678 的卷，而不要求确认。

### bluemix sl block volume-list
{: #sl_block_volume_list}

列出块存储器。
```
 bluemix sl block volume-list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-u, --username</dt>
<dd>按卷用户名过滤。</dd>
<dt>-d, --datacenter</dt>
<dd>按数据中心短名称过滤。</dd>
<dt>-t, --storage-type</dt>
<dd>按存储卷类型过滤，选项为：performance 或 endurance。</dd>
<dt>-o, --order</dt>
<dd>按购买了块存储器的订单的标识过滤。</dd>
<dt>--sortby</dt>
<dd>要按其排序的列，选项为：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、active_transactions 或 created_by。</dd>
<dt>--columns</dt>
<dd>要显示的列，选项为：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr 或 created_by。</dd>
</dl>

**示例**：
```
 bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
此命令列出当前帐户中位于 dal09 的所有耐久性卷，并按容量对其排序。


### bluemix sl block volume-detail
{: #sl_block_volume_detail}

显示指定卷的详细信息。
```
 bluemix sl block volume-detail VOLUME_ID
```


**示例**：
```
 bluemix sl block volume-detail 12345678
```
此命令显示标识为 12345678 的卷的详细信息。

### bluemix sl block volume-duplicate
{: #sl_block_volume_duplicate}

通过复制现有卷来订购块卷。
```
bluemix sl block volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>用于复制的源卷快照的标识。</dd>
<dt>-s, --duplicate-size</dt>
<dd>复制块卷的大小（以 GB 为单位），如果未指定大小，那么将使用原始卷的大小。</dd>
<dt>-i, --duplicate-iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数；如果未指定 IOPS，那么将使用原始卷的 IOPS。</dd>
<dt>-t, --duplicate-tier</dt>
<dd>耐久性存储器层，如果未指定层，那么将使用原始卷的层。</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>订购用于复制的快照空间的大小，如果未指定快照空间大小，那么将使用源卷的快照空间大小。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl block volume-duplicate 12345678
```
此命令显示通过复制标识为 12345678 的卷来订购新卷。

### bluemix sl block volume-order
{: #sl_block_volume_order}

订购块存储卷。
```
   bluemix sl block volume-order [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-t, --storage-type</dt>
<dd>必需。存储卷的类型，选项为：performance 或 endurance。</dd>
<dt>-s, --size</dt>
<dd>必需。存储卷大小 (GB)</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数 [storage-type 为 performance 时是必需的]。</dd>
<dt>-e, --tier</dt>
<dd>耐久性存储器层 (IOP/GB) [storage-type 为 endurance 时是必需的]，选项为：0.25、2、4 或 10。</dd>
<dt>-o, --os-type</dt>
<dd>必需。操作系统，选项为：HYPER_V、LINUX、VMWARE、WINDOWS_2008、WINDOWS_GPT、WINDOWS 和 XEN。</dd>
<dt>-d, --datacenter</dt>
<dd>必需。数据中心短名称。</dd>
<dt>-n, --snapshot-size</dt>
<dd>用于随耐久性块存储器一起订购快照空间的可选参数；指定要订购的快照空间大小（以 GB 为单位）。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
此命令订购性能卷，大小为 1000 GB，IOPS 为 4000，操作系统类型为 LINUX，位于 dal09。
### bluemix sl block volume-options
{: #sl_block_volume_options}

列出用于订购块存储器的所有选项。
```
 bluemix sl block volume-options
```


**示例**：
```
 bluemix sl block volume-options
```
此命令列出用于创建块存储卷的所有选项，包括存储器类型、卷大小、操作系统类型、IOPS、层级、数据中心和快照大小。


### bluemix sl cdn cancel
{: #sl_cdn_cancel}

取消 CDN 帐户。
```
bluemix sl cdn cancel ACCOUNT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>
### bluemix sl cdn detail
{: #sl_cdn_detail}

CDN 帐户的详细信息。
```
bluemix sl cdn detail ACCOUNT_ID
```

### bluemix sl cdn list
{: #sl_cdn_list}

列出所有 CDN 帐户。
```
bluemix sl cdn list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、name、type 或 created。</dd>
<dt>--order</dt>
<dd>按订单标识过滤。</dd>
</dl>
### bluemix sl cdn load
{: #sl_cdn_load}

在所有边缘节点上高速缓存一个或多个文件。
```
bluemix sl cdn load ACCOUNT_ID CONTENT_URL [CONTENT_URL...]
```

### bluemix sl cdn order
{: #sl_cdn_order}

订购 CDN 帐户。
```
bluemix sl cdn order [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-b, --bandwidth</dt>
<dd>CDN 带宽，如果未指定，将使用“现买现付”价格。</dd>
<dt>-s, --storage</dt>
<dd>CDN 存储器，如果未指定，将使用“现买现付”价格。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>
### bluemix sl cdn options
{: #sl_cdn_options}

用于订购 CDN 帐户的带宽和存储选项。
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add
{: #sl_cdn_origin_add}

创建源拉取映射。
```
bluemix sl cdn origin-add ACCOUNT_ID CONTENT_URL [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-t, --type</dt>
<dd>此映射的介质类型 (http、flash、wm、...)，缺省值为 http。</dd>
<dt>-c, --cname</dt>
<dd>连接到映射的可选 CNAME。</dd>
</dl>
### bluemix sl cdn origin-list
{: #sl_cdn_origin_list}

列出源拉取映射。
```
bluemix sl cdn origin-list ACCOUNT_ID
```

### bluemix sl cdn origin-remove
{: #sl_cdn_origin_remove}

除去源拉取映射。
```
bluemix sl cdn origin-remove ACCOUNT_ID ORIGIN_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>
### bluemix sl cdn purge
{: #sl_cdn_purge}

清除所有边缘节点中高速缓存的文件。
```
bluemix sl cdn purge ACCOUNT_ID CONTENT_URL [CONTENT_URL...][OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>
### bluemix sl file access-authorize
{: #sl_file_access_authorize}

授权主机访问给定卷。
```
bluemix sl file access-authorize VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --hardware-id</dt>
<dd>要授权的一个硬件服务器的标识。</dd>
<dt>-v, --virtual-id</dt>
<dd>要授权的一个虚拟服务器的标识。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要授权的一个 IP 地址的标识。</dd>
<dt>-p, --ip-address</dt>
<dd>要授权的 IP 地址。</dd>
<dt>-s, --subnet-id</dt>
<dd>要授权的一个子网的标识。</dd>
</dl>

**示例**：
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
此命令授权标识为 87654321 的虚拟服务器访问标识为 12345678 的卷。

### bluemix sl file access-list
{: #sl_file_access_list}

列出 ACL。
```
bluemix sl file access-list VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、name、type、private_ip_address、host_iqn、username 或 password。</dd>
<dt>--columns</dt>
<dd>要显示的列，选项为：id、name、type、private_ip_address、host_iqn、username 或 password。</dd>
</dl>

**示例**：
```
bluemix sl file access-list 12345678 --sortby id
```
此命令列出有权访问标识为 12345678 的卷的所有主机，并按标识对其排序。

### bluemix sl file access-revoke
{: #sl_file_access_revoke}

撤销主机访问给定卷的授权。
```
bluemix sl file access-revoke VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --hardware-id</dt>
<dd>要撤销的一个硬件服务器的标识。</dd>
<dt>-v, --virtual-id</dt>
<dd>要撤销的一个虚拟服务器的标识。</dd>
<dt>-i, --ip-address-id</dt>
<dd>要撤销的一个 IP 地址的标识。</dd>
<dt>-p, --ip-address</dt>
<dd>要撤销的 IP 地址。</dd>
<dt>-s, --subnet-id</dt>
<dd>要撤销的一个子网的标识。</dd>
</dl>

**示例**：
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
此命令撤销标识为 87654321 的虚拟服务器对标识为 12345678 的卷的访问权。

### bluemix sl file replica-failback
{: #sl_file_replica_failback}

从副本对文件卷执行故障恢复操作。
```
bluemix sl file replica-failback VOLUME_ID
```


**示例**：
```
bluemix sl file replica-failback 12345678
```
此命令对标识为 12345678 的卷执行故障恢复操作。

### bluemix sl file replica-failover
{: #sl_file_replica_failover}

从文件卷故障转移到给定的副本卷。
```
bluemix sl file replica-failover VOLUME_ID REPLICA_ID
```


**示例**：
```
bluemix sl file replica-failover 12345678 87654321
```
此命令对标识为 12345678 的卷执行到标识为 87654321 的副本卷的故障转移操作。

### bluemix sl file replica-locations
{: #sl_file_replica_locations}

列出给定卷的适用复制数据中心。
```
bluemix sl file replica-locations VOLUME_ID
```


**示例**：
```
bluemix sl file replica-locations 12345678
```
此命令列出标识为 12345678 的文件卷的适用复制数据中心。

### bluemix sl file replica-order
{: #sl_file_replica_order}

订购文件存储器副本卷。
```
bluemix sl file replica-order VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --snapshot-schedule</dt>
<dd>必需。用于复制的快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
<dt>-d, --datacenter</dt>
<dd>必需。副本的数据中心的短名称，例如 dal09。</dd>
<dt>-t, --tier</dt>
<dd>可选。为其订购副本的主卷的耐久性存储器层 (IOPS/GB)，选项为：0.25、2、4 或 10；如果未指定任何层，那么将使用原始卷的层。</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数；如果未指定 IOPS，那么将使用原始卷的 IOPS。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
此命令为标识为 12345678 的卷订购副本，此副本执行 DAILY 复制，位于 dal09，层级为 4。

### bluemix sl file replica-partners
{: #sl_file_replica_partners}

列出文件卷的现有复制卷。
```
bluemix sl file replica-partners VOLUME_ID [OPTIONS]
```


**示例**：
```
bluemix sl file replica-partners 12345678
```
此命令列出标识为 12345678 的文件卷的现有复制卷。

### bluemix sl file snapshot-cancel
{: #sl_file_snapshot_cancel}

取消给定卷的现有快照空间。
```
bluemix sl file snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--reason</dt>
<dd>可选的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消快照空间，而不是在计费周年取消。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
此命令立即取消标识为 12345678 的快照，而不要求确认。

### bluemix sl file snapshot-create
{: #sl_file_snapshot_create}

创建给定卷的快照。
```
bluemix sl file snapshot-create VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-n, --note</dt>
<dd>要对新快照设置的注释。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
此命令创建标识为 12345678 的卷的快照，并添加注释 snapshotforbluemix。

### bluemix sl file snapshot-disable
{: #sl_file_snapshot_disable}

禁止按指定安排生成给定卷的快照。
```
bluemix sl file snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --schedule-type</dt>
<dd>必需。快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
此命令禁止为标识为 12345678 的卷生成每日快照。

### bluemix sl file snapshot-enable
{: #sl_file_snapshot_enable}

允许按指定安排生成给定卷的快照。
```
bluemix sl file snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --schedule-type</dt>
<dd>必需。快照安排，选项为：HOURLY、DAILY 或 WEEKLY。</dd>
<dt>-c, --retention-count</dt>
<dd>必需。要保留的快照数。</dd>
<dt>-m, --minute</dt>
<dd>应生成快照的时刻（分钟，0 到 59 之间的整数）。</dd>
<dt>-r, --hour</dt>
<dd>应生成快照的时刻（小时，0 到 23 之间的整数）。</dd>
<dt>-d, --day-of-week</dt>
<dd>应生成快照的日期（星期，0 到 6 之间的整数）。0 表示周日，1 表示周一，2 表示周二，3 表示周三，4 表示周四，5 表示周五，6 表示周六。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
此命令允许为标识为 12345678 的卷生成快照。快照将在每周日 2:00 生成，最多保留 5 个快照。

### bluemix sl file snapshot-delete
{: #sl_file_snapshot_delete}

删除给定卷的快照。
```
bluemix sl file snapshot-delete SNAPSHOT_ID
```


**示例**：
```
bluemix sl file snapshot-delete 12345678
```
此命令删除标识为 12345678 的快照。

### bluemix sl file snapshot-list
{: #sl_file_snapshot_list}

列出文件存储器快照。
```
bluemix sl file snapshot-list VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、name、created 或 size_bytes。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-list 12345678 --sortby id
```
此命令列出标识为 12345678 的卷的所有快照，并按标识对其排序。

### bluemix sl file snapshot-order
{: #sl_file_snapshot_order}

为文件存储卷订购快照空间。
```
bluemix sl file snapshot-order VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --size</dt>
<dd>必需。要创建的快照空间的大小（以 GB 为单位）。</dd>
<dt>-t, --tier</dt>
<dd>可选。为其订购空间的文件卷的耐久性存储器层 (IOPS/GB)，选项为：0.25、2、4 或 10。</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数。</dd>
<dt>-u, --upgrade</dt>
<dd>指示订单是升级的标志。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
此命令为标识为 12345678 的卷订购快照空间，大小为 1000 GB，层级为 4 IOPS/GB。

### bluemix sl file snapshot-restore
{: #sl_file_snapshot_restore}

使用给定快照复原文件卷。
```
bluemix sl file snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**示例**：
```
bluemix sl file snapshot-restore 12345678 87654321
```
此命令通过标识为 87654321 的快照复原标识为 12345678 的卷。

### bluemix sl file volume-cancel
{: #sl_file_volume_cancel}

取消现有文件存储卷。
```
bluemix sl file volume-cancel VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--reason</dt>
<dd>可选的取消原因。</dd>
<dt>--immediate</dt>
<dd>立即取消文件存储卷，而不是在计费周年取消。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
此命令立即取消标识为 12345678 的卷，而不要求确认。

### bluemix sl file volume-list
{: #sl_file_volume_list}

列出文件存储器。
```
bluemix sl file volume-list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-u, --username</dt>
<dd>按卷用户名过滤。</dd>
<dt>-d, --datacenter</dt>
<dd>按数据中心短名称过滤。</dd>
<dt>-t, --storage-type</dt>
<dd>按存储卷类型过滤，选项为：performance 或 endurance。</dd>
<dt>-o, --order</dt>
<dd>按购买了文件存储器的订单的标识过滤。</dd>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr、active_transactions 或 mount_addr。</dd>
<dt>--columns</dt>
<dd>要显示的列，选项为：id、username、datacenter、storage_type、capacity_gb、bytes_used、ip_addr 或 mount_addr。</dd>
</dl>

**示例**：
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
此命令列出当前帐户中位于 dal09 的所有耐久性卷，并按容量对其排序。


### bluemix sl file volume-detail
{: #sl_file_volume_detail}

显示指定卷的详细信息。
```
bluemix sl file volume-detail VOLUME_ID
```


**示例**：
```
bluemix sl file volume-detail 12345678
```
此命令显示标识为 12345678 的卷的详细信息。

### bluemix sl file volume-duplicate
{: #sl_file_volume_duplicate}

通过复制现有卷来订购文件卷。
```
bluemix sl file volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>用于复制的原始卷快照的标识。</dd>
<dt>-s, --duplicate-size</dt>
<dd>复制文件卷的大小（以 GB 为单位），如果未指定大小，那么将使用原始卷的大小。</dd>
<dt>-i, --duplicate-iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数；如果未指定 IOPS，那么将使用原始卷的 IOPS。</dd>
<dt>-t, --duplicate-tier</dt>
<dd>耐久性存储器层，如果未指定层，那么将使用原始卷的层。</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>订购用于复制的快照空间的大小，如果未指定快照空间大小，那么将使用原始卷的快照空间大小。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file volume-duplicate 12345678
```
此命令显示通过复制标识为 12345678 的卷来订购新卷。

### bluemix sl file volume-order
{: #sl_file_volume_order}

订购文件存储卷。
```
bluemix sl file volume-order [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-t, --storage-type</dt>
<dd>必需。存储卷的类型，选项为：performance 或 endurance。</dd>
<dt>-s, --size</dt>
<dd>必需。存储卷大小 (GB)</dd>
<dt>-i, --iops</dt>
<dd>性能存储器 IOPS，介于 100 到 6000 之间，是 100 的倍数 [storage-type 为 performance 时是必需的]。</dd>
<dt>-e, --tier</dt>
<dd>耐久性存储器层 (IOP/GB) [storage-type 为 endurance 时是必需的]，选项为：0.25、2、4 或 10。</dd>
<dt>-d, --datacenter</dt>
<dd>必需。数据中心短名称。</dd>
<dt>-n, --snapshot-size</dt>
<dd>用于订购快照空间和卷的可选参数。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
此命令订购性能卷，大小为 1000 GB，IOPS 为 4000，位于 dal09。

### bluemix sl file volume-options
{: #sl_file_volume_options}

列出用于订购文件存储器的所有选项。
```
bluemix sl file volume-options
```


**示例**：
```
bluemix sl file volume-options
```
此命令列出用于创建文件存储卷的所有选项，包括存储器类型、卷大小、IOPS、层级、数据中心和快照大小。

### bluemix sl dns import
{: #sl_dns_import}

导入基于 BIND 区域文件的区域。
```
bluemix sl dns import ZONEFILE [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--dry-run</dt>
<dd>实际不创建记录。</dd>
</dl>

**示例**：
```
 bluemix sl dns import ~/blumix.net.txt
```
此命令从 ~/blumix.net.txt 文件导入区域及其资源记录。

### bluemix sl dns record-add
{: #sl_dns_record_add}

在区域中添加资源记录。
```
bluemix sl dns record-add ZONE RECORD TYPE DATA [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--ttl</dt>
<dd>TTL（生存时间）（以秒为单位），例如：86400，缺省值为 7200。</dd>
</dl>

**示例**：
```
 bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
此命令将 A 记录添加到区域 bluemix.net，其主机为“ftp”，数据为“127.0.0.1”，ttl 为 86400 秒。

### bluemix sl dns record-edit
{: #sl_dns_record_edit}

更新区域中的资源记录。
```
   bluemix sl dns record-edit ZONE [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--by-record</dt>
<dd>按主机记录（例如 www）编辑。</dd>
<dt>--by-id</dt>
<dd>按标识编辑单个记录。</dd>
<dt>--data</dt>
<dd>记录数据，例如 IP 地址。</dd>
<dt>--ttl</dt>
<dd>TTL 值（以秒为单位），例如：86400。</dd>
</dl>

**示例**：
```
 bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
此命令编辑区域 bluemix.net 下标识为 12345678 的记录，并将其数据设置为“127.0.0.2”，ttl 设置为 3600。

### bluemix sl dns record-list
{: #sl_dns_record_list}

列出区域中的所有资源记录。
```
   bluemix sl dns record-list ZONE [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--data</dt>
<dd>按记录数据（例如，IP 地址）过滤。</dd>
<dt>--record</dt>
<dd>按主机记录（例如 www）过滤。</dd>
<dt>--ttl</dt>
<dd>按 TTL 值（以秒为单位，例如 86400）过滤。</dd>
<dt>--type</dt>
<dd>按记录类型（例如，A 或 CNAME）过滤。</dd>
</dl>

**示例**：
```
 bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
此命令列出区域 bluemix.net 下的所有 A 记录，依据其过滤的主机为 elasticsearch，ttl 为 900 秒。

### bluemix sl dns record-remove
{: #sl_dns_record_remove}

从区域中除去资源记录。
```
 bluemix sl dns record-remove RECORD_ID
```


**示例**：
```
 bluemix sl dns record-remove 12345678
```
此命令除去标识为 12345678 的资源记录。

### bluemix sl dns zone-create
{: #sl_dns_zone_create}

创建区域。
```
 bluemix sl dns zone-create ZONE
```


**示例**：
```
 bluemix sl dns zone-create bluemix.net
```
此命令创建名为 bluemix.net 的区域。

### bluemix sl dns zone-delete
{: #sl_dns_zone_delete}

删除区域。
```
 bluemix sl dns zone-delete ZONE
```


**示例**：
```
 bluemix sl dns zone-delete bluemix.net
```
此命令删除名为 bluemix.net 的区域。

### bluemix sl dns zone-list
{: #sl_dns_zone_list}

列出帐户的所有区域。
```
   bluemix sl dns zone-list
```


**示例**：
```
   bluemix sl dns zone-list
```
此命令列出当前帐户下的所有区域。

### bluemix sl dns zone-print
{: #sl_dns_zone_print}

以 BIND 格式打印区域和资源记录。
```
 bluemix sl dns zone-print ZONE
```


**示例**：
```
 bluemix sl dns zone-print bluemix.net
```
此命令以 BIND 格式显示名为 bluemix.net 的区域。


### bluemix sl globalip create
{: #sl_globalip_create}

创建全局 IP。
```
bluemix sl globalip create [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--v6</dt>
<dd>订购 IPv6 IP 地址。</dd>
<dt>--test</dt>
<dd>测试订单。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
     bluemix sl globalip create --v6
```
此命令创建 IP V6 地址。

### bluemix sl globalip assign
{: #sl_globalip_assign}

为目标路由器或设备分配全局 IP。
```
bluemix sl globalip assign IDENTIFIER TARGET
```


**示例**：
```
 bluemix sl globalip assign 12345678 9.111.123.456
```
此命令将标识为 12345678 的 IP 地址分配给 IP 地址为 9.111.123.456 的目标设备。


### bluemix sl globalip cancel
{: #sl_globalip_cancel}

取消全局 IP。
```
bluemix sl globalip cancel IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl globalip cancel 12345678
```
此命令取消标识为 12345678 的 IP 地址。

### bluemix sl globalip list
{: #sl_globalip_list}

列出帐户的所有全局 IP。
```
bluemix sl globalip list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--v4</dt>
<dd>仅显示 IPv4 IP。</dd>
<dt>--v6</dt>
<dd>仅显示 IPv6 IP。</dd>
<dt>--order</dt>
<dd>按购买此 IP 地址的订单的标识过滤。</dd>
</dl>

**示例**：
```
bluemix sl globalip list --v4
```
此命令列出当前帐户的所有 IP V4 地址。

### bluemix sl globalip unassign
{: #sl_globalip_unassign}

从目标路由器或设备取消分配全局 IP。
```
 bluemix sl globalip unassign IDENTIFIER
```


**示例**：
```
 bluemix sl globalip unassign 12345678
```
此命令从目标设备取消分配标识为 12345678 的 IP 地址。

### bluemix sl image delete
{: #sl_image_delete}

删除映像。
```
   bluemix sl image delete IDENTIFIER
```
**示例**：
```
   bluemix sl image delete 12345678
```
此命令删除标识为 `12345678` 的映像。

### bluemix sl image detail
{: #sl_image_detail}

获取映像的详细信息。
```
 bluemix sl image detail IDENTIFIER
```
**示例**：
```
 bluemix sl image detail 12345678
```
此命令获取标识为 12345678 的映像的详细信息。

### bluemix sl image edit
{: #sl_image_edit}

编辑映像的详细信息。
```
   bluemix sl image edit IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--name</dt>
<dd>映像的名称。</dd>
<dt>--note</dt>
<dd>映像的其他注释。</dd>
<dt>--tag</dt>
<dd>映像的标记。</dd>
</dl>

*示例**：
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
此命令编辑标识为 `12345678` 的映像，并将其名称设置为 `ubuntu16`，注释设置为 `testing`，标记设置为 `staging`。

### bluemix sl image list
{: #sl_image_list}

列出帐户的所有映像。
```
   bluemix sl image list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--name</dt>
<dd>过滤映像名称。</dd>
<dt>--public</dt>
<dd>仅显示公用映像。</dd>
<dt>--private</dt>
<dd>仅显示专用映像。</dd>
</dl>

### bluemix sl ipsec cancel
{: #sl_ipsec_cancel}

取消 IPSec VPN 隧道上下文。
```
bluemix sl ipsec cancel CONTEXT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--immediate</dt>
<dd>立即取消 IPSec，而不是在计费周年取消。</dd>
<dt>--reason</dt>
<dd>可选的取消原因。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl ipsec config
{: #sl_ipsec_config}

请求隧道上下文的配置。
```
bluemix sl ipsec config CONTEXT_ID [OPTIONS]
```

### bluemix sl ipsec detail
{: #sl_ipsec_detail}

列出 IPSec VPN 隧道上下文详细信息。
```
bluemix sl ipsec detail CONTEXT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-i, --include</dt>
<dd>包含其他资源，选项为：at、is、rs、sr 或 ss。</dd>
</dl>
### bluemix sl ipsec list
{: #sl_ipsec_list}

列出 IPSec VPN 隧道上下文。
```
bluemix sl ipsec list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--order</dt>
<dd>按购买了 IPSec 的订单的标识过滤。</dd>
</dl>
### bluemix sl ipsec order
{: #sl_ipsec_order}

订购 IPSec VPN 隧道。
```
bluemix sl ipsec order [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --datacenter</dt>
<dd>必需。IPSec 的数据中心的短名称，例如 dal09。</dd>
</dl>

### bluemix sl ipsec subnet-add
{: #sl_ipsec_subnet_add}

向 IPSec 隧道上下文添加子网。
```
bluemix sl ipsec subnet-add CONTEXT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --subnet-id</dt>
<dd>要添加的子网标识（必需）。</dd>
<dt>-t, --subnet-type</dt>
<dd>要添加的子网类型（必需），选项为：internal、remote 或 service。</dd>
<dt>-n, --network</dt>
<dd>要创建的子网标识。</dd>
</dl>

### bluemix sl ipsec subnet-remove
{: #sl_ipsec_subnet_remove}

从 IPSec 隧道上下文中除去子网。
```
bluemix sl ipsec subnet-remove CONTEXT_ID SUBNET_ID SUBNET_TYPE [OPTIONS]
```

### bluemix sl ipsec translation-add
{: #sl_ipsec_translation_add}

向 IPSec 隧道添加地址转换。
```
bluemix sl ipsec translation-add CONTEXT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --static-ip</dt>
<dd>静态 IP 地址（必需）。</dd>
<dt>-r, --remote-ip</dt>
<dd>远程 IP 地址（必需）。</dd>
<dt>-n, --note</dt>
<dd>注释。</dd>
</dl>
### bluemix sl ipsec translation-remove
{: #sl_ipsec_translation_remove}

从 IPSec 中除去转换条目。
```
bluemix sl ipsec translation-remove CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

### bluemix sl ipsec translation-update
{: #sl_ipsec_translation_update}

更新 IPSec 的地址转换。
```
bluemix sl ipsec translation-update CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-s, --static-ip</dt>
<dd>静态 IP 地址（必需）。</dd>
<dt>-r, --remote-ip</dt>
<dd>远程 IP 地址（必需）。</dd>
<dt>-n, --note</dt>
<dd>注释。</dd>
</dl>
### bluemix sl ipsec update
{: #sl_ipsec_update}

更新隧道上下文属性。
```
bluemix sl ipsec update CONTEXT_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-n, --name</dt>
<dd>友好名称。</dd>
<dt>-r, --remote-peer</dt>
<dd>远程同级 IP 地址。</dd>
<dt>-k, --preshared-key</dt>
<dd>预共享密钥。</dd>
<dt>-a, --phase1-auth</dt>
<dd>第 1 阶段认证，选项为：MD5、SHA1 或 SHA256。</dd>
<dt>-c, --phase1-crypto</dt>
<dd>第 1 阶段加密，选项为：DES、3DES、AES128、AES192 或 AES256。</dd>
<dt>-d, --phase1-dh</dt>
<dd>第 1 阶段 Diffie-Hellman 组，选项为：0、1、2 或 5。</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>第 1 阶段密钥生存期，范围为 120-172800。</dd>
<dt>-u, --phase2-auth</dt>
<dd>第 2 阶段认证，选项为：MD5、SHA1 或 SHA256。</dd>
<dt>-y, --phase2-crypto</dt>
<dd>第 2 阶段加密，选项为：DES、3DES、AES128、AES192 或 AES256。</dd>
<dt>-e, --phase2-dh</dt>
<dd>第 2 阶段 Diffie-Hellman 组，选项为：0、1、2 或 5。</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>第 2 阶段完美前向加密，范围为 0-1。</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>第 2 阶段密钥生存期，范围为 120-172800。</dd>
</dl>

### bluemix sl loadbal cancel
{: #sl_loadbal_cancel}

取消现有负载均衡器。
```
bluemix sl loadbal cancel LOADBAL_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl loadbal create
{: #sl_loadbal_create}

添加负载均衡器（假设通过 create 选项返回标识）。
```
bluemix sl loadbal create PRICE_ID LOCATION [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl loadbal create-options
{: #sl_loadbal_create_options}

获取用于创建负载均衡器的价格选项。
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail
{: #sl_loadbal_detail}

获取负载均衡器的详细信息。
```
bluemix sl loadbal detail LOADBAL_ID
```

### bluemix sl loadbal group-add
{: #sl_loadbal_group_add}

添加新的负载均衡器服务。
```
bluemix sl loadbal group-add LOADBAL_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-a, --allocation</dt>
<dd>必需。已分配的连接百分比。</dd>
<dt>-p, --port</dt>
<dd>必需。端口号。</dd>
<dt>-t, --routing-type</dt>
<dd>必需。路由类型的标识。运行“bluemix sl loadbal routing-types”可查找标识。</dd>
<dt>-m, --routing-method</dt>
<dd>必需。路由方法的标识。运行“luemix sl loadbal routing-methods”可查找标识。</dd>
</dl>

### bluemix sl loadbal group-delete
{: #sl_loadbal_group_delete}

删除现有的负载均衡器服务组。
```
bluemix sl loadbal group-delete GROUP_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl loadbal group-edit
{: #sl_loadbal_group_edit}

编辑现有的负载均衡器服务组。
```
bluemix sl loadbal group-edit LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-a, --allocation</dt>
<dd>更改已分配的连接百分比。</dd>
<dt>-p, --port</dt>
<dd>更改端口号。</dd>
<dt>-t, --routing-type</dt>
<dd>更改路由类型的标识。运行“bluemix sl loadbal routing-types”可查找标识。</dd>
<dt>-m, --routing-method</dt>
<dd>更改路由方法的标识。运行“luemix sl loadbal routing-methods”可查找标识。</dd>
</dl>

### bluemix sl loadbal group-reset
{: #sl_loadbal_group_reset}

重置特定服务组上的连接。
```
bluemix sl loadbal group-reset LOADBAL_ID GROUP_ID
```

### bluemix sl loadbal health-checks
{: #sl_loadbal_health_checks}

列出运行状况检查类型。
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list
{: #sl_loadbal_list}

列出活动负载均衡器。
```
bluemix sl loadbal list
```

<strong>命令选项</strong>：

   <dl>
<dt>-d, --datacenter</dt>
<dd>按数据中心短名称过滤。</dd>
<dt>-o, --order</dt>
<dd>按购买了负载均衡器的订单的标识过滤。</dd>
<dt>-p, --ip-address</dt>
<dd>按 IP 地址过滤。</dd>
</dl>
### bluemix sl loadbal routing-methods
{: #sl_loadbal_routing_methods}

列出路由方法。
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types
{: #sl_loadbal_routing_types}

列出路由类型。
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add
{: #sl_loadbal_service_add}

添加新的负载均衡器服务。
```
bluemix sl loadbal service-add LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--disabled</dt>
<dd>可选。创建服务但禁用此服务，如果未指定，缺省值为已启用。</dd>
<dt>-p, --port</dt>
<dd>必需。服务的端口号。</dd>
<dt>-w, --weight</dt>
<dd>必需。服务的权重。</dd>
<dt>-t, --healthcheck-type</dt>
<dd>必需。运行状况检查类型。</dd>
<dt>-i, --ip-address</dt>
<dd>必需。服务的 IP 地址。</dd>
</dl>

### bluemix sl loadbal service-delete
{: #sl_loadbal_service_delete}

删除现有的负载均衡器服务。
```
bluemix sl loadbal service-delete SERVICE_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl loadbal service-edit
{: #sl_loadbal_service_edit}

编辑服务组的属性。
```
bluemix sl loadbal service-edit LOADBAL_ID SERVICE_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--disabled</dt>
<dd>禁用服务。</dd>
<dt>--enabled</dt>
<dd>启用服务。</dd>
<dt>-p, --port</dt>
<dd>更改服务的端口号。</dd>
<dt>-w, --weight</dt>
<dd>更改服务的权重。</dd>
<dt>-t, --healthcheck-type</dt>
<dd>更改运行状况检查类型。</dd>
<dt>-i, --ip-address</dt>
<dd>更改服务的 IP 地址。</dd>
</dl>

### bluemix sl loadbal service-toggle
{: #sl_loadbal_service_toggle}

切换现有负载均衡器服务的状态。
```
bluemix sl loadbal service-toggle SERVICE_ID
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

### bluemix sl security sshkey-add
{: #sl_security_sshkey_add}

添加新的 SSH 密钥。
```
 bluemix sl security sshkey-add LABEL [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --in-file</dt>
<dd>要为此密钥导入的 id_rsa.pub 文件。</dd>
<dt>-k, --key</dt>
<dd>实际 SSH 密钥。</dd>
<dt>--note</dt>
<dd>将与密钥关联的额外注释。</dd>
</dl>

**示例**：
```
 bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
此命令从 ~/.ssh/id_rsa.pub 文件添加 SSH 密钥，注释为“mykey”。

### bluemix sl security sshkey-edit
{: #sl_security_sshkey_edit}

编辑 SSH 密钥。
```
 bluemix sl security sshkey-edit IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--label</dt>
<dd>密钥的新标签。</dd>
<dt>--note</dt>
<dd>密钥的新注释。</dd>
</dl>

**示例**：
```
 bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
此命令更新标识为 12345678 的 SSH 密钥，并将标签设置为“Bluemix”，注释设置为“testing”。

### bluemix sl security sshkey-list
{: #sl_security_sshkey_list}

列出帐户的 SSH 密钥。
```
 bluemix sl security sshkey-list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、label、fingerprint 或 notes。</dd>
</dl>

**示例**：
```
 bluemix sl security sshkey-list --sortby label
```
此命令列出当前帐户的所有 SSH 密钥，并按标签对其排序。

### bluemix sl security sshkey-print
{: #sl_security_sshkey_print}

将 SSH 密钥输出到屏幕。
```
 bluemix sl security sshkey-print IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --out-file</dt>
<dd>公用 SSH 密钥将写入此文件。</dd>
</dl>

**示例**：
```
 bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
此命令显示标识为 12345678 的 SSH 密钥的标识、标签和注释，并将公用密钥写入 ~/mykey.pub 文件。

### bluemix sl security sshkey-remove
{: #sl_security_sshkey_remove}

永久除去 SSH 密钥。
```
 bluemix sl security sshkey-remove IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl security sshkey-remove 12345678 -f
```
此命令除去标识为 12345678 的 SSH 密钥，而不要求确认。

### bluemix sl security cert-add
{: #sl_security_cert_add}

添加和上传 SSL 证书详细信息。
```
 bluemix sl security cert-add [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--crt</dt>
<dd>证书文件。</dd>
<dt>--csr</dt>
<dd>证书签名请求文件。</dd>
<dt>--icc</dt>
<dd>中间证书文件。</dd>
<dt>--key</dt>
<dd>专用密钥文件。</dd>
<dt>--notes</dt>
<dd>其他注释。</dd>
</dl>

**示例**：
```
 bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key 
```
此命令为域 bluemix.net 添加证书文件 ~/bluemix.net.cert 和专用密钥文件 ~/bluemix.net.key。

### bluemix sl security cert-edit
{: #sl_security_cert_edit}

编辑 SSL 证书。
```
 bluemix sl security cert-edit IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--crt</dt>
<dd>证书文件。</dd>
<dt>--csr</dt>
<dd>证书签名请求文件。</dd>
<dt>--icc</dt>
<dd>中间证书文件。</dd>
<dt>--key</dt>
<dd>专用密钥文件。</dd>
<dt>--notes</dt>
<dd>其他注释。</dd>
</dl>

**示例**：
```
 bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
此命令编辑标识为 12345678 的证书，并使用 ~/bluemix.net.key 文件更新其专用密钥。

### bluemix sl security cert-download
{: #sl_security_cert_download}

下载 SSL 证书和密钥文件。
```
 bluemix sl security cert-download IDENTIFIER
```


**示例**：
```
 bluemix sl security cert-download 12345678
```
此命令将 4 个文件下载到标识为 12345678 的证书所在的当前目录。这 4 个文件为：证书文件、证书签名请求文件、中间证书文件和专用密钥文件。

### bluemix sl security cert-list
{: #sl_security_cert_list}

列出帐户的 SSL 证书。
```
 bluemix sl security cert-list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--status</dt>
<dd>显示具有此状态的证书，缺省值为：all，选项为： all、valid 或 expired。</dd>
<dt>--sortby</dt>
<dd>列排序依据，选项为：id、common_name、days_until_expire 或 notes。</dd>
</dl>

**示例**：
```
 bluemix sl security cert-list --status valid --sortby days_until_expire
```
此命令列出当前帐户的所有有效证书，并按有效天数对其排序。

### bluemix sl security cert-remove
{: #sl_security_cert_remove}

除去 SSL 证书。
```
 bluemix sl security cert-remove IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl security cert-remove 12345678
```
此命令除去标识为 12345678 的证书。

### bluemix sl subnet cancel
{: #sl_subnet_cancel}

取消子网。
```
bluemix sl subnet cancel IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl subnet cancel 12345678 -f
```
此命令取消标识为 12345678 的子网，而不要求确认。

### bluemix sl subnet create
{: #sl_subnet_create}

向帐户添加新的子网。
```
   bluemix sl subnet create NETWORK QUANTITY VLAN_ID [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--v6, --ipv6</dt>
<dd>订购 IPv6 地址。</dd>
<dt>--test</dt>
<dd>不订购子网；只获取报价。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl subnet create public 16 567
```
此命令创建具有 16 个 IP v4 地址的公共子网，并会将其放在标识为 567 的 VLAN 上。


### bluemix sl subnet detail
{: #sl_subnet_detail}

获取子网的详细信息。
```
   bluemix sl subnet detail IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--no-vs</dt>
<dd>隐藏虚拟服务器列表。</dd>
<dt>--no-hardware</dt>
<dd>隐藏硬件列表。</dd>
</dl>

**示例**：
```
 bluemix sl subnet detail 12345678
```
此命令显示有关标识为 12345678 的子网的详细信息，包括虚拟服务器和硬件服务器信息。


### bluemix sl subnet list
{: #sl_subnet_list}

列出帐户的所有子网。
```
   bluemix sl subnet list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>要按其排序的列。选项为：id、identifier、type、network_space、datacenter、vlan_id、IP、hardware 和 vs。</dd>
<dt>-d, --datacenter</dt>
<dd>按数据中心短名称过滤。</dd>
<dt>--identifier</dt>
<dd>按网络标识过滤。</dd>
<dt>-t, --subnet-type</dt>
<dd>按子网类型过滤。</dd>
<dt>--network-space</dt>
<dd>按网络空间过滤。</dd>
<dt>--v4, --ipv4</dt>
<dd>仅显示 IPv4 子网。</dd>
<dt>--v6, --ipv6</dt>
<dd>仅显示 IPv6 子网。</dd>
<dt>--order</dt>
<dd>按购买子网的订单的标识过滤。</dd>
</dl>

**示例**：
```
 bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
此命令列出当前帐户的 IP V4 子网，依据以下条件进行过滤：数据中心为 dal09，子网类型为 PRIMARY，网络空间为 PUBLIC。



### bluemix sl subnet lookup
{: #sl_subnet_lookup}

查找 IP 地址并显示其子网和设备信息。
```
   bluemix sl subnet lookup IP_ADDRESS
```


**示例**：
```
 bluemix sl subnet lookup 9.125.235.255
```
此命令查找地址为 9.125.235.255 的 IP 地址记录，并显示其子网和设备信息。


### bluemix sl vlan create
{: #sl_vlan_create}

创建新的 VLAN。
```
   bluemix sl vlan create [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-t, --vlan-type</dt>
<dd>VLAN 的类型：public 或 private。</dd>
<dt>-r, --router</dt>
<dd>路由器的主机名。</dd>
<dt>-d, --datacenter</dt>
<dd>数据中心的短名称。</dd>
<dt>-s, --size</dt>
<dd>子网的大小，选项为：8（5 个可用 IP）、16（13 个可用 IP）或 32（29 个可用 IP）。</dd>
<dt>-n, --name</dt>
<dd>VLAN 的名称。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
此命令创建公共 VLAN，它位于具有 16 个 IP 地址的数据中心 dal09，名称为 myvlan。
### bluemix sl vlan cancel
{: #sl_vlan_cancel}

取消 VLAN。
```
   bluemix sl vlan cancel IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
   bluemix sl vlan cancel 12345678 -f
```
此命令取消标识为 12345678 的 VLAN，而不要求确认。



### bluemix sl vlan detail
{: #sl_vlan_detail}

获取有关 VLAN 的详细信息。
```
   bluemix sl vlan detail IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--no-vs</dt>
<dd>隐藏虚拟服务器列表。</dd>
<dt>--no-hardware</dt>
<dd>隐藏硬件列表。</dd>
</dl>

**示例**：
```
 bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
此命令显示标识为 12345678 的 VLAN 的详细信息，但不列出虚拟服务器或硬件服务器。



### bluemix sl vlan edit
{: #sl_vlan_edit}

编辑有关 VLAN 的详细信息。
```
   bluemix sl vlan edit IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-n, --name</dt>
<dd>VLAN 的名称。</dd>
</dl>

**示例**：
```
 bluemix sl vlan edit 12345678 -n myvlan-rename
```
此命令更新标识为 12345678 的 VLAN，并将其命名为新名称“myvlan-rename”。


### bluemix sl vlan list
{: #sl_vlan_list}

列出帐户的所有 VLAN。
```
 bluemix sl vlan list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--sortby</dt>
<dd>要按其排序的列，选项为：id、number、name、firewall、datacenter、hardware、virtual_servers 或 public_ips。</dd>
<dt>-d, --datacenter</dt>
<dd>按数据中心短名称过滤。</dd>
<dt>-n, --number</dt>
<dd>按 VLAN 编号过滤。</dd>
<dt>--name</dt>
<dd>按 VLAN 名称过滤。</dd>
<dt>--order</dt>
<dd>按购买了 VLAN 的订单的标识过滤。</dd>
</dl>

**示例**：
```
 bluemix sl vlan list -d dal09 --sortby number
```
此命令列出当前帐户的所有 VLAN，依据其过滤的数据中心为 dal09，并按 VLAN 编号对其排序。




### bluemix sl vlan options
{: #sl_vlan_options}

列出用于创建 VLAN 的所有选项。
```
 bluemix sl vlan options
```


**示例**：
```
 bluemix sl vlan options
```
此命令列出用于创建 VLAN 的所有选项，例如 VLAN 类型、数据中心、子网大小、路由器等。

### bluemix sl vs cancel
{: #sl_vs_cancel}

取消虚拟服务器实例。
```
   bluemix sl vs cancel IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs cancel 12345678
```
此命令取消标识为 12345678 的虚拟服务器实例。


### bluemix sl vs capture
{: #sl_vs_capture}

将虚拟服务器实例捕获到映像中。
```
 bluemix sl vs capture IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-n, --name</dt>
<dd>必需。映像的名称。</dd>
<dt>--all</dt>
<dd>捕获属于 VS 的所有磁盘。</dd>
<dt>--note</dt>
<dd>添加要与映像关联的注释。</dd>
</dl>

**示例**：
```
 bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
此命令将标识为 12345678 的虚拟服务器实例中的所有磁盘捕获到映像“mybluemix”中，注释为“testing”。



### bluemix sl vs create
{: #sl_vs_create}

创建虚拟服务器实例。
```
   bluemix sl vs create [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-H, --hostname</dt>
<dd>必需。FQDN 的主机部分。</dd>
<dt>-D, --domain</dt>
<dd>必需。FQDN 的域部分。</dd>
<dt>-c, --cpu</dt>
<dd>必需。CPU 核心数。</dd>
<dt>-m, --memory</dt>
<dd>必需。内存（以兆字节为单位）。</dd>
<dt>-d, --datacenter</dt>
<dd>必需。数据中心短名称。</dd>
<dt>-o, --os</dt>
<dd>操作系统安装代码。提示：可以指定 <OS>_LATEST。</dd>
<dt>--image</dt>
<dd>映像标识。请参阅“bluemix sl image list”以获取参考信息。</dd>
<dt>--billing</dt>
<dd>计费费率。缺省值为：hourly。选项为：hourly 或 monthly。</dd>
<dt>--dedicated</dt>
<dd>创建专用虚拟服务器（专用节点）。</dd>
<dt>--san</dt>
<dd>使用 SAN 存储器（而非本地磁盘）。</dd>
<dt>--test</dt>
<dd>实际不创建虚拟服务器。</dd>
<dt>--export</dt>
<dd>将选项导出到模板文件。</dd>
<dt>-i, --postinstall</dt>
<dd>要下载的安装后脚本。</dd>
<dt>-k, --key</dt>
<dd>要添加到 root 用户的 SSH 密钥的标识（允许多次出现）。</dd>
<dt>--disk</dt>
<dd>磁盘大小（允许多次出现）。</dd>
<dt>--private</dt>
<dd>强制虚拟服务器只有权访问专用网络。</dd>
<dt>--like</dt>
<dd>使用现有虚拟服务器中的配置。</dd>
<dt>-n, --network</dt>
<dd>网络端口速度（以 Mbps 为单位）。</dd>
<dt>--tag</dt>
<dd>要添加到实例的标记（允许多次出现）。</dd>
<dt>-t, --template</dt>
<dd>对命令行选项使用缺省值的模板文件。</dd>
<dt>-u, --userdata</dt>
<dd>用户定义的元数据字符串。</dd>
<dt>-F, --userfile</dt>
<dd>从文件中读取用户数据。</dd>
<dt>--vlan-public</dt>
<dd>要将虚拟服务器放到其中的公共 VLAN 的标识。</dd>
<dt>--vlan-private</dt>
<dd>要将虚拟服务器放到其中的专用 VLAN 的标识。</dd>
<dt>--wait</dt>
<dd>等待虚拟服务器完成供应（最长 X 秒）后再返回。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
  bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
此命令订购虚拟服务器实例，其主机名为 myvsi，域为 bluemix.net，4 个 CPU 核心，4096M 内存，位于数据中心 dal10。

### bluemix sl vs options
{: #sl_vs_options}

列出用于创建虚拟服务器实例的选项。
```
   bluemix sl vs options [OPTIONS]
```


**示例**：
```
 bluemix sl vs options
```
此命令列出用于创建虚拟服务器实例的所有选项，例如数据中心、CPU、内存、操作系统、磁盘、网络速度等。

### bluemix sl vs credentials
{: #sl_vs_credentials}

列出虚拟服务器实例凭证。
```
   bluemix sl vs credentials IDENTIFIER [OPTIONS]
```


**示例**：
```
 bluemix sl vs credentials 12345678
```
此命令列出标识为 12345678 的虚拟服务器实例的所有用户名和密码对。

### bluemix sl vs detail
{: #sl_vs_detail}

获取虚拟服务器实例的详细信息。
```
   bluemix sl vs detail IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--passwords</dt>
<dd>显示密码（小心有人在你背后偷看！）.</dd>
<dt>--price</dt>
<dd>显示关联的价格。</dd>
</dl>

**示例**：
```
   bluemix sl vs details 12345678
```
此命令列出有关标识为 12345678 的虚拟服务器实例的详细信息。


### bluemix sl vs dns-sync
{: #sl_vs_dns_sync}

同步虚拟服务器实例的 DNS 记录。
```
   bluemix sl vs dns-sync IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-a, --a-record</dt>
<dd>同步主机的 A 记录。</dd>
<dt>--aaaa-record</dt>
<dd>同步主机的 AAAA 记录。</dd>
<dt>--ptr</dt>
<dd>同步主机的 PTR 记录。</dd>
<dt>--ttl</dt>
<dd>为 A 和/或 PTR 记录设置 TTL，缺省值为：7200。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
此命令将标识为 12345678 的虚拟服务器实例的 A 记录（IP V4 地址）与 DNS 服务器同步，并将此 A 记录的 ttl 设置为 3600。
### bluemix sl vs edit
{: #sl_vs_edit}

编辑虚拟服务器实例的详细信息。
```
   bluemix sl vs edit IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-D, --domain</dt>
<dd>FQDN 的域部分。</dd>
<dt>-H, --hostname</dt>
<dd>FQDN 的主机部分。示例：server。</dd>
<dt>--tag</dt>
<dd>要设置的标记，或使用空字符串表示全部除去。</dd>
<dt>-u, --userdata</dt>
<dd>用户定义的元数据字符串。</dd>
<dt>-F, --userfile</dt>
<dd>从文件中读取用户数据。</dd>
<dt>--public-speed</dt>
<dd>公共端口速度，选项为：0、10、100、1000 或 10000。</dd>
<dt>--private-speed</dt>
<dd>专用端口速度，选项为：0、10、100、1000 或 10000。</dd>
</dl>

**示例**：
```
 bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
此命令更新标识为 12345678 的虚拟服务器实例，并将其域设置为“bluemix.net”，主机名设置为“myapp”，标记设置为“testcli”。

### bluemix sl vs list
{: #sl_vs_list}

列出帐户的虚拟服务器实例。
```
   bluemix sl vs list [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-c, --cpu</dt>
<dd>CPU 核心数。</dd>
<dt>-D, --domain</dt>
<dd>FQDN 的域部分。</dd>
<dt>-d, --datacenter</dt>
<dd>数据中心短名称。</dd>
<dt>-H, --hostname</dt>
<dd>FQDN 的主机部分。</dd>
<dt>-m, --memory</dt>
<dd>内存（以兆字节为单位）。</dd>
<dt>-n, --network</dt>
<dd>网络端口速度（以 Mbps 为单位）。</dd>
<dt>--hourly</dt>
<dd>仅显示每小时实例。</dd>
<dt>--monthly</dt>
<dd>仅显示每月实例。</dd>
<dt>--tag</dt>
<dd>按标记过滤（允许多次出现）。</dd>
<dt>--sortby</dt>
<dd>要按其排序的列，选项为：id、hostname、domain、datacenter、cpu、memory、primary_ip 或 backend_ip。缺省值为：hostname。</dd>
<dt>--columns</dt>
<dd>要显示的列，选项为：guid、primary_ip、backend_ip、datacenter、action、power_state、created_by 或 tags。缺省值为：id、hostname、primary_ip、backend_ip、datacenter 或 action。</dd>
</dl>

**示例**：
```
 bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
此命令列出当前帐户的所有每小时计费的虚拟服务器实例，依据其过滤的域为“bluemix.net”域，并按内存对其排序。



### bluemix sl vs pause
{: #sl_vs_pause}

暂停活动的虚拟服务器实例。
```
   bluemix sl vs pause IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs pause 12345678 -f
```
此命令暂停标识为 12345678 的虚拟服务器实例，而不要求确认。



### bluemix sl vs power-off
{: #sl_vs_power_off}

关闭活动虚拟服务器实例的电源。
```
   bluemix sl vs power-off IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--hard</dt>
<dd>执行硬关闭。</dd>
<dt>--soft</dt>
<dd>执行软关闭。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
   bluemix sl vs power-off 12345678 --soft
```
此命令对标识为 12345678 的虚拟服务器实例执行软电源关闭操作。

### bluemix sl vs power-on
{: #sl_vs_power_on}

打开虚拟服务器实例的电源。
```
 bluemix sl vs power-on IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs power-on 12345678
```
此命令对标识为 12345678 的虚拟服务器实例执行打开电源操作。


### bluemix sl vs ready
{: #sl_vs_ready}

检查虚拟服务器实例是否准备就绪可供使用。
```
 bluemix sl vs ready IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--wait</dt>
<dd>等待虚拟服务器完成供应（最长 X 秒）后再返回。</dd>
</dl>

**示例**：
```
 bluemix sl vs ready 12345678 --wait 30
```
此命令检查标识为 12345678 的虚拟服务器实例的状态以确定其是否准备就绪可持续使用，并且最长等待 30 秒。

### bluemix sl vs reboot
{: #sl_vs_reboot}

重新引导活动的虚拟服务器实例。
```
 bluemix sl vs reboot IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>--hard</dt>
<dd>执行硬重新引导。</dd>
<dt>--soft</dt>
<dd>执行硬重新引导。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs reboot 12345678 --hard
```
此命令对标识为 12345678 的虚拟服务器实例执行硬重新引导。



### bluemix sl vs reload
{: #sl_vs_reload}

在虚拟服务器实例上重新装入操作系统。
```
 bluemix sl vs reload IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-i, --postinstall</dt>
<dd>要下载的安装后脚本。</dd>
<dt>--image</dt>
<dd>映像标识。缺省值为使用当前操作系统。</dd>
<dt>请参阅</dt>
<dd>“bluemix sl image list”以获取参考信息。</dd>
<dt>-k, --key</dt>
<dd>要添加到 root 用户的 SSH 密钥的标识（允许多次出现）。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
   bluemix sl vs reload 12345678
```
此命令为标识为 12345678 的虚拟服务器实例重新装入当前操作系统。
### bluemix sl vs rescue
{: #sl_vs_rescue}

将虚拟服务器实例重新引导到拯救映像。
```
 bluemix sl vs rescue IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs rescue 12345678
```
此命令将标识为 12345678 的虚拟服务器实例重新引导到拯救映像。


### bluemix sl vs resume
{: #sl_vs_resume}

恢复已暂停的虚拟服务器实例。
```
   bluemix sl vs resume IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs resume 12345678
```
此命令恢复标识为 12345678 的虚拟服务器实例。


### bluemix sl vs upgrade
{: #sl_vs_upgrade}

升级虚拟服务器实例。
```
   bluemix sl vs upgrade IDENTIFIER [OPTIONS]
```

<strong>命令选项</strong>：

   <dl>
<dt>-c, --cpu</dt>
<dd>CPU 核心数。</dd>
<dt>--private</dt>
<dd>CPU 核心将位于专用主机服务器上。</dd>
<dt>-m, --memory</dt>
<dd>内存（以兆字节为单位）。</dd>
<dt>--network</dt>
<dd>网络端口速度（以 Mbps 为单位）。</dd>
<dt>-f, --force</dt>
<dd>强制操作而不确认。</dd>
</dl>

**示例**：
```
 bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
此命令升级标识为 12345678 的虚拟服务器实例，并将 CPU 核心数设置为 8，内存设置为 8192M，网络端口速度设置为 1000 Mbps。

