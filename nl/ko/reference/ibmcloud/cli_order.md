---

copyright:

  years: 2018


lastupdated: "2018-11-05"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:tip: .tip}

# 주문

<table summary="해당 명령에 대한 자세한 정보를 제공하는 링크가 있는 알파벳순으로 정렬된 일반 {{site.data.keyword.BluSoftlayer_notm}} 인프라 명령">
 <caption>표 1. {{site.data.keyword.BluSoftlayer_notm}} 인프라 주문</caption>
 <thead>
 <th colspan="6">{{site.data.keyword.BluSoftlayer_notm}} 인프라 주문</th>
 </thead>
 <tbody>
 <tr>
  <td>[ibmcloud sl order package-locations](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_category_list)</td>
  <td>[ibmcloud sl order item-list](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_item_list)</td>
  <td>[ibmcloud sl order package-locations](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_package_locations)</td>
  <td>[ibmcloud sl order place](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_place)</td>
  <td>[ibmcloud sl order place-quote](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_place_quote)</td>
  <td>[ibmcloud sl order preset-list](/docs/cli/reference/ibmcloud/cli_order.html#sl_order_preset_list)</td>
 </tr>
 </tbody>
</table>

## ibmcloud sl order package-locations
{: #sl_order_category_list}

패키지 카테고리 나열
```
ibmcloud sl order package-locations [OPTIONS] PACKAGE_KEYNAME
```

<strong>명령 옵션</strong>:
<dl>
<dt>--required</dt>
<dd>패키지의 필수 카테고리만 나열</dd>
</dl>

**예제**:
```
ibmcloud sl order package-locations BARE_METAL_SERVER
```
이 명령을 통해서는 Bare Metal Server의 카테고리를 나열합니다.

## ibmcloud sl order item-list
{: #sl_order_item_list}

주문에 사용된 패키지 항목 나열
```
ibmcloud sl order item-list [OPTIONS] PACKAGE_KEYNAME
```

<strong>명령 옵션</strong>:
<dl>
<dt>--keyword</dt>
<dd>항목 이름을 필터링하는 데 사용한 단어(또는 문자열)</dd>
<dt>--category</dt>
<dd>기준에 따라 항목을 필터링하는 카테고리 코드</dd>
</dl>

**예제**:
```
ibmcloud sl order item-list CLOUD_SERVER
```
이 명령을 통해서는 VSI 패키지의 모든 항목을 나열합니다.

## ibmcloud sl order package-locations
{: #sl_order_package_locations}

패키지를 주문할 수 있는 데이터 센터 나열
```
ibmcloud sl order package-locations PACKAGE_KEYNAME
```

## ibmcloud sl order place
{: #sl_order_place}

주문하거나 주문 확인
```
ibmcloud sl order place PACKAGE_KEYNAME LOCATION ORDER_ITEM1,ORDER_ITEM2,ORDER_ITEM3,ORDER_ITEM4... [OPTIONS]
```

<strong>명령 옵션</strong>:
<dl>
<dt>--preset</dt>
<dd>주문 사전 설정(패키지에서 필요한 경우)</dd>
<dt>--verify</dt>
<dd>실제로 주문하지 않고 주문을 확인만 하는지 나타내는 플래그</dd>
<dt>--billing</dt>
<dd>청구 비율 [시간별|월별], [기본값: 시간별]</dd>
<dt>--complex-type</dt>
<dd>주문의 복합 유형입니다. 이 유형은 일반적으로 'SoftLayer_Container_Product_Order_'로 시작합니다.</dd>
<dt>--extras</dt>
<dd>주문과 함께 보내야 하는 추가 데이터를 나타내는 JSON 문자열</dd>
<dt>-f, --force</dt>
<dd>확인하지 않고 조작 강제 실행</dd>
</dl>

**예제**:
```
ibmcloud sl order place CLOUD_SERVER DALLAS13 GUEST_CORES_4,RAM_16_GB,REBOOT_REMOTE_CONSOLE,1_GBPS_PUBLIC_PRIVATE_NETWORK_UPLINKS,BANDWIDTH_0_GB_2,1_IP_ADDRESS,GUEST_DISK_100_GB_SAN,OS_UBUNTU_16_04_LTS_XENIAL_XERUS_MINIMAL_64_BIT_FOR_VSI,MONITORING_HOST_PING,NOTIFICATION_EMAIL_AND_TICKET,AUTOMATED_NOTIFICATION,UNLIMITED_SSL_VPN_USERS_1_PPTP_VPN_USER_PER_ACCOUNT,NESSUS_VULNERABILITY_ASSESSMENT_REPORTING --billing hourly --extras '{"virtualGuests": [{"hostname": "test", "domain": "softlayer.com"}]}' --complex-type SoftLayer_Container_Product_Order_Virtual_Guest
```
이 명령을 통해 4 CPU, 16GB RAM, 100GB SAN 디스크, Ubuntu 16.04 및 dal13의 1Gbps 공용 및 개인용 업링크가 포함된 시간별 VSI를 주문합니다.

## ibmcloud sl order place-quote
{: #sl_order_place_quote}

견적내기
```
ibmcloud sl order place-quote PACKAGE_KEYNAME LOCATION ORDER_ITEM1,ORDER_ITEM2,ORDER_ITEM3,ORDER_ITEM4... [OPTIONS]
```

<strong>명령 옵션</strong>:
<dl>
<dt>--preset</dt>
<dd>주문 사전 설정(패키지에서 필요한 경우)</dd>
<dt>--verify</dt>
<dd>실제로 주문하지 않고 주문을 확인만 하는지 나타내는 플래그</dd>
<dt>--billing</dt>
<dd>청구 비율 [시간별|월별], [기본값: 시간별]</dd>
<dt>--complex-type</dt>
<dd>주문의 복합 유형입니다. 이 유형은 일반적으로 'SoftLayer_Container_Product_Order_'로 시작합니다.</dd>
<dt>--extras</dt>
<dd>주문과 함께 보내야 하는 추가 데이터를 나타내는 JSON 문자열</dd>
<dt>-f, --force</dt>
<dd>확인하지 않고 조작 강제 실행</dd>
</dl>

**예제**:
```
sl order place-quote CLOUD_SERVER DALLAS13 GUEST_CORES_4,RAM_16_GB,REBOOT_REMOTE_CONSOLE,1_GBPS_PUBLIC_PRIVATE_NETWORK_UPLINKS,BANDWIDTH_0_GB_2,1_IP_ADDRESS,GUEST_DISK_100_GB_SAN,OS_UBUNTU_16_04_LTS_XENIAL_XERUS_MINIMAL_64_BIT_FOR_VSI,MONITORING_HOST_PING,NOTIFICATION_EMAIL_AND_TICKET,AUTOMATED_NOTIFICATION,UNLIMITED_SSL_VPN_USERS_1_PPTP_VPN_USER_PER_ACCOUNT,NESSUS_VULNERABILITY_ASSESSMENT_REPORTING --extras '{"virtualGuests": [{"hostname": "test", "domain": "softlayer.com"}]}' --complex-type SoftLayer_Container_Product_Order_Virtual_Guest --name "foobar" --send-email
```
이 명령을 통해 4 CPU, 16GB RAM, 100GB SAN 디스크, Ubuntu 16.04 및 dal13의 1Gbps 공용 및 개인용 업링크가 포함된 VSI의 견적을 냅니다.

## ibmcloud sl order preset-list
{: #sl_order_preset_list}

패키지 사전 설정 나열
```
ibmcloud sl order preset-list [OPTIONS] PACKAGE_KEYNAME
```

<strong>명령 옵션</strong>:
<dl>
<dt>--keyword</dt>
<dd>항목 이름을 필터링하는 데 사용한 단어(또는 문자열)</dd>
</dl>

**예제**:
```
ibmcloud sl order preset-list BARE_METAL_SERVER
```
이 명령을 통해서는 Bare Metal Server의 사전 설정을 나열합니다.