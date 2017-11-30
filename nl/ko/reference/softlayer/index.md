---

copyright:

  years: 2016,2017

lastupdated: "2017-09-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# {{site.data.keyword.BluSoftlayer_notm}} (bluemix sl) 명령
{: #softlayer_cli}

{{site.data.keyword.BluSoftlayer}} 플러그인은 {{site.data.keyword.Bluemix_notm}} CLI에 병합되었습니다. 더 이상 플러그인을 설치할 필요가 없습니다.

{{site.data.keyword.Bluemix_notm}} 명령행 인터페이스(CLI)에서 {{site.data.keyword.BluSoftlayer_notm}} 명령을 사용하여 SoftLayer 서비스를 구성하고 관리하십시오.


시작하려면 IBM {{site.data.keyword.Bluemix_notm}} CLI를 설치하십시오. 세부사항은
[Bluemix CLI ![외부 링크 아이콘](../../../icons/launch-glyph.svg)](http://clis.ng.bluemix.net/ui/home.html){: new_window}를 참조하십시오.

{{site.data.keyword.Bluemix_notm}} 명령의 전체 목록은 [{{site.data.keyword.Bluemix_notm:}} (bx) 명령](docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_cli)을 참조하십시오.


## 일반 {{site.data.keyword.BluSoftlayer_notm}} 명령

다음 명령이 지원됩니다. 사용 가능한 명령의 목록을 보려면 `bluemix sl` 명령을 사용하십시오.

<table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 명령">
<caption>표 1. 일반 Softlayer 명령</caption>
 <thead>
 <th colspan="6">일반 Softlayer 명령</th>
 </thead>
 <tbody>
 <tr>
 <td>[bluemix sl init](/docs/cli/reference/softlayer/index.html#sl_init)</td>
 <td>[bluemix sl help](/docs/cli/reference/softlayer/index.html#sl_help)</td>
   </tbody>
 </table>


## {{site.data.keyword.BluSoftlayer_notm}} 블록 스토리지 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 2. Softlayer 블록 스토리지</caption>
 <thead>
 <th colspan="6">Softlayer 블록 스토리지</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} CDN 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 3. Softlayer CDN</caption>
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

## {{site.data.keyword.BluSoftlayer_notm}} 파일 스토리지 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 4. Softlayer 파일 스토리지</caption>
 <thead>
 <th colspan="6">Softlayer 파일 스토리지</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} DNS 명령

<table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 5. Softlayer DNS 명령</caption>
 <thead>
 <th colspan="6">Softlayer DNS 명령</th>
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

<table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 6. Softlayer 글로벌 IP 명령</caption>
 <thead>
 <th colspan="6">Softlayer 글로벌 IP 명령</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 이미지 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 7. Softlayer 이미지 명령</caption>
 <thead>
 <th colspan="6">Softlayer 이미지 명령</th>
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
 
 ## {{site.data.keyword.BluSoftlayer_notm}} IPSec VPN 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 7. Softlayer IPSec VPN 명령</caption>
 <thead>
 <th colspan="6">Softlayer IPSec VPN 명령</th>
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

 ## {{site.data.keyword.BluSoftlayer_notm}} 로드 밸런서 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 8. Softlayer 로드 밸런서 명령</caption>
 <thead>
 <th colspan="6">Softlayer 로드 밸런서 명령</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 보안 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 9. Softlayer 보안 명령</caption>
 <thead>
 <th colspan="5">Softlayer 보안 명령</th>
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

## {{site.data.keyword.BluSoftlayer_notm}} 서브넷 명령
 
 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 10. Softlayer 서브넷 명령</caption>
 <thead>
 <th colspan="5">Softlayer 서브넷 명령</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} 가상 서버 명령

 <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 11. Softlayer 가상 서버 명령</caption>
 <thead>
 <th colspan="6">Softlayer 가상 서버 명령</th>
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
 
## {{site.data.keyword.BluSoftlayer_notm}} VLAN 명령

  <table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 Softlayer 명령">
<caption>표 12. Softlayer VLAN 명령</caption>
 <thead>
 <th colspan="6">Softlayer VLAN 명령</th>
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

### 명령 사용
명령에 대한 도움말 정보를 보려면 `bluemix sl [command] -h`를 실행하십시오.

### bluemix sl init
{: #sl_init}

Softlayer 환경에 연결하는 데 사용되는 구성 설정을 초기화하십시오. 구성에는 사용자 이름, API 키 또는 비밀번호, 계정 및 엔드포인트가 포함됩니다.
```
bluemix sl init [OPTIONS]
```

<strong>명령 옵션</strong>:
<dl>
<dt>-a, --api-endpoint</dt>
<dd>Softlayer API 엔드포인트 URL. 기본값: https://api.softlayer.com/rest/v3.1(Softlayer API 키 인증의 경우), https://api.softlayer.com/mobile/v3.1(IBM ID 인증의 경우)</dd>
<dt>-u, --sl-user</dt>
<dd>Softlayer 사용자 이름.</dd>
<dt>-p, --sl-password</dt>
<dd>Softlayer 비밀번호 또는 API 키.</dd>
<dt>-c, --account-id</dt>
<dd>Softlayer 계정 ID 입니다.</dd>
<dt>-q, --security-question-id</dt>
<dd>인증에 사용되는 보안 질문 ID. 모르는 경우 계정 소유자에게 문의하십시오.</dd>
<dt>-w, --security-question-answer</dt>
<dd>인증에 사용되는 보안 질문의 대답. 모르는 경우 계정 소유자에게 문의하십시오.</dd>
<dt>-s, --security-code</dt>
<dd>2단계 인증이 사용되는 경우 보안 공급업체에서 생성한 보안 코드.</dd>
<dt>-v, --security-vendor</dt>
<dd>인증을 위해 보안 코드를 제공하는 보안 공급업체. 옵션: VERISIGN,TOTP,PHONE_FACTOR.</dd>
<dt>-t, --auth-token</dt>
<dd>전화 인증이 사용되는 경우 인증 토큰.</dd>
</dl>

예를 들면, Softlayer 사용자 이름 및 비밀번호/API 키로 로그인
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
예를 들면, Bluemix Single-Sign-On을 사용하여 Softlayer 로그인
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

팁: Bluemix CLI 컨텍스트와 함께 Cloud Foundry CLI를 실행하려면 'bx cf <command>'를 사용하십시오.
```

$ bx sl init
Softlayer 인증을 구성하는 방법을 선택하십시오. 
1. Softlayer 사용자 이름 및 비밀번호/API 키로 로그인
2. Use Bluemix Single-Sign-On
Enter a number> 2
Softlayer API endpoint URL: [https://api.softlayer.com/mobile/v3.1]> 
Setting account to: 278444
OK
                              

                              
Softlayer API 엔드포인트:    https://api.softlayer.com/mobile/v3.1   
계정 ID:                278444   
사용자 ID:                   12345678   
IMS 토큰:                 xxxxxxxxxx
```

### bluemix sl help
{: #sl_help}

Softlayer 환경을 조작하기 위한 모든 명령에 대한 도움말 정보를 봅니다.
```
bluemix sl help

```

### bluemix sl block access-authorize
{: #sl_block_access_authorize}

지정된 볼륨에 액세스하도록 호스트에 권한을 부여합니다.
```
bluemix sl block access-authorize VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --hardware-id</dt>
<dd>권한 부여할 하나의 하드웨어 서버의 ID입니다.</dd>
<dt>-v, --virtual-id</dt>
<dd>권한 부여할 하나의 가상 서버의 ID입니다.</dd>
<dt>-i, --ip-address-id</dt>
<dd>권한 부여할 하나의 IP 주소의 ID입니다.</dd>
<dt>-p, --ip-address</dt>
<dd>권한 부여할 IP 주소입니다.</dd>
</dl>

**예제**:
```
bluemix sl block access-authorize 12345678 --virtual-id 87654321
```
이 명령은 ID 87654321인 가상 서버가 ID가 12345678인 볼륨에 액세스하도록 권한을 부여합니다.

### bluemix sl block access-list
{: #sl_block_access_list}

ACL을 나열합니다.
```
bluemix sl block access-list VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>표시할 열. 옵션: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**예제**:
```
bluemix sl block access-list 12345678 --sortby id
```
이 명령은 ID가 12345678인 볼륨에 액세스하도록 권한이 부여된 모든 호스트를 나열하고 ID별로 정렬합니다.

### bluemix sl block access-revoke
{: #sl_block_access_revoke}

지정된 볼륨에 액세스하는 호스트의 권한을 취소합니다.
```
 bluemix sl block access-revoke VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --hardware-id</dt>
<dd>권한을 취소할 하나의 하드웨어 서버 ID.</dd>
<dt>-v, --virtual-id</dt>
<dd>권한을 취소할 하나의 가상 서버 ID.</dd>
<dt>-i, --ip-address-id</dt>
<dd>권한을 취소할 하나의 IP 주소 ID.</dd>
<dt>-p, --ip-address</dt>
<dd>권한을 취소할 하나의 IP 주소.</dd>
</dl>

**예제**:
```
bluemix sl block access-revoke 12345678 --virtual-id 87654321
```
이 명령은 ID 87654321인 가상 서버의 ID가 12345678인 볼륨에 대한 액세스 권한을 취소합니다.

### bluemix sl block replica-failback
{: #sl_block_replica_failback}

복제본에서 블록 볼륨을 장애 복구합니다.
```
 bluemix sl block replica-failback VOLUME_ID
```


**예제**:
```
 bluemix sl block replica-failback 12345678
```
이 명령은 ID가 12345678인 볼륨에 대해 장애 복구 조작을 수행합니다.

### bluemix sl block replica-failover
{: #sl_block_replica_failover}

지정된 복제본 볼륨으로 블록 볼륨을 장애 복구합니다.
```
bluemix sl block replica-failover VOLUME_ID REPLICA_ID
```


**예제**:
```
 bluemix sl block replica-failover 12345678 87654321
```
이 명령은 ID 87654321인 복제본 볼륨에 ID가 12345678인 볼륨에 대한 장애 복구 조작을 수행합니다.

### bluemix sl block replica-locations
{: #sl_block_replica_locations}

지정된 볼륨에 적합한 복제본 데이터 센터를 나열합니다.
```
bluemix sl block replica-locations VOLUME_ID
```


**예제**:
```
bluemix sl block replica-locations 12345678
```
이 명령은 ID가 12345678인 블록 볼륨에 적합한 복제본 데이터 센터를 나열합니다.

### bluemix sl block replica-order
{: #sl_block_replica_order}

블록 스토리지 복제본 볼륨을 주문합니다.
```
 bluemix sl block replica-order VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --snapshot-schedule</dt>
<dd>필수. 복제에 사용할 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>필수. 복제본에 대한 데이터 센터의 짧은 이름(예: dal09).</dd>
<dt>-t, --tier</dt>
<dd>선택사항. 복제본이 주문되는 기본 볼륨의 Endurance 스토리지 계층(GB당 IOPS). 옵션: 0.25,2,4,10. 계층이 지정되지 않은 경우 원본 볼륨의 계층이 사용됩니다.</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP. 지정되지 않은 경우 원본 볼륨의 IOPS가 사용됩니다.</dd>
<dt>-o, --os-type</dt>
<dd>선택사항. 복제본이 주문되는 기본 볼륨의 운영 체제 유형(예: Linux). 옵션: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl block replica-order 12345678 -s DAILY -d dal09 --tier 4 --os-type LINUX
```
이 명령은 ID가 12345678인 볼륨에 대한 복제본(일별 복제를 수행하며, 계층 레벨 4 및 OS 유형 Linux인 dal09에 위치함)을 주문합니다.

### bluemix sl block replica-partners
{: #sl_block_replica_partners}

블록 볼륨의 기존 복제본 볼륨을 나열합니다.
```
bluemix sl block replica-partners VOLUME_ID [OPTIONS]
```


**예제**:
```
bluemix sl block replica-partners 12345678
```
이 명령은 ID가 12345678인 블록 볼륨의 기존 복제본 볼륨을 나열합니다.

### bluemix sl block snapshot-cancel
{: #sl_block_snapshot_cancel}

지정된 볼륨에 대한 기존 스냅샷 영역을 취소합니다.
```
 bluemix sl block snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--reason</dt>
<dd>취소에 대한 선택적 이유입니다.</dd>
<dt>--immediate</dt>
<dd>청구 주기 대신 즉시 스냅샷 영역 취소.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl block snapshot-cancel 12345678 --immediate -f
```
이 명령은 확인을 요청하지 않고 즉시 ID가 12345678인 스냅샷을 취소합니다.

### bluemix sl block snapshot-create
{: #sl_block_snapshot_create}

지정된 볼륨에서 스냅샷을 작성합니다.
```
 bluemix sl block snapshot-create VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-n, --note</dt>
<dd>새 스냅샷에 설정할 참고.</dd>
</dl>

**예제**:
```
bluemix sl block snapshot-create 12345678 --note snapshotforbluemix
```
이 명령은 snapshotforbluemix와 같은 추가 참고와 함께 ID가 12345678인 볼륨에 대한 스냅샷을 작성합니다.

### bluemix sl block snapshot-disable
{: #sl_block_snapshot_disable}

지정된 볼륨에서 지정된 스케줄에 따라 스냅샷을 사용 안함으로 설정합니다.
```
 bluemix sl block snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --schedule-type</dt>
<dd>필수. 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**예제**:
```
 bluemix sl block snapshot-disable 12345678 -s DAILY
```
이 명령은 ID가 12345678인 볼륨에 대한 일별 스냅샷을 사용 안함으로 설정합니다.

### bluemix sl block snapshot-enable
{: #sl_block_snapshot_enable}

지정된 스케줄에 따라 지정된 볼륨의 스냅샷을 사용으로 설정합니다.
```
 bluemix sl block snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --schedule-type</dt>
<dd>필수. 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>필수. 유지할 스냅샷 수입니다.</dd>
<dt>-m, --minute</dt>
<dd>스냅샷을 작성해야 하는 시간(분), 0 - 59 사이의 정수. </dd>
<dt>-r, --hour</dt>
<dd>스냅샷을 작성해야 하는 시간, 0 - 23 사이의 정수. </dd>
<dt>-d, --day-of-week</dt>
<dd>스냅샷을 작성해야 하는 요일, 0 - 6 사이의 정수.
0은 일요일, 1은 월요일, 2는 화요일, 3은 수요일, 4는 목요일, 5는 금요일, 6은 토요일을 의미합니다. </dd>
</dl>

**예제**:
```
 bluemix sl block snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
이 명령은 ID가 12345678인 볼륨의 스냅샷을 사용으로 설정하고, 스냅샷은 매주 일요일 2시에 작성되며 최대 5개의 스냅샷이 유지됩니다.

### bluemix sl block snapshot-delete
{: #sl_block_snapshot_delete}

지정된 볼륨에서 스냅샷을 삭제합니다.
```
  bluemix sl block snapshot-delete SNAPSHOT_ID
```


**예제**:
```
 bluemix sl block snapshot-delete 12345678
```
이 명령은 ID가 12345678인 스냅샷을 삭제합니다.

### bluemix sl block snapshot-list
{: #sl_block_snapshot_list}

블록 스토리지 스냅샷을 나열합니다.
```
 bluemix sl block snapshot-list VOLUME_ID [OPTIONS]

```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,name,created,size_bytes.</dd>
</dl>

**예제**:
```
 bluemix sl block snapshot-list 12345678 --sortby id
```
이 명령은 ID가 12345678인 볼륨의 모든 스냅샷을 나열하고 ID별로 정렬합니다.

### bluemix sl block snapshot-order
{: #sl_block_snapshot_order}

블록 스토리지 볼륨의 스냅샷 영역을 주문합니다.
```
 bluemix sl block snapshot-order VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --size</dt>
<dd>필수. 작성할 스냅샷 영역의 크기(GB).</dd>
<dt>-t, --tier</dt>
<dd>선택사항. 영역이 주문되는 블록 볼륨의 Endurance 스토리지 계층(GB당 IOPS). 옵션: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP.</dd>
<dt>-u, --upgrade</dt>
<dd>업그레이드 주문임을 표시하는 플래그.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
   bluemix sl block snapshot-order 12345678 -s 1000 -t 4
```
이 명령은 ID가 12345678인 볼륨에 대한 스냅샷 영역을 주문합니다. 크기는 1,000GB이고 계층 레벨은 GB당 4IOPS입니다.

### bluemix sl block snapshot-restore
{: #sl_block_snapshot_restore}

지정된 스냅샷을 사용하여 블록 볼륨을 복원합니다.
```
 bluemix sl block snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**예제**:
```
 bluemix sl block snapshot-restore 12345678 87654321
```
이 명령은 ID 87654321인 스냅샷에서 ID가 12345678인 볼륨을 복원합니다.

### bluemix sl block volume-cancel
{: #sl_block_volume_cancel}

기존 블록 스토리지 볼륨을 취소합니다.
```
 bluemix sl block volume-cancel VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--reason</dt>
<dd>취소에 대한 선택적 이유입니다.</dd>
<dt>--immediate</dt>
<dd>청구 주기 대신에 즉시 블록 스토리지 볼륨 취소.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl block volume-cancel 12345678 --immediate -f
```
이 명령은 확인을 요청하지 않고 즉시 ID가 12345678인 볼륨을 취소합니다.

### bluemix sl block volume-list
{: #sl_block_volume_list}

블록 스토리지를 나열합니다.
```
 bluemix sl block volume-list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-u, --username</dt>
<dd>볼륨 사용자 이름별 필터링.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터 짧은 이름별 필터링.</dd>
<dt>-t, --storage-type</dt>
<dd>스토리지 볼륨 유형별 필터링. 옵션: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>블록 스토리지를 구매한 주문 ID별 필터링.</dd>
<dt>--sortby</dt>
<dd>정렬 기준 열, 옵션: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, active_transactions, created_by.</dd>
<dt>--columns</dt>
<dd>표시할 열, 옵션: id, username, datacenter, storage_type, capacity_gb, bytes_used, ip_addr, created_by.</dd>
</dl>

**예제**:
```
 bluemix sl block volume-list -d dal09 -t endurance --sortby capacity_gb
```
이 명령은 dal09에 위치하는 현재 계정의 모든 endurance 볼륨을 나열하고 용량별로 정렬합니다.


### bluemix sl block volume-detail
{: #sl_block_volume_detail}

지정된 볼륨의 세부사항을 표시합니다.
```
 bluemix sl block volume-detail VOLUME_ID
```


**예제**:
```
 bluemix sl block volume-detail 12345678
```
이 명령은 ID가 12345678인 볼륨의 세부사항을 표시합니다.

### bluemix sl block volume-duplicate
{: #sl_block_volume_duplicate}

기존 볼륨을 복제하여 블록 볼륨을 주문합니다.
```
bluemix sl block volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>복제에 사용할 원본 볼륨 스냅샷의 ID.</dd>
<dt>-s, --duplicate-size</dt>
<dd>중복 블록 볼륨의 크기(GB). 크기가 지정되지 않은 경우 원본 볼륨의 크기가 사용됩니다.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOPS. 지정되지 않은 경우 원본 볼륨의 IOPS가 사용됩니다.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Endurance 스토리지 계층. 계층이 지정되지 않은 경우 원본 볼륨의 계층이 사용됩니다.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>복제를 위해 주문할 스냅샷 영역의 크기. 스냅샷 영역 크기가 지정되지 않은 경우 원본 볼륨의 스냅샷 영역 크기가 사용됩니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl block volume-duplicate 12345678
```
이 명령은 ID가 12345678인 볼륨을 복제하여 새 볼륨 주문을 표시합니다.

### bluemix sl block volume-order
{: #sl_block_volume_order}

블록 스토리지 볼륨을 주문합니다.
```
   bluemix sl block volume-order [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-t, --storage-type</dt>
<dd>필수. 스토리지 볼륨의 유형. 옵션: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>필수. 스토리지 볼륨의 크기(GB).</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP[storage-type performance에 필요].</dd>
<dt>-e, --tier</dt>
<dd>Endurance 스토리지 계층(GB당 IOP)[storage-type endurance에 필요]. 옵션: 0.25,2,4,10.</dd>
<dt>-o, --os-type</dt>
<dd>필수. 운영 체제. 옵션: HYPER_V,LINUX,VMWARE,WINDOWS_2008,WINDOWS_GPT,WINDOWS,XEN.</dd>
<dt>-d, --datacenter</dt>
<dd>필수. 데이터 센터의 짧은 이름.</dd>
<dt>-n, --snapshot-size</dt>
<dd>Endurance 블록 스토리지와 함께 스냅샷 영역을 주문하기 위한 선택적 매개변수. 주문할 스냅샷 영역의 크기(GB)를 지정합니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl block volume-order --storage-type performance --size 1000 --iops 4000 --os-type LINUX -d dal09
```
이 명령은 크기가 1000GB, IOPS가 4000, OS 유형은 LINUX이고, dal09에 위치하는 performance 볼륨을 주문합니다.

### bluemix sl block volume-options
{: #sl_block_volume_options}

블록 스토리지 주문을 위한 모든 옵션을 나열합니다.
```
 bluemix sl block volume-options
```


**예제**:
```
 bluemix sl block volume-options
```
이 명령은 스토리지 유형, 볼륨 크기, OS 유형, IOPS, 계층 레벨, 데이터 센터 및 스냅샷 크기를 포함하여 블록 스토리지 볼륨 작성에 대한 모든 옵션을 나열합니다.


### bluemix sl cdn cancel
{: #sl_cdn_cancel}

CDN 계정을 취소합니다.
```
bluemix sl cdn cancel ACCOUNT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>
### bluemix sl cdn detail
{: #sl_cdn_detail}

CDN 계정을 상세히 설명합니다.
```
bluemix sl cdn detail ACCOUNT_ID
```

### bluemix sl cdn list
{: #sl_cdn_list}

모든 CDN 계정을 나열합니다.
```
bluemix sl cdn list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id, name, type, created.</dd>
<dt>--order</dt>
<dd>주문 ID별 필터링.</dd>
</dl>
### bluemix sl cdn load
{: #sl_cdn_load}

모든 에지 노드에 하나 이상의 파일을 캐시합니다.
```
bluemix sl cdn load ACCOUNT_ID CONTENT_URL [CONTENT_URL...]
```

### bluemix sl cdn order
{: #sl_cdn_order}

CDN 계정을 주문합니다.
```
bluemix sl cdn order [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-b, --bandwidth</dt>
<dd>CDN 대역폭. 지정되지 않은 경우 '종량과금제' 가격이 사용됩니다.</dd>
<dt>-s, --storage</dt>
<dd>CDN 스토리지. 지정되지 않은 경우 '종량과금제' 가격이 사용됩니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>
### bluemix sl cdn options
{: #sl_cdn_options}

CDN 계정 주문을 위한 대역폭 및 스토리지 옵션입니다.
```
bluemix sl cdn options
```

### bluemix sl cdn origin-add
{: #sl_cdn_origin_add}

원본 가져오기 맵핑을 작성합니다.
```
bluemix sl cdn origin-add ACCOUNT_ID CONTENT_URL [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-t, --type</dt>
<dd>이 맵핑의 매체 유형(http, flash, wm, ...). 기본값: http.</dd>
<dt>-c, --cname</dt>
<dd>맵핑에 첨부할 선택적 CNAME.</dd>
</dl>
### bluemix sl cdn origin-list
{: #sl_cdn_origin_list}

원본 가져오기 맵핑을 나열합니다.
```
bluemix sl cdn origin-list ACCOUNT_ID
```

### bluemix sl cdn origin-remove
{: #sl_cdn_origin_remove}

원본 가져오기 맵핑을 제거합니다.
```
bluemix sl cdn origin-remove ACCOUNT_ID ORIGIN_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>
### bluemix sl cdn purge
{: #sl_cdn_purge}

모든 에지 노드에서 캐시된 파일을 제거합니다.
```
bluemix sl cdn purge ACCOUNT_ID CONTENT_URL [CONTENT_URL...][OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>
### bluemix sl file access-authorize
{: #sl_file_access_authorize}

지정된 볼륨에 액세스하도록 호스트에 권한을 부여합니다.
```
bluemix sl file access-authorize VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --hardware-id</dt>
<dd>권한 부여할 하나의 하드웨어 서버의 ID입니다.</dd>
<dt>-v, --virtual-id</dt>
<dd>권한 부여할 하나의 가상 서버의 ID입니다.</dd>
<dt>-i, --ip-address-id</dt>
<dd>권한 부여할 하나의 IP 주소의 ID입니다.</dd>
<dt>-p, --ip-address</dt>
<dd>권한 부여할 IP 주소입니다.</dd>
<dt>-s, --subnet-id</dt>
<dd>권한 부여할 하나의 서브넷 ID입니다.</dd>
</dl>

**예제**:
```
bluemix sl file access-authorize 12345678 --virtual-id 87654321
```
이 명령은 ID 87654321인 가상 서버가 ID가 12345678인 볼륨에 액세스하도록 권한을 부여합니다.

### bluemix sl file access-list
{: #sl_file_access_list}

ACL을 나열합니다.
```
bluemix sl file access-list VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,name,type,private_ip_address,host_iqn,username,password.</dd>
<dt>--columns</dt>
<dd>표시할 열. 옵션: id,name,type,private_ip_address,host_iqn,username,password.</dd>
</dl>

**예제**:
```
bluemix sl file access-list 12345678 --sortby id
```
이 명령은 ID가 12345678인 볼륨에 액세스하도록 권한이 부여된 모든 호스트를 나열하고 ID별로 정렬합니다.

### bluemix sl file access-revoke
{: #sl_file_access_revoke}

지정된 볼륨에 액세스하는 호스트의 권한을 취소합니다.
```
bluemix sl file access-revoke VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --hardware-id</dt>
<dd>권한을 취소할 하나의 하드웨어 서버 ID.</dd>
<dt>-v, --virtual-id</dt>
<dd>권한을 취소할 하나의 가상 서버 ID.</dd>
<dt>-i, --ip-address-id</dt>
<dd>권한을 취소할 하나의 IP 주소 ID.</dd>
<dt>-p, --ip-address</dt>
<dd>권한을 취소할 하나의 IP 주소.</dd>
<dt>-s, --subnet-id</dt>
<dd>권한을 취소할 하나의 서브넷 ID.</dd>
</dl>

**예제**:
```
bluemix sl file access-revoke 12345678 --virtual-id 87654321
```
이 명령은 ID 87654321인 가상 서버의 ID가 12345678인 볼륨에 대한 액세스 권한을 취소합니다.

### bluemix sl file replica-failback
{: #sl_file_replica_failback}

복제본에서 파일 볼륨을 장애 복구합니다.
```
bluemix sl file replica-failback VOLUME_ID
```


**예제**:
```
bluemix sl file replica-failback 12345678
```
이 명령은 ID가 12345678인 볼륨에 대해 장애 복구 조작을 수행합니다.

### bluemix sl file replica-failover
{: #sl_file_replica_failover}

지정된 복제본 볼륨으로 파일 볼륨을 장애 복구합니다.
```
bluemix sl file replica-failover VOLUME_ID REPLICA_ID
```


**예제**:
```
bluemix sl file replica-failover 12345678 87654321
```
이 명령은 ID 87654321인 복제본 볼륨에 ID가 12345678인 볼륨에 대한 장애 복구 조작을 수행합니다.

### bluemix sl file replica-locations
{: #sl_file_replica_locations}

지정된 볼륨에 적합한 복제본 데이터 센터를 나열합니다.
```
bluemix sl file replica-locations VOLUME_ID
```


**예제**:
```
bluemix sl file replica-locations 12345678
```
이 명령은 ID가 12345678인 파일 볼륨에 적합한 복제본 데이터 센터를 나열합니다.

### bluemix sl file replica-order
{: #sl_file_replica_order}

파일 스토리지 복제본 볼륨을 주문합니다.
```
bluemix sl file replica-order VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --snapshot-schedule</dt>
<dd>필수. 복제에 사용할 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
<dt>-d, --datacenter</dt>
<dd>필수. 복제본에 대한 데이터 센터의 짧은 이름(예: dal09).</dd>
<dt>-t, --tier</dt>
<dd>선택사항. 복제본이 주문되는 기본 볼륨의 Endurance 스토리지 계층(GB당 IOPS). 옵션: 0.25,2,4,10. 계층이 지정되지 않은 경우 원본 볼륨의 계층이 사용됩니다.</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP. 지정되지 않은 경우 원본 볼륨의 IOPS가 사용됩니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file replica-order 12345678 -s DAILY -d dal09 --tier 4
```
이 명령은 ID가 12345678인 볼륨에 대한 복제본(일별 복제를 수행하며, dal09에 위치하고, 계층 레벨이 4임)을 주문합니다.

### bluemix sl file replica-partners
{: #sl_file_replica_partners}

파일 볼륨의 기존 복제본 볼륨을 나열합니다.
```
bluemix sl file replica-partners VOLUME_ID [OPTIONS]
```


**예제**:
```
bluemix sl file replica-partners 12345678
```
이 명령은 ID가 12345678인 파일 볼륨의 기존 복제본 볼륨을 나열합니다.

### bluemix sl file snapshot-cancel
{: #sl_file_snapshot_cancel}

지정된 볼륨의 기존 스냅샷 영역을 취소합니다.
```
bluemix sl file snapshot-cancel SNAPSHOT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--reason</dt>
<dd>취소에 대한 선택적 이유입니다.</dd>
<dt>--immediate</dt>
<dd>청구 주기 대신 즉시 스냅샷 영역 취소.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file snapshot-cancel 12345678 --immediate -f
```
이 명령은 확인을 요청하지 않고 즉시 ID가 12345678인 스냅샷을 취소합니다.

### bluemix sl file snapshot-create
{: #sl_file_snapshot_create}

지정된 볼륨에서 스냅샷을 작성합니다.
```
bluemix sl file snapshot-create VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-n, --note</dt>
<dd>새 스냅샷에 설정할 참고.</dd>
</dl>

**예제**:
```
bluemix sl file snapshot-create 12345678 --note snapshotforbluemix
```
이 명령은 snapshotforbluemix와 같은 추가 참고와 함께 ID가 12345678인 볼륨에 대한 스냅샷을 작성합니다.

### bluemix sl file snapshot-disable
{: #sl_file_snapshot_disable}

지정된 볼륨에서 지정된 스케줄에 따라 스냅샷을 사용 안함으로 설정합니다.
```
bluemix sl file snapshot-disable VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --schedule-type</dt>
<dd>필수. 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
</dl>

**예제**:
```
bluemix sl file snapshot-disable 12345678 -s DAILY
```
이 명령은 ID가 12345678인 볼륨에 대한 일별 스냅샷을 사용 안함으로 설정합니다.

### bluemix sl file snapshot-enable
{: #sl_file_snapshot_enable}

지정된 스케줄에 따라 지정된 볼륨의 스냅샷을 사용으로 설정합니다.
```
bluemix sl file snapshot-enable VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --schedule-type</dt>
<dd>필수. 스냅샷 스케줄. 옵션: HOURLY,DAILY,WEEKLY.</dd>
<dt>-c, --retention-count</dt>
<dd>필수. 유지할 스냅샷 수입니다.</dd>
<dt>-m, --minute</dt>
<dd>스냅샷을 작성해야 하는 시간(분), 0 - 59 사이의 정수. </dd>
<dt>-r, --hour</dt>
<dd>스냅샷을 작성해야 하는 시간, 0 - 23 사이의 정수. </dd>
<dt>-d, --day-of-week</dt>
<dd>스냅샷을 작성해야 하는 요일, 0 - 6 사이의 정수.
0은 일요일, 1은 월요일, 2는 화요일, 3은 수요일, 4는 목요일, 5는 금요일, 6은 토요일을 의미합니다. </dd>
</dl>

**예제**:
```
bluemix sl file snapshot-enable 12345678 -s WEEKLY -c 5 -m 0 --hour 2 -d 0
```
이 명령은 ID가 12345678인 볼륨의 스냅샷을 사용으로 설정하고, 스냅샷은 매주 일요일 2시에 작성되며 최대 5개의 스냅샷이 유지됩니다.

### bluemix sl file snapshot-delete
{: #sl_file_snapshot_delete}

지정된 볼륨에서 스냅샷을 삭제합니다.
```
bluemix sl file snapshot-delete SNAPSHOT_ID
```


**예제**:
```
bluemix sl file snapshot-delete 12345678
```
이 명령은 ID가 12345678인 스냅샷을 삭제합니다.

### bluemix sl file snapshot-list
{: #sl_file_snapshot_list}

파일 스토리지 스냅샷을 나열합니다.
```
bluemix sl file snapshot-list VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,name,created,size_bytes.</dd>
</dl>

**예제**:
```
bluemix sl file snapshot-list 12345678 --sortby id
```
이 명령은 ID가 12345678인 볼륨의 모든 스냅샷을 나열하고 ID별로 정렬합니다.

### bluemix sl file snapshot-order
{: #sl_file_snapshot_order}

파일 스토리지 볼륨의 스냅샷 영역을 주문합니다.
```
bluemix sl file snapshot-order VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --size</dt>
<dd>필수. 작성할 스냅샷 영역의 크기(GB).</dd>
<dt>-t, --tier</dt>
<dd>선택사항. 영역이 주문되는 파일 볼륨의 Endurance 스토리지 계층(GB당 IOPS). 옵션: 0.25,2,4,10.</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP.</dd>
<dt>-u, --upgrade</dt>
<dd>업그레이드 주문임을 표시하는 플래그.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file snapshot-order 12345678 -s 1000 -t 4
```
이 명령은 ID가 12345678인 볼륨에 대한 스냅샷 영역을 주문합니다. 크기는 1,000GB이고 계층 레벨은 GB당 4IOPS입니다.

### bluemix sl file snapshot-restore
{: #sl_file_snapshot_restore}

지정된 스냅샷을 사용하여 파일 볼륨을 복원합니다.
```
bluemix sl file snapshot-restore VOLUME_ID SNAPSHOT_ID
```


**예제**:
```
bluemix sl file snapshot-restore 12345678 87654321
```
이 명령은 ID 87654321인 스냅샷에서 ID가 12345678인 볼륨을 복원합니다.

### bluemix sl file volume-cancel
{: #sl_file_volume_cancel}

기존 파일 스토리지 볼륨을 취소합니다.
```
bluemix sl file volume-cancel VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--reason</dt>
<dd>취소에 대한 선택적 이유입니다.</dd>
<dt>--immediate</dt>
<dd>청구 주기 대신 즉시 파일 스토리지 볼륨 취소.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file volume-cancel 12345678 --immediate -f
```
이 명령은 확인을 요청하지 않고 즉시 ID가 12345678인 볼륨을 취소합니다.

### bluemix sl file volume-list
{: #sl_file_volume_list}

파일 스토리지를 나열합니다.
```
bluemix sl file volume-list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-u, --username</dt>
<dd>볼륨 사용자 이름별 필터링.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터 짧은 이름별 필터링.</dd>
<dt>-t, --storage-type</dt>
<dd>스토리지 볼륨 유형별 필터링. 옵션: performance,endurance.</dd>
<dt>-o, --order</dt>
<dd>파일 스토리지를 구매한 주문 ID별 필터링.</dd>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,active_transactions,mount_addr.</dd>
<dt>--columns</dt>
<dd>표시할 열. 옵션: id,username,datacenter,storage_type,capacity_gb,bytes_used,ip_addr,mount_addr.</dd>
</dl>

**예제**:
```
bluemix sl file volume-list -d dal09 -t endurance --sortby capacity_gb
```
이 명령은 dal09에 위치하는 현재 계정의 모든 endurance 볼륨을 나열하고 용량별로 정렬합니다.


### bluemix sl file volume-detail
{: #sl_file_volume_detail}

지정된 볼륨의 세부사항을 표시합니다.
```
bluemix sl file volume-detail VOLUME_ID
```


**예제**:
```
bluemix sl file volume-detail 12345678
```
이 명령은 ID가 12345678인 볼륨의 세부사항을 표시합니다.

### bluemix sl file volume-duplicate
{: #sl_file_volume_duplicate}

기존 볼륨을 복제하여 파일 볼륨을 주문합니다.
```
bluemix sl file volume-duplicate VOLUME_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-o, --origin-snapshot-id</dt>
<dd>복제에 사용할 원본 볼륨 스냅샷의 ID.</dd>
<dt>-s, --duplicate-size</dt>
<dd>중복 파일 볼륨의 크기(GB). 크기가 지정되지 않은 경우 원본 볼륨의 크기가 사용됩니다.</dd>
<dt>-i, --duplicate-iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOPS. 지정되지 않은 경우 원본 볼륨의 IOPS가 사용됩니다.</dd>
<dt>-t, --duplicate-tier</dt>
<dd>Endurance 스토리지 계층. 계층이 지정되지 않은 경우 원본 볼륨의 계층이 사용됩니다.</dd>
<dt>-n, --duplicate-snapshot-size</dt>
<dd>복제를 위해 주문할 스냅샷 영역의 크기. 스냅샷 영역 크기가 지정되지 않은 경우 원본 볼륨의 스냅샷 영역 크기가 사용됩니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file volume-duplicate 12345678
```
이 명령은 ID가 12345678인 볼륨을 복제하여 새 볼륨 주문을 표시합니다.

### bluemix sl file volume-order
{: #sl_file_volume_order}

파일 스토리지 볼륨을 주문합니다.
```
bluemix sl file volume-order [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-t, --storage-type</dt>
<dd>필수. 스토리지 볼륨의 유형. 옵션: performance,endurance.</dd>
<dt>-s, --size</dt>
<dd>필수. 스토리지 볼륨의 크기(GB).</dd>
<dt>-i, --iops</dt>
<dd>100 - 6000의 100의 배수인 Performance 스토리지 IOP[storage-type performance에 필요].</dd>
<dt>-e, --tier</dt>
<dd>Endurance 스토리지 계층(GB당 IOP)[storage-type endurance에 필요]. 옵션: 0.25,2,4,10.</dd>
<dt>-d, --datacenter</dt>
<dd>필수. 데이터 센터의 짧은 이름.</dd>
<dt>-n, --snapshot-size</dt>
<dd>볼륨과 함께 스냅샷 영역을 주문하기 위한 선택적 매개변수.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
bluemix sl file volume-order --storage-type performance --size 1000 --iops 4000  -d dal09
```
이 명령은 크기가 1000GB이고, IOPS가 4000이며, dal09에 위치하는 performance 볼륨을 주문합니다.

### bluemix sl file volume-options
{: #sl_file_volume_options}

파일 스토리지 주문을 위한 모든 옵션을 나열합니다.
```
bluemix sl file volume-options
```


**예제**:
```
bluemix sl file volume-options
```
이 명령은 스토리지 유형, 볼륨 크기, IOPS, 계층 레벨, 데이터 센터 및 스냅샷 크기를 포함하여 파일 스토리지 볼륨 작성을 위한 모든 옵션을 나열합니다.

### bluemix sl dns import
{: #sl_dns_import}

BIND 구역 파일과 다른 구역을 가져옵니다.
```
bluemix sl dns import ZONEFILE [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--dry-run</dt>
<dd>레코드를 실제로 작성하지 않음.</dd>
</dl>

**예제**:
```
 bluemix sl dns import ~/blumix.net.txt
```
이 명령은 ~/blumix.net.txt 파일에서 구역 및 해당 리소스 레코드를 가져옵니다.

### bluemix sl dns record-add
{: #sl_dns_record_add}

구역에 리소스 레코드를 추가합니다.
```
bluemix sl dns record-add ZONE RECORD TYPE DATA [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--ttl</dt>
<dd>TTL(Time-To-Live)(초). 예: 86400. 기본값: 7200.</dd>
</dl>

**예제**:
```
 bluemix sl dns record-add bluemix.net ftp A 127.0.0.1 --ttl 86400
```
이 명령은 A 레코드를 bluemix.net 구역에 추가합니다. 그 호스트는 "ftp"이고, 데이터는 "127.0.0.1"이며 ttl은 86400초입니다.

### bluemix sl dns record-edit
{: #sl_dns_record_edit}

구역의 리소스 레코드를 업데이트합니다.
```
   bluemix sl dns record-edit ZONE [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--by-record</dt>
<dd>호스트 레코드로 편집(예: www).</dd>
<dt>--by-id</dt>
<dd>해당 ID별로 단일 레코드 편집.</dd>
<dt>--data</dt>
<dd>레코드 데이터(예: IP 주소).</dd>
<dt>--ttl</dt>
<dd>TTL 값(초)(예: 86400).</dd>
</dl>

**예제**:
```
 bluemix sl dns record-edit bluemix.net --by-id 12345678 --data 127.0.0.2 --ttl 3600
```
이 명령은 ID가 12345678인 bluemix.net 구역 아래의 레코드를 편집하고, 해당 데이터는 "127.0.0.2"로 설정하고 ttl은 3600으로 설정합니다.

### bluemix sl dns record-list
{: #sl_dns_record_list}

구역의 모든 리소스 레코드를 나열합니다.
```
   bluemix sl dns record-list ZONE [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--data</dt>
<dd>레코드 데이터별 필터링(예: IP 주소).</dd>
<dt>--record</dt>
<dd>호스트 레코드로 필터링(예: www).</dd>
<dt>--ttl</dt>
<dd>TTL 값별 필터링(초)(예: 86400).</dd>
<dt>--type</dt>
<dd>레코드 유형별 필터링(예: A 또는 CNAME).</dd>
</dl>

**예제**:
```
 bluemix sl dns record-list bluemix.net --record elasticsearch --type A --ttl 900
```
이 명령은 bluemix.net 구역 아래의 모든 A 레코드를 나열합니다. 호스트 기준 필터링은 elasticsearch이고 ttl은 900초입니다.

### bluemix sl dns record-remove
{: #sl_dns_record_remove}

구역에서 리소스 레코드를 제거합니다.
```
 bluemix sl dns record-remove RECORD_ID
```


**예제**:
```
 bluemix sl dns record-remove 12345678
```
이 명령은 ID가 12345678인 리소스 레코드를 제거합니다.

### bluemix sl dns zone-create
{: #sl_dns_zone_create}

구역을 작성합니다.
```
 bluemix sl dns zone-create ZONE
```


**예제**:
```
 bluemix sl dns zone-create bluemix.net
```
이 명령은 이름이 bluemix.net인 구역을 작성합니다.

### bluemix sl dns zone-delete
{: #sl_dns_zone_delete}

구역을 삭제합니다.
```
 bluemix sl dns zone-delete ZONE
```


**예제**:
```
 bluemix sl dns zone-delete bluemix.net
```
이 명령은 이름이 bluemix.net인 구역을 삭제합니다.

### bluemix sl dns zone-list
{: #sl_dns_zone_list}

계정의 모든 구역을 나열합니다.
```
   bluemix sl dns zone-list
```


**예제**:
```
   bluemix sl dns zone-list
```
이 명령은 현재 계정 아래의 모든 구역을 나열합니다.

### bluemix sl dns zone-print
{: #sl_dns_zone_print}

구역 및 리소스 레코드를 BIND 형식으로 인쇄합니다.
```
 bluemix sl dns zone-print ZONE
```


**예제**:
```
 bluemix sl dns zone-print bluemix.net
```
이 명령은 BIND 형식으로 bluemix.net이라는 구역을 인쇄합니다.


### bluemix sl globalip create
{: #sl_globalip_create}

글로벌 IP를 작성합니다.
```
bluemix sl globalip create [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--v6</dt>
<dd>IPv6 IP 주소 주문.</dd>
<dt>--test</dt>
<dd>테스트 주문.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
     bluemix sl globalip create --v6
```
이 명령은 IP V6 주소를 작성합니다.

### bluemix sl globalip assign
{: #sl_globalip_assign}

대상 라우터 또는 디바이스에 글로벌 IP를 지정합니다.
```
bluemix sl globalip assign IDENTIFIER TARGET
```


**예제**:
```
 bluemix sl globalip assign 12345678 9.111.123.456
```
이 명령은 ID가 12345678인 IP 주소를 IP 주소가 9.111.123.456인 대상 디바이스에 지정합니다.


### bluemix sl globalip cancel
{: #sl_globalip_cancel}

글로벌 IP를 취소합니다.
```
bluemix sl globalip cancel IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl globalip cancel 12345678
```
이 명령은 ID가 12345678인 IP 주소를 취소합니다.

### bluemix sl globalip list
{: #sl_globalip_list}

계정의 모든 글로벌 IP를 나열합니다.
```
bluemix sl globalip list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--v4</dt>
<dd>IPv4 IP만 표시.</dd>
<dt>--v6</dt>
<dd>IPv6 IP만 표시.</dd>
<dt>--order</dt>
<dd>이 IP 주소를 구매한 주문의 ID별 필터링.</dd>
</dl>

**예제**:
```
bluemix sl globalip list --v4
```
이 명령은 현재 계정의 모든 IP V4 주소를 나열합니다.

### bluemix sl globalip unassign
{: #sl_globalip_unassign}

대상 라우터 또는 디바이스에서 글로벌 IP의 지정을 해제합니다.
```
 bluemix sl globalip unassign IDENTIFIER
```


**예제**:
```
 bluemix sl globalip unassign 12345678
```
이 명령은 대상 디바이스에서 ID가 12345678인 IP 주소의 지정을 해제합니다.

### bluemix sl image delete
{: #sl_image_delete}

이미지를 삭제합니다.
```
   bluemix sl image delete IDENTIFIER
```
**예제**:
```
   bluemix sl image delete 12345678
```
이 명령은 ID `12345678`인 이미지를 삭제합니다.

### bluemix sl image detail
{: #sl_image_detail}

이미지의 세부사항을 가져옵니다.
```
 bluemix sl image detail IDENTIFIER
```
**예제**:
```
 bluemix sl image detail 12345678
```
이 명령은 ID가 12345678인 이미지의 세부사항을 가져옵니다.

### bluemix sl image edit
{: #sl_image_edit}

이미지의 세부사항을 편집합니다.
```
   bluemix sl image edit IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--name</dt>
<dd>이미지의 이름입니다.</dd>
<dt>--note</dt>
<dd>이미지에 대한 추가 참고입니다.</dd>
<dt>--tag</dt>
<dd>이미지에 대한 태그입니다.</dd>
</dl>

*예제**:
```  
bluemix sl image edit 12345678 --name ubuntu16 --note testing --tag staging
```
이 명령은 ID `12345678`인 이미지를 편집하고, 해당 이름을 `ubuntu16`으로, 참고를 `testing`으로, 태그를 `staging`으로 설정합니다.

### bluemix sl image list
{: #sl_image_list}

계정의 모든 이미지를 나열합니다.
```
   bluemix sl image list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--name</dt>
<dd>이미지 이름 필터링.</dd>
<dt>--public</dt>
<dd>공용 이미지만 표시.</dd>
<dt>--private</dt>
<dd>개인용 이미지만 표시.</dd>
</dl>

### bluemix sl ipsec cancel
{: #sl_ipsec_cancel}

IPSec VPN 터널 컨텍스트를 취소합니다.
```
bluemix sl ipsec cancel CONTEXT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--immediate</dt>
<dd>청구 주기 대신 즉시 IPSec 취소.</dd>
<dt>--reason</dt>
<dd>취소에 대한 선택적 이유입니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl ipsec config
{: #sl_ipsec_config}

터널 컨텍스트의 구성을 요청합니다.
```
bluemix sl ipsec config CONTEXT_ID [OPTIONS]
```

### bluemix sl ipsec detail
{: #sl_ipsec_detail}

IPSec VPN 터널 컨텍스트 세부사항을 나열합니다.
```
bluemix sl ipsec detail CONTEXT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-i, --include</dt>
<dd>추가 리소스 포함. 옵션: at,is,rs,sr,ss.</dd>
</dl>
### bluemix sl ipsec list
{: #sl_ipsec_list}

IPSec VPN 터널 컨텍스트를 나열합니다.
```
bluemix sl ipsec list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--order</dt>
<dd>IPSEC을 구매한 주문 ID별 필터링.</dd>
</dl>
### bluemix sl ipsec order
{: #sl_ipsec_order}

IPSec VPN 터널을 주문합니다.
```
bluemix sl ipsec order [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --datacenter</dt>
<dd>필수. IPSEC에 대한 데이터 센터의 짧은 이름(예: dal09).</dd>
</dl>

### bluemix sl ipsec subnet-add
{: #sl_ipsec_subnet_add}

IPSec 터널 컨텍스트에 서브넷을 추가합니다.
```
bluemix sl ipsec subnet-add CONTEXT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --subnet-id</dt>
<dd>추가할 서브넷 ID. 필수.</dd>
<dt>-t, --subnet-type</dt>
<dd>추가할 서브넷 유형. 필수. 옵션: internal,remote,service.</dd>
<dt>-n, --network</dt>
<dd>작성할 서브넷 네트워크 ID.</dd>
</dl>

### bluemix sl ipsec subnet-remove
{: #sl_ipsec_subnet_remove}

IPSEC 터널 컨텍스트에서 서브넷을 제거합니다.
```
bluemix sl ipsec subnet-remove CONTEXT_ID SUBNET_ID SUBNET_TYPE [OPTIONS]
```

### bluemix sl ipsec translation-add
{: #sl_ipsec_translation_add}

IPSec 터널에 주소 변환을 추가합니다.
```
bluemix sl ipsec translation-add CONTEXT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --static-ip</dt>
<dd>정적 IP 주소. 필수.</dd>
<dt>-r, --remote-ip</dt>
<dd>원격 IP 주소. 필수.</dd>
<dt>-n, --note</dt>
<dd>참고.</dd>
</dl>
### bluemix sl ipsec translation-remove
{: #sl_ipsec_translation_remove}

IPSec에서 변환 항목을 제거합니다.
```
bluemix sl ipsec translation-remove CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

### bluemix sl ipsec translation-update
{: #sl_ipsec_translation_update}

IPSec의 주소 변환을 업데이트합니다.
```
bluemix sl ipsec translation-update CONTEXT_ID TRANSLATION_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-s, --static-ip</dt>
<dd>정적 IP 주소. 필수.</dd>
<dt>-r, --remote-ip</dt>
<dd>원격 IP 주소. 필수.</dd>
<dt>-n, --note</dt>
<dd>참고.</dd>
</dl>
### bluemix sl ipsec update
{: #sl_ipsec_update}

터널 컨텍스트 특성을 업데이트합니다.
```
bluemix sl ipsec update CONTEXT_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-n, --name</dt>
<dd>별명.</dd>
<dt>-r, --remote-peer</dt>
<dd>원격 피어 IP 주소.</dd>
<dt>-k, --preshared-key</dt>
<dd>사전 공유된 키.</dd>
<dt>-a, --phase1-auth</dt>
<dd>1단계(Phase) 인증. 옵션: MD5,SHA1,SHA256.</dd>
<dt>-c, --phase1-crypto</dt>
<dd>1단계(Phase) 암호화. 옵션: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-d, --phase1-dh</dt>
<dd>1단계(Phase) diffie hellman 그룹. 옵션: 0,1,2,5.</dd>
<dt>-t, --phase1-key-ttl</dt>
<dd>1단계(Phase) 키 수명. 범위: 120 - 172800.</dd>
<dt>-u, --phase2-auth</dt>
<dd>2단계(Phase) 인증. 옵션: MD5,SHA1,SHA256.</dd>
<dt>-y, --phase2-crypto</dt>
<dd>2단계(Phase) 암호화. 옵션: DES,3DES,AES128,AES192,AES256.</dd>
<dt>-e, --phase2-dh</dt>
<dd>2단계(Phase) diffie hellman 그룹. 옵션: 0,1,2,5.</dd>
<dt>-f, --phase2-forward-secrecy</dt>
<dd>2단계(Phase) PFS(Perfect Forward Secrecy). 범위: 0 - 1.</dd>
<dt>-l, --phase2-key-ttl</dt>
<dd>2단계(Phase) 키 수명. 범위: 120 - 172800.</dd>
</dl>

### bluemix sl loadbal cancel
{: #sl_loadbal_cancel}

기존 로드 밸런서를 취소합니다.
```
bluemix sl loadbal cancel LOADBAL_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl loadbal create
{: #sl_loadbal_create}

작성-옵션에서 리턴된 ID가 지정된 로드 밸런서를 추가합니다.
```
bluemix sl loadbal create PRICE_ID LOCATION [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl loadbal create-options
{: #sl_loadbal_create_options}

로드 밸런서를 작성하기 위한 가격 옵션을 가져옵니다.
```
bluemix sl loadbal create-options
```

### bluemix sl loadbal detail
{: #sl_loadbal_detail}

로드 밸런서 세부사항을 가져옵니다.
```
bluemix sl loadbal detail LOADBAL_ID
```

### bluemix sl loadbal group-add
{: #sl_loadbal_group_add}

새 로드 밸런서 서비스를 추가합니다.
```
bluemix sl loadbal group-add LOADBAL_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-a, --allocation</dt>
<dd>필수. 연결의 할당된 백분율.</dd>
<dt>-p, --port</dt>
<dd>필수. 포트 번호.</dd>
<dt>-t, --routing-type</dt>
<dd>필수. 라우팅 유형의 ID. ID를 찾으려면 'bluemix sl loadbal routing-types'를 실행하십시오.</dd>
<dt>-m, --routing-method</dt>
<dd>필수. 라우팅 메소드의 ID. ID를 찾으려면 'bluemix sl loadbal routing-methods'를 실행하십시오.</dd>
</dl>

### bluemix sl loadbal group-delete
{: #sl_loadbal_group_delete}

기존 로드 밸런서 서비스 그룹을 삭제합니다.
```
bluemix sl loadbal group-delete GROUP_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl loadbal group-edit
{: #sl_loadbal_group_edit}

기존 로드 밸런서 서비스 그룹을 편집합니다.
```
bluemix sl loadbal group-edit LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-a, --allocation</dt>
<dd>연결의 할당된 백분율을 변경합니다.</dd>
<dt>-p, --port</dt>
<dd>포트 번호를 변경합니다.</dd>
<dt>-t, --routing-type</dt>
<dd>라우팅 유형의 ID를 변경합니다. ID를 찾으려면 'bluemix sl loadbal routing-types'를 실행하십시오.</dd>
<dt>-m, --routing-method</dt>
<dd>라우팅 메소드의 ID를 변경합니다. ID를 찾으려면 'bluemix sl loadbal routing-methods'를 실행하십시오.</dd>
</dl>

### bluemix sl loadbal group-reset
{: #sl_loadbal_group_reset}

특정 서비스 그룹에서 연결을 재설정합니다.
```
bluemix sl loadbal group-reset LOADBAL_ID GROUP_ID
```

### bluemix sl loadbal health-checks
{: #sl_loadbal_health_checks}

상태 검사 유형을 나열합니다.
```
bluemix sl loadbal health-checks
```

### bluemix sl loadbal list
{: #sl_loadbal_list}

활성 로드 밸런서를 나열합니다.
```
bluemix sl loadbal list
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-d, --datacenter</dt>
<dd>데이터 센터 짧은 이름별 필터링.</dd>
<dt>-o, --order</dt>
<dd>로드 밸런서를 구매한 주문 ID별 필터링.</dd>
<dt>-p, --ip-address</dt>
<dd>IP 주소별 필터링.</dd>
</dl>
### bluemix sl loadbal routing-methods
{: #sl_loadbal_routing_methods}

라우팅 메소드를 나열합니다.
```
bluemix sl loadbal routing-methods
```

### bluemix sl loadbal routing-types
{: #sl_loadbal_routing_types}

라우팅 유형을 나열합니다.
```
bluemix sl loadbal routing-types
```

### bluemix sl loadbal service-add
{: #sl_loadbal_service_add}

새 로드 밸런서 서비스를 추가합니다.
```
bluemix sl loadbal service-add LOADBAL_ID GROUP_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--disabled</dt>
<dd>선택사항. 서비스를 사용 안함으로 작성합니다. 지정되지 않은 경우 기본값이 사용됩니다.</dd>
<dt>-p, --port</dt>
<dd>필수. 서비스의 포트 번호.</dd>
<dt>-w, --weight</dt>
<dd>필수. 서비스의 가중치.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>필수. 상태 검사 유형.</dd>
<dt>-i, --ip-address</dt>
<dd>필수. 서비스의 IP 주소.</dd>
</dl>

### bluemix sl loadbal service-delete
{: #sl_loadbal_service_delete}

기존 로드 밸런서 서비스를 삭제합니다.
```
bluemix sl loadbal service-delete SERVICE_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl loadbal service-edit
{: #sl_loadbal_service_edit}

서비스 그룹의 특성을 편집합니다.
```
bluemix sl loadbal service-edit LOADBAL_ID SERVICE_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--disabled</dt>
<dd>서비스를 사용 안함으로 설정합니다.</dd>
<dt>--enabled</dt>
<dd>서비스를 사용으로 설정합니다.</dd>
<dt>-p, --port</dt>
<dd>서비스의 포트 번호를 변경합니다.</dd>
<dt>-w, --weight</dt>
<dd>서비스의 가중치를 변경합니다.</dd>
<dt>-t, --healthcheck-type</dt>
<dd>상태 검사 유형을 변경합니다.</dd>
<dt>-i, --ip-address</dt>
<dd>서비스의 IP 주소를 변경합니다.</dd>
</dl>

### bluemix sl loadbal service-toggle
{: #sl_loadbal_service_toggle}

기존 로드 밸런서 서비스의 상태를 토글합니다.
```
bluemix sl loadbal service-toggle SERVICE_ID
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

### bluemix sl security sshkey-add
{: #sl_security_sshkey_add}

새 SSH 키를 추가합니다.
```
 bluemix sl security sshkey-add LABEL [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --in-file</dt>
<dd>이 키를 위해 가져올 id_rsa.pub 파일.</dd>
<dt>-k, --key</dt>
<dd>실제 SSH 키.</dd>
<dt>--note</dt>
<dd>키와 연관되는 추가 참고.</dd>
</dl>

**예제**:
```
 bluemix sl security sshkey-add -f ~/.ssh/id_rsa.pub --note mykey
```
이 명령은 ~/.ssh/id_rsa.pub 파일에서 "mykey" 참고가 지정된 SSH 키를 추가합니다.


### bluemix sl security sshkey-edit
{: #sl_security_sshkey_edit}

SSH 키를 편집합니다.
```
 bluemix sl security sshkey-edit IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--label</dt>
<dd>키의 새 레이블.</dd>
<dt>--note</dt>
<dd>키의 새 참고.</dd>
</dl>

**예제**:
```
 bluemix sl security sshkey-edit 12345678 --label Bluemix --note testing
```
이 명령은 ID가 12345678인 SSH 키를 업데이트하고 레이블을 "Bluemix"로 설정하고 참고를 "testing"으로 설정합니다.

### bluemix sl security sshkey-list
{: #sl_security_sshkey_list}

계정의 SSH 키를 나열합니다.
```
 bluemix sl security sshkey-list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,label,fingerprint,notes.</dd>
</dl>

**예제**:
```
 bluemix sl security sshkey-list --sortby label
```
이 명령은 현재 계정의 모든 SSH 키를 나열하고 레이블별로 정렬합니다.

### bluemix sl security sshkey-print
{: #sl_security_sshkey_print}

SSH 키를 화면에 인쇄합니다.
```
 bluemix sl security sshkey-print IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --out-file</dt>
<dd>공용 SSH 키가 이 파일에 작성됩니다. </dd>
</dl>

**예제**:
```
 bluemix sl security sshkey-print 12345678 -f ~/mykey.pub
```
이 명령은 ID와 레이블 그리고 ID가 12345678인 SSH 키의 참고를 표시하고 공개 키를 ~/mykey.pub 파일에 작성합니다.

### bluemix sl security sshkey-remove
{: #sl_security_sshkey_remove}

SSH 키를 영구적으로 제거합니다.
```
 bluemix sl security sshkey-remove IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl security sshkey-remove 12345678 -f
```
이 명령은 확인 요청 없이 ID가 12345678인 SSH 키를 제거합니다.

### bluemix sl security cert-add
{: #sl_security_cert_add}

SSL 인증서 세부사항을 추가하고 업로드합니다.
```
 bluemix sl security cert-add [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--crt</dt>
<dd>인증 파일.</dd>
<dt>--csr</dt>
<dd>인증서 서명 요청 파일.</dd>
<dt>--icc</dt>
<dd>중간 인증서 파일.</dd>
<dt>--key</dt>
<dd>개인 키 파일.</dd>
<dt>--notes</dt>
<dd>추가 참고.</dd>
</dl>

**예제**:
```
 bluemix sl security cert-add --crt ~/bluemix.net.cert --key ~/bluemix.net.key 
```
이 명령은 도메인 bluemix.net에 대한 인증서 파일 ~/bluemix.net.cert 및 개인 키 파일 ~/bluemix.net.key를 추가합니다.

### bluemix sl security cert-edit
{: #sl_security_cert_edit}

SSL 인증서를 편집합니다.
```
 bluemix sl security cert-edit IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--crt</dt>
<dd>인증 파일.</dd>
<dt>--csr</dt>
<dd>인증서 서명 요청 파일.</dd>
<dt>--icc</dt>
<dd>중간 인증서 파일.</dd>
<dt>--key</dt>
<dd>개인 키 파일.</dd>
<dt>--notes</dt>
<dd>추가 참고.</dd>
</dl>

**예제**:
```
 bluemix sl security cert-edit 12345678 --key ~/bluemix.net.key
```
이 명령은 ID가 12345678인 인증서를 편집하고 해당 개인 키를 ~/bluemix.net.key 파일로 업데이트합니다.

### bluemix sl security cert-download
{: #sl_security_cert_download}

SSL 인증서 및 키 파일을 다운로드합니다.
```
 bluemix sl security cert-download IDENTIFIER
```


**예제**:
```
 bluemix sl security cert-download 12345678
```
이 명령은 ID가 12345678인 인증서에 대해 현재 디렉토리에 4개 파일을 다운로드합니다. 4개 파일은 인증서 파일, 인증서 서명 요청 파일, 중간 인증서 파일 및 개인 키 파일입니다.

### bluemix sl security cert-list
{: #sl_security_cert_list}

계정의 SSL 인증서를 나열합니다.
```
 bluemix sl security cert-list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--status</dt>
<dd>이 상태의 인증서 표시. 기본값: all, options are: all,valid,expired.</dd>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,common_name,days_until_expire,notes.</dd>
</dl>

**예제**:
```
 bluemix sl security cert-list --status valid --sortby days_until_expire
```
이 명령은 현재 계정의 모든 유효한 인증서를 나열하고 유효성 검증일 기준으로 정렬합니다.

### bluemix sl security cert-remove
{: #sl_security_cert_remove}

SSL 인증서를 제거합니다.
```
 bluemix sl security cert-remove IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl security cert-remove 12345678
```
이 명령은 ID가 12345678인 인증서를 제거합니다.

### bluemix sl subnet cancel
{: #sl_subnet_cancel}

서브넷을 취소합니다.
```
bluemix sl subnet cancel IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl subnet cancel 12345678 -f
```
이 명령은 확인 요청 없이 ID가 12345678인 서브넷을 취소합니다.

### bluemix sl subnet create
{: #sl_subnet_create}

계정에 새 서브넷을 추가합니다.
```
   bluemix sl subnet create NETWORK QUANTITY VLAN_ID [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--v6, --ipv6</dt>
<dd>IPv6 주소 주문.</dd>
<dt>--test</dt>
<dd>서브넷을 주문하지 않음. 견적서만 가져오기.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl subnet create public 16 567
```
이 명령은 16개의 IP v4 주소를 사용하여 공용 서브넷을 작성하고 ID 567인 VLAN에 배치합니다.



### bluemix sl subnet detail
{: #sl_subnet_detail}

서브넷의 세부사항을 가져옵니다.
```
   bluemix sl subnet detail IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--no-vs</dt>
<dd>가상 서버 목록 숨기기.</dd>
<dt>--no-hardware</dt>
<dd>하드웨어 목록 숨기기.</dd>
</dl>

**예제**:
```
 bluemix sl subnet detail 12345678
```
이 명령은 가상 서버 및 하드웨어 서버 정보를 포함하여 ID가 12345678인 서브넷에 대한 자세한 정보를 표시합니다.


### bluemix sl subnet list
{: #sl_subnet_list}

계정의 모든 서브넷을 나열합니다.
```
   bluemix sl subnet list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열. 옵션: id,identifier,type,network_space,datacenter,vlan_id,IPs,hardware,vs.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터 짧은 이름별 필터링.</dd>
<dt>--identifier</dt>
<dd>네트워크 ID별 필터링.</dd>
<dt>-t, --subnet-type</dt>
<dd>서브넷 유형별 필터링.</dd>
<dt>--network-space</dt>
<dd>네트워크 영역별 필터링.</dd>
<dt>--v4, --ipv4</dt>
<dd>IPv4 서브넷만 표시.</dd>
<dt>--v6, --ipv6</dt>
<dd>IPv6 서브넷만 표시.</dd>
<dt>--order</dt>
<dd>서브넷을 구매한 주문 ID별 필터링.</dd>
</dl>

**예제**:
```
 bluemix sl subnet list -d dal09 -t PRIMARY --network-space PUBLIC --v4
```
이 명령은 현재 계정의 IP V4 서브넷을 나열합니다. 데이터 센터 기준 필터링은 dal09이고, 서브넷 유형은 PRIMARY이며 네트워크 영역은 PUBLIC입니다.



### bluemix sl subnet lookup
{: #sl_subnet_lookup}

IP 주소를 찾고 해당 서브넷 및 디바이스 정보를 표시합니다.
```
   bluemix sl subnet lookup IP_ADDRESS
```


**예제**:
```
 bluemix sl subnet lookup 9.125.235.255
```
이 명령은 주소가 9.125.235.255인 IP 주소 레코드를 찾고 해당 서브넷과 디바이스 정보를 표시합니다.


### bluemix sl vlan create
{: #sl_vlan_create}

새 VLAN을 작성합니다.
```
   bluemix sl vlan create [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-t, --vlan-type</dt>
<dd>VLAN의 유형(공용 또는 사설).</dd>
<dt>-r, --router</dt>
<dd>라우터의 호스트 이름.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터의 짧은 이름.</dd>
<dt>-s, --size</dt>
<dd>서브넷의 크기. 옵션: 8(사용 가능한 5개의 IP), 16(사용 가능한 13개의 IP) 또는 32(사용 가능한 29개의 IP).</dd>
<dt>-n, --name</dt>
<dd>VLAN의 이름.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vlan create -t public -d dal09 -s 16 -n myvlan
```
이 명령은 16개의 IP 주소와 함께 데이터 센터 dal09에 위치하고 이름이 myvlan인 공용 VLAN을 작성합니다.
### bluemix sl vlan cancel
{: #sl_vlan_cancel}

VLAN을 취소합니다.
```
   bluemix sl vlan cancel IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
   bluemix sl vlan cancel 12345678 -f
```
이 명령은 확인 요청 없이 ID가 12345678인 VLAN을 취소합니다.



### bluemix sl vlan detail
{: #sl_vlan_detail}

VLAN에 대한 세부사항을 가져옵니다.
```
   bluemix sl vlan detail IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--no-vs</dt>
<dd>가상 서버 목록 숨기기.</dd>
<dt>--no-hardware</dt>
<dd>하드웨어 목록 숨기기.</dd>
</dl>

**예제**:
```
 bluemix sl vlan detail 12345678  --no-vs --no-hardware
```
이 명령은 ID가 12345678인 VLAN의 세부사항을 표시하며 가상 서버 또는 하드웨어 서버는 나열하지 않습니다.


### bluemix sl vlan edit
{: #sl_vlan_edit}

VLAN에 대한 세부사항을 편집합니다.
```
   bluemix sl vlan edit IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-n, --name</dt>
<dd>VLAN의 이름.</dd>
</dl>

**예제**:
```
 bluemix sl vlan edit 12345678 -n myvlan-rename
```
이 명령은 ID가 12345678인 VLAN을 업데이트하고 새 이름으로 "myvlan-rename"을 지정합니다.


### bluemix sl vlan list
{: #sl_vlan_list}

계정의 모든 VLAN을 나열합니다.
```
 bluemix sl vlan list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--sortby</dt>
<dd>정렬 기준 열, 옵션: id, number, name, firewall, datacenter, hardware, virtual_servers, public_ips.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터 짧은 이름별 필터링.</dd>
<dt>-n, --number</dt>
<dd>VLAN 번호별 필터링.</dd>
<dt>--name</dt>
<dd>VLAN 이름별 필터링.</dd>
<dt>--order</dt>
<dd>VLAN을 구매한 주문 ID별 필터링.</dd>
</dl>

**예제**:
```
 bluemix sl vlan list -d dal09 --sortby number
```
이 명령은 현재 계정의 모든 VLAN을 나열합니다. 데이터 센터 기준 필터링은 dal09와 동일하고 VLAN 번호별로 정렬합니다.




### bluemix sl vlan options
{: #sl_vlan_options}

VLAN 작성을 위한 모든 옵션을 나열합니다.
```
 bluemix sl vlan options
```


**예제**:
```
 bluemix sl vlan options
```
이 명령은 VLAN을 작성하기 위한 모든 옵션(예: VLAN 유형, 데이터 센터, 서브넷 크기, 라우터 등)을 나열합니다.

### bluemix sl vs cancel
{: #sl_vs_cancel}

가상 서버 인스턴스를 취소합니다.
```
   bluemix sl vs cancel IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs cancel 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스를 취소합니다.


### bluemix sl vs capture
{: #sl_vs_capture}

가상 서버 인스턴스를 이미지로 캡처합니다.
```
 bluemix sl vs capture IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-n, --name</dt>
<dd>필수. 이미지의 이름입니다.</dd>
<dt>--all</dt>
<dd>VS에 속해 있는 모든 디스크 캡처.</dd>
<dt>--note</dt>
<dd>이미지와 연관시킬 참고 추가.</dd>
</dl>

**예제**:
```
 bluemix sl vs capture 12345678 -n mybluemix --all --note testing
```
이 명령은 모든 디스크와 함께 ID가 12345678인 가상 서버 인스턴스를 이름이 "mybluemix"이며 "testing" 참고가 지정된 이미지로 캡처합니다.



### bluemix sl vs create
{: #sl_vs_create}

가상 서버 인스턴스를 작성합니다.
```
   bluemix sl vs create [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-H, --hostname</dt>
<dd>필수. FQDN의 호스트 부분. </dd>
<dt>-D, --domain</dt>
<dd>필수. FQDN의 도메인 부분.</dd>
<dt>-c, --cpu</dt>
<dd>필수. CPU 코어 수.</dd>
<dt>-m, --memory</dt>
<dd>필수. 메모리(MB).</dd>
<dt>-d, --datacenter</dt>
<dd>필수. 데이터 센터의 짧은 이름.</dd>
<dt>-o, --os</dt>
<dd>OS 설치 코드. 팁: <OS>_LATEST를 지정할 수 있습니다.</dd>
<dt>--image</dt>
<dd>이미지 ID. 'bluemix sl image list'를 참조하십시오.</dd>
<dt>--billing</dt>
<dd>청구 비율. 기본값: hourly. 옵션: hourly, monthly.</dd>
<dt>--dedicated</dt>
<dd>데디케이티드 가상 서버 작성(개인용 노드).</dd>
<dt>--san</dt>
<dd>로컬 디스크 대신 SAN 스토리지 사용.</dd>
<dt>--test</dt>
<dd>가상 서버를 실제로 작성하지 않음.</dd>
<dt>--export</dt>
<dd>템플리트 파일로 옵션 내보내기.</dd>
<dt>-i, --postinstall</dt>
<dd>다운로드할 사후 설치 스크립트.</dd>
<dt>-k, --key</dt>
<dd>루트 사용자에게 추가할 SSH 키 ID(다중 발생 허용).</dd>
<dt>--disk</dt>
<dd>디스크 크기(다중 발생 허용).</dd>
<dt>--private</dt>
<dd>가상 서버가 사설 네트워크만 액세스하도록 강제 실행.</dd>
<dt>--like</dt>
<dd>기존 가상 서버의 구성 사용.</dd>
<dt>-n, --network</dt>
<dd>네트워크 포트 속도(Mbps).</dd>
<dt>--tag</dt>
<dd>인스턴스에 추가할 태그(다중 발생 허용).</dd>
<dt>-t, --template</dt>
<dd>명령행 옵션을 기본값으로 설정하는 템플리트 파일.</dd>
<dt>-u, --userdata</dt>
<dd>사용자 정의 메타데이터 문자열.</dd>
<dt>-F, --userfile</dt>
<dd>파일에서 사용자 데이터 읽기.</dd>
<dt>--vlan-public</dt>
<dd>가상 서버를 배치하려는 공용 VLAN ID.</dd>
<dt>--vlan-private</dt>
<dd>가상 서버를 배치하려는 사설 VLAN ID.</dd>
<dt>--wait</dt>
<dd>리턴하기 전에 가상 서버가 프로비저닝을 완료할 때까지 최대 X초 동안 대기.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
  bluemix sl vs create -H myvsi -D bluemix.net -c 4 -m 4096 -d dal10 -o UBUNTU_16_64 --disk 100 --disk 1000 --vlan-public 413
```
이 명령은 호스트 이름이 myvsi이고 도메인이 bluemix.net이며 4개의 CPU 코어와 4096M 메모리를 포함하며 데이터 센터 dal10에 위치하는 가상 서버 인스턴스를 주문합니다.

### bluemix sl vs options
{: #sl_vs_options}

가상 서버 인스턴스 작성을 위한 옵션을 나열합니다.
```
   bluemix sl vs options [OPTIONS]
```


**예제**:
```
 bluemix sl vs options
```
이 명령은 가상 서버 인스턴스를 작성하기 위한 모든 옵션(예: 데이터 센터, CPU, 메모리, OS, 디스크, 네트워크 속도 등)을 나열합니다.

### bluemix sl vs credentials
{: #sl_vs_credentials}

가상 서버 인스턴스 신임 정보를 나열합니다.
```
   bluemix sl vs credentials IDENTIFIER [OPTIONS]
```


**예제**:
```
 bluemix sl vs credentials 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스의 모든 사용자 이름과 비밀번호 쌍을 나열합니다.

### bluemix sl vs detail
{: #sl_vs_detail}

가상 서버 인스턴스의 세부사항을 가져옵니다.
```
   bluemix sl vs detail IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--passwords</dt>
<dd>비밀번호를 표시합니다(유출되지 않도록 주의).</dd>
<dt>--price</dt>
<dd>연관된 가격을 표시합니다.</dd>
</dl>

**예제**:
```
   bluemix sl vs details 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스에 대한 자세한 정보를 나열합니다.


### bluemix sl vs dns-sync
{: #sl_vs_dns_sync}

가상 서버 인스턴스의 DNS 레코드를 동기화합니다.
```
   bluemix sl vs dns-sync IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-a, --a-record</dt>
<dd>호스트의 A 레코드를 동기화합니다.</dd>
<dt>--aaaa-record</dt>
<dd>호스트의 AAAA 레코드를 동기화합니다.</dd>
<dt>--ptr</dt>
<dd>호스트의 PTR 레코드를 동기화합니다.</dd>
<dt>--ttl</dt>
<dd>A 및/또는 PTR 레코드용 TTL을 설정합니다. 기본값은 7200입니다.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs dns-sync 12345678 --a-record --ttl 3600
```
이 명령은 ID가 12345678인 가상 서버 인스턴스의 A 레코드(IP V4 주소)를 DNS 서버에 동기화하고 이 A 레코드의 ttl을 3600으로 설정합니다.
### bluemix sl vs edit
{: #sl_vs_edit}

가상 서버 인스턴스의 세부사항을 편집합니다.
```
   bluemix sl vs edit IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-D, --domain</dt>
<dd>FQDN의 도메인 부분.</dd>
<dt>-H, --hostname</dt>
<dd>FQDN의 호스트 부분. 예: server.</dd>
<dt>--tag</dt>
<dd>설정할 태그 또는 모두 제거하려면 빈 문자열 지정.</dd>
<dt>-u, --userdata</dt>
<dd>사용자 정의 메타데이터 문자열.</dd>
<dt>-F, --userfile</dt>
<dd>파일에서 사용자 데이터 읽기.</dd>
<dt>--public-speed</dt>
<dd>공용 포트 속도. 옵션: 0,10,100,1000,10000.</dd>
<dt>--private-speed</dt>
<dd>개인용 포트 속도. 옵션: 0,10,100,1000,10000.</dd>
</dl>

**예제**:
```
 bluemix sl vs edit 12345678 -D bluemix.net -H myapp --tag testcli --public-speed 1000
```
이 명령은 ID가 12345678인 가상 서버 인스턴스를 업데이트하고 해당 도메인을 "bluemix.net"으로, 호스트 이름을 "myapp"으로, 태그를 "testcli"로 설정합니다.

### bluemix sl vs list
{: #sl_vs_list}

계정의 가상 서버 인스턴스를 나열합니다.
```
   bluemix sl vs list [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-c, --cpu</dt>
<dd>CPU 코어 수.</dd>
<dt>-D, --domain</dt>
<dd>FQDN의 도메인 부분.</dd>
<dt>-d, --datacenter</dt>
<dd>데이터 센터의 짧은 이름.</dd>
<dt>-H, --hostname</dt>
<dd>FQDN의 호스트 부분. </dd>
<dt>-m, --memory</dt>
<dd>메모리(MB).</dd>
<dt>-n, --network</dt>
<dd>네트워크 포트 속도(Mbps).</dd>
<dt>--hourly</dt>
<dd>시간별 인스턴스만 표시.</dd>
<dt>--monthly</dt>
<dd>월별 인스턴스만 표시.</dd>
<dt>--tag</dt>
<dd>태그별 필터링(다중 발생 허용).</dd>
<dt>--sortby</dt>
<dd>정렬 기준 열, 옵션: id,hostname,domain,datacenter,cpu,memory,primary_ip,backend_ip. 기본값: hostname.</dd>
<dt>--columns</dt>
<dd>표시할 열, 옵션: guid,primary_ip,backend_ip,datacenter,action,power_state,created_by,tags. 기본값: id,hostname,primary_ip,backend_ip,datacenter,action.</dd>
</dl>

**예제**:
```
 bluemix sl vs list --domain bluemix.net --hourly --sortby memory
```
이 명령은 현재 계정의 시간별 청구되는 모든 가상 서버 인스턴스를 나열합니다. 도메인 기준 필터링은 "bluemix.net"과 동일하고 메모리별로 정렬합니다.



### bluemix sl vs pause
{: #sl_vs_pause}

활성 가상 서버 인스턴스를 일시정지합니다.
```
   bluemix sl vs pause IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs pause 12345678 -f
```
이 명령은 확인 요청 없이 ID가 12345678인 가상 서버 인스턴스를 일시정지합니다.



### bluemix sl vs power-off
{: #sl_vs_power_off}

활성 가상 서버 인스턴스의 전원을 끕니다.
```
   bluemix sl vs power-off IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--hard</dt>
<dd>하드 시스템 종료 수행.</dd>
<dt>--soft</dt>
<dd>소프트 시스템 종료 수행.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
   bluemix sl vs power-off 12345678 --soft
```
이 명령은 ID가 12345678인 가상 서버 인스턴스에 대해 소프트 전원 끄기를 수행합니다.

### bluemix sl vs power-on
{: #sl_vs_power_on}

가상 서버 인스턴스의 전원을 켭니다.
```
 bluemix sl vs power-on IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs power-on 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스에 대해 전원 켜기를 수행합니다.


### bluemix sl vs ready
{: #sl_vs_ready}

가상 서버 인스턴스가 사용할 준비가 되었는지 확인합니다.
```
 bluemix sl vs ready IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--wait</dt>
<dd>리턴하기 전에 가상 서버가 프로비저닝을 완료할 때까지 최대 X초 동안 대기.</dd>
</dl>

**예제**:
```
 bluemix sl vs ready 12345678 --wait 30
```
이 명령은 계속 사용할 준비가 되었는지 확인하기 위해 ID가 12345678인 가상 서버 인스턴스 상태를 확인하고 최대 30초 동안 대기합니다.

### bluemix sl vs reboot
{: #sl_vs_reboot}

활성 가상 서버 인스턴스를 다시 부팅합니다.
```
 bluemix sl vs reboot IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>--hard</dt>
<dd>하드 재부팅 수행.</dd>
<dt>--soft</dt>
<dd>하드 재부팅 수행.</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs reboot 12345678 --hard
```
이 명령은 ID가 12345678인 가상 서버 인스턴스에 대해 하드 재부팅을 수행합니다.



### bluemix sl vs reload
{: #sl_vs_reload}

가상 서버 인스턴스에 운영 체제를 다시 로드합니다.
```
 bluemix sl vs reload IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-i, --postinstall</dt>
<dd>다운로드할 사후 설치 스크립트.</dd>
<dt>--image</dt>
<dd>이미지 ID. 기본값은 현재 운영 체제를 사용하는 것입니다. </dd>
<dt>참조:</dt>
<dd>참조를 위한 'bluemix sl image list'.</dd>
<dt>-k, --key</dt>
<dd>루트 사용자에게 추가할 SSH 키 ID(다중 발생 허용).</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
   bluemix sl vs reload 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스에 대해 현재 운영 체제를 다시 로드합니다.
### bluemix sl vs rescue
{: #sl_vs_rescue}

가상 서버 인스턴스를 복구 이미지로 다시 부팅합니다.
```
 bluemix sl vs rescue IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs rescue 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스를 복구 이미지로 다시 부팅합니다.


### bluemix sl vs resume
{: #sl_vs_resume}

일시정지된 가상 서버 인스턴스를 재개합니다.
```
   bluemix sl vs resume IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs resume 12345678
```
이 명령은 ID가 12345678인 가상 서버 인스턴스를 재개합니다.


### bluemix sl vs upgrade
{: #sl_vs_upgrade}

가상 서버 인스턴스를 업그레이드합니다.
```
   bluemix sl vs upgrade IDENTIFIER [OPTIONS]
```

<strong>명령 옵션</strong>:

   <dl>
<dt>-c, --cpu</dt>
<dd>CPU 코어 수.</dd>
<dt>--private</dt>
<dd>CPU 코어는 전용 호스트 서버에 위치합니다. </dd>
<dt>-m, --memory</dt>
<dd>메모리(MB).</dd>
<dt>--network</dt>
<dd>네트워크 포트 속도(Mbps).</dd>
<dt>-f, --force</dt>
<dd>확인 없이 조작 강제 실행.</dd>
</dl>

**예제**:
```
 bluemix sl vs upgrade 12345678 -c 8 -m 8192 --network 1000
```
이 명령은 ID가 12345678인 가상 서버 인스턴스를 업그레이드하고 CPU 코어 수를 8로, 메모리를 8192M로, 네트워크 포트 속도를 1000Mbps로 설정합니다.

