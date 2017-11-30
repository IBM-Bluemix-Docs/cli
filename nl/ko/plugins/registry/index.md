---



copyright:

  years: 2017

lastupdated: "2017-10-26"


---

{:codeblock: .codeblock}
{:shortdesc: .shortdesc}
{:tip: .tip}
{:new_window: target="_blank"}

# {{site.data.keyword.registrylong_notm}} CLI
{: #containerregcli}

{{site.data.keyword.registrylong}} CLI는 {{site.data.keyword.Bluemix_notm}} 계정의 레지스트리 및 관련 리소스를 관리하기 위한 플러그인입니다.
{: shortdesc}

**전제조건**
* 레지스트리 명령을 실행하기 전에 `bx login` 명령으로 {{site.data.keyword.Bluemix_notm}}에 로그인하여
액세스 토큰을 생성하고 세션을 인증하십시오.

{{site.data.keyword.registrylong_notm}} CLI 사용 방법에 대해 알아보려면 [개인용 이미지 레지스트리 설정](../../../services/Registry/index.html)을 참조하십시오.

<table summary="{{site.data.keyword.registrylong_notm}} 관리">
<caption>표 1. {{site.data.keyword.Bluemix_notm}}의 {{site.data.keyword.registrylong_notm}}를 관리하기 위한 명령
</caption>
 <thead>
 <th colspan="5">레지스트리 관리 명령</th>
 </thead>
 <tbody>
 <tr>
 <td>[bx cr api](#bx_cr_api)</td>
 <td>[bx cr build](#bx_cr_build)</td>
 <td>[bx cr info](#bx_cr_info)</td>
 <td>[bx cr image-inspect](#bx_cr_image_inspect)</td>
 <td>[bx cr image-list (bx cr images)](#bx_cr_image_list)</td>
 </tr>
 <tr>
 <td>[bx cr image-rm](#bx_cr_image_rm)</td>
 <td>[bx cr login](#bx_cr_login)</td>
 <td>[bx cr namespace-add](#bx_cr_namespace_add)</td>
 <td>[bx cr namespace-list (bx cr namespaces)](#bx_cr_namespace_list)</td>
 <td>[bx cr namespace-rm](#bx_cr_namespace_rm)</td>
 </tr>
 <tr>
 <td>[bx cr plan](#bx_cr_plan)</td>
 <td>[bx cr plan-upgrade](#bx_cr_plan_upgrade)</td>
 <td>[bx cr pricing](#bx_cr_pricing)</td>
 <td>[bx cr quota](#bx_cr_quota)</td>
 <td>[bx cr quota-set](#bx_cr_quota_set)</td>
 </tr>
 <tr>
 <td>[bx cr token-add](#bx_cr_token_add)</td>
 <td>[bx cr token-get](#bx_cr_token_get)</td>
 <td>[bx cr token-list (bx cr tokens)](#bx_cr_token_list)</td>
 <td>[bx cr token-rm](#bx_cr_token_rm)</td>
 <td>[bx cr vulnerability-assessment (bx cr va)](#bx_cr_va)</td>
 </tr>
 </tbody></table>



## bx cr api
{: #bx_cr_api}

명령을 실행할 레지스트리 API 엔드포인트에 대한 세부사항을 리턴합니다.

```
bx cr api
```
{: codeblock}


## bx cr build
{: #bx_cr_build}

{{site.data.keyword.registrylong_notm}}에 Docker 이미지를 빌드합니다.

```
bx cr build [--no-cache] [--pull] [--quiet | -q] [--build-arg value ...] --tag value DIRECTORY
```
{: codeblock}

**매개변수**
<dl>
<dt>DIRECTORY</dt>
<dd>빌드 컨텍스트의 위치이며, Dockerfile 및 전제조건 파일이 포함되어 있습니다. </dd>
<dt>--no-cache</dt>
<dd>(선택사항) 지정된 경우, 이전 빌드에서 캐시된 이미지 계층은 이 빌드에 사용되지 않습니다.</dd>
<dt>--pull</dt>
<dd>(선택사항) 지정된 경우, 일치하는 태그가 있는 이미지가 이미 빌드 호스트에 있더라도 기본 이미지를 가져옵니다.</dd>
<dt>--quiet, -q</dt>
<dd>(선택사항) 지정된 경우, 오류가 발생하지 않는 한 빌드 출력이 억제됩니다.</dd>
<dt> --build-arg value</dt>
<dd>(선택사항) 추가 빌드 인수를 'KEY=VALUE' 형식으로 지정하십시오. 이 매개변수를 여러 번 포함하여 복수의 빌드 인수를 지정할 수 있습니다. Dockerfile에서 키와 일치하는 ARG 행을 지정하는 경우 빌드 인수의 값은 환경 변수로 사용 가능합니다.</dd>
<dt>--tag value, -t value</dt>
<dd>빌드할 이미지의 전체 이름이며, 레지스트리 URL 및 네임스페이스가 포함됩니다.</dd>
</dl>


## bx cr info
{: #bx_cr_info}

로그인한 레지스트리의 이름과 계정을 표시합니다.

```
bx cr info
```
{: codeblock}


## bx cr image-inspect
{: #bx_cr_image_inspect}

특정 이미지에 대한 세부사항을 표시합니다. 

```
bx cr image-inspect [--format FORMAT] IMAGE [IMAGE...]
```
{: codeblock}

**매개변수**

<dl>
<dt>--format FORMAT</dt>
<dd>(선택사항) Go 템플리트를 사용하여 출력 요소를 형식화합니다.자세한 정보는 [이미지에 대한 정보 보기](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)를 참조하십시오.

</dd>
<dt>IMAGE</dt>
<dd>검사할 이미지에 대한 전체 레지스트리 경로이며, 형식은 `namespace/image:tag`입니다. 이미지 경로에 태그가 지정되지 않은 경우 `latest` 태그가 지정된 이미지를 검사합니다. 각 경로를 공백으로 구분하여 명령에 각 개인용 레지스트리 경로를 나열하여 여러 이미지를 검사할 수 있습니다.</dd>
</dl>


## bx cr image-list (bx cr images)
{: #bx_cr_image_list}

{{site.data.keyword.Bluemix_notm}} 계정의 모든 이미지를 표시합니다. 

```
 bx cr image-list [--no-trunc] [-q, --quiet] [--include-ibm] [--format FORMAT]
```
{: codeblock}

**매개변수**
<dl>
<dt>--no-trunc</dt>
<dd>(선택사항) 이미지 다이제스트를 자르지 않습니다. </dd>
<dt>-q, --quiet</dt>
<dd>(선택사항) 각 이미지가 `repository:tag` 형식으로 나열됩니다. </dd>
<dt>--include-ibm</dt>
<dd>(선택사항) 출력에 {{site.data.keyword.IBM_notm}} 제공 공용 이미지를 포함합니다. 이 옵션이 없으면 기본적으로 개인용 이미지만 나열됩니다. </dd>
<dt>--format FORMAT</dt>
<dd>(선택사항) Go 템플리트를 사용하여 출력 요소를 형식화합니다.자세한 정보는 [이미지에 대한 정보 보기](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)를 참조하십시오.

</dd>
</dl>


## bx cr image-rm
{: #bx_cr_image_rm}

레지스트리에서 하나 이상의 지정된 이미지를 삭제합니다. 

```
bx cr image-rm IMAGE [IMAGE...]
```
{: codeblock}

**매개변수**
<dl>
<dt>IMAGE</dt>
<dd>제거할 이미지에 대한 전체 레지스트리 경로이며, 형식은 `namespace/image:tag`입니다. 이미지 경로에 태그가 지정되지 않은 경우 `latest` 태그가 지정된 이미지가 기본적으로 삭제됩니다. 각 경로를 공백으로 구분하여 명령에 각 개인용 레지스트리 경로를 나열하여 여러 이미지를 삭제할 수 있습니다.</dd>
</dl>


## bx cr login
{: #bx_cr_login}

이 명령은 레지스트리에 대해 `docker login` 명령을 실행합니다. 레지스트리에 대해 `docker push` 또는 `docker pull` 명령을 실행할 수 있으려면 `docker login` 명령이 필요합니다. 이 명령은 다른 `bx cr` 명령을 실행하는 데 필요하지 않습니다. Docker가 설치되지 않은 경우 이 명령은 오류 메시지를 리턴합니다.

```
bx cr login
```
{: codeblock}


## bx cr namespace-add
{: #bx_cr_namespace_add}

{{site.data.keyword.Bluemix_notm}} 계정에 네임스페이스를 추가합니다. 

```
bx cr namespace-add NAMESPACE
```
{: codeblock}

**매개변수**
<dl>
<dt>NAMESPACE</dt>
<dd>추가하려는 네임스페이스입니다. 네임스페이스는 동일 지역의 모든 {{site.data.keyword.Bluemix_notm}} 계정에서 고유해야 합니다. </dd>
</dl>


## bx cr namespace-list (bx cr namespaces)
{: #bx_cr_namespace_list}

{{site.data.keyword.Bluemix_notm}} 계정이 소유하는 모든 네임스페이스를 표시합니다. 

```
bx cr namespace-list
```
{: codeblock}


## bx cr namespace-rm
{: #bx_cr_namespace_rm}

{{site.data.keyword.Bluemix_notm}} 계정에서 네임스페이스를 제거합니다. 이 네임스페이스의 이미지는 네임스페이스가 제거될 때 삭제됩니다. 

```
bx cr namespace-rm NAMESPACE
```
{: codeblock}

**매개변수**
<dl>
<dt>NAMESPACE</dt>
<dd>제거하려는 네임스페이스입니다. </dd>
</dl>


## bx cr plan
{: #bx_cr_plan}

가격 책정 플랜을 표시합니다. 

```
bx cr plan
```
{: codeblock}


## bx cr plan-upgrade
{: #bx_cr_plan_upgrade}

표준 플랜으로 업그레이드합니다.

플랜에 대한 정보는 [레지스트리 플랜](../../../services/Registry/registry_overview.html#registry_plans)을 참조하십시오.

```
bx cr plan-upgrade [PLAN]
```
{: codeblock}

**매개변수**
<dl>
<dt>PLAN</dt>
<dd>업그레이드될 대상 가격 책정 플랜의 이름입니다. PLAN이 지정되지 않는 경우 기본값은 `standard`입니다.</dd>
</dl>


## bx cr pricing
{: #bx_cr_pricing}

이 명령은 제거되었습니다. 가격 책정 계산기를 사용하여 예상 비용을 계산할 수 있습니다. [{{site.data.keyword.registrylong_notm}}의 비용 추정](../../../services/Registry/registry_overview.html#registry_plan_billing)을 참조하십시오.


## bx cr quota
{: #bx_cr_quota}

트래픽 및 스토리지에 대한 현재 할당량과, 이러한 할당량의 사용량 정보를 표시합니다. 

```
bx cr quota
```
{: codeblock}


## bx cr quota-set
{: #bx_cr_quota_set}

지정된 할당량을 수정합니다. 

```
bx cr quota-set [--traffic VALUE] [--storage VALUE]
```
{: codeblock}

**매개변수**
<dl>
<dt>--traffic VALUE</dt>
<dd>(선택사항) 트래픽 할당량을 MB 단위의 지정된 값으로 변경합니다. 이 오퍼레이션은 사용자가 트래픽을 설정할 수 있도록 권한 부여되지 않았거나 현재 가격 책정 플랜을 초과하는 값을 설정하면 실패합니다. </dd>
<dt>--storage VALUE</dt>
<dd>(선택사항) 스토리지 할당량을 MB 단위의 지정된 값으로 변경합니다. 이 오퍼레이션은 사용자가 스토리지를 설정할 수 있도록 권한 부여되지 않았거나 현재 가격 책정 플랜을 초과하는 값을 설정하면 실패합니다. </dd>
</dl>


## bx cr token-add
{: #bx_cr_token_add}

레지스트리에 대한 액세스를 제어하는 데 사용할 수 있는 토큰을 추가합니다. 

```
bx cr token-add [--description VALUE] [-q, --quiet] [--non-expiring] [--readwrite]
```

{: codeblock}


**매개변수**
<dl>
<dt>--description VALUE</dt>
<dd>(선택사항) `bx cr token-list`를 실행할 때 표시되는 토큰에 대한 설명으로서 값을 지정합니다. 토큰이 {{site.data.keyword.containerlong_notm}}에 의해 자동으로 작성되는 경우에는 설명이 Kubernetes 클러스터 이름으로 설정됩니다. 이 경우에 토큰은 클러스터가 제거될 때 자동으로 제거됩니다. </dd>
<dt>-q, --quiet</dt>
<dd>(선택사항) 주변 텍스트 없이 토큰만 표시합니다. </dd>
<dt>--non-expiring</dt>
<dd>(선택사항) 만료되지 않는 액세스 권한으로 토큰을 작성합니다. 이 매개변수 설정이 없는 경우 기본적으로 토큰의 액세스 권한이 24시간 후에 만료됩니다. </dd>
<dt>--readwrite</dt>
<dd>(선택사항) 읽기/쓰기 액세스 권한을 부여하는 토큰을 작성합니다. 이 옵션이 없는 경우 기본적으로 액세스 권한은 읽기 전용입니다. </dd>
</dl>


## bx cr token-get
{: #bx_cr_token_get}

지정된 토큰을 레지스트리에서 검색합니다. 

```
bx cr token-get TOKEN
```

{: codeblock}

**매개변수**
<dl>
<dt>TOKEN</dt>
<dd>(선택사항) 검색할 토큰의 고유 ID입니다. </dd>
</dl>


## bx cr token-list (bx cr tokens)
{: #bx_cr_token_list}

{{site.data.keyword.Bluemix_notm}} 계정에 대해 존재하는 모든 토큰을 표시합니다. 

```
bx cr token-list --format FORMAT
```
{: codeblock}

**매개변수**
<dl>
<dt>--format FORMAT</dt>
<dd>(선택사항) Go 템플리트를 사용하여 출력 요소를 형식화합니다.자세한 정보는 [이미지에 대한 정보 보기](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)를 참조하십시오.

</dd>
</dl>

## bx cr token-rm
{: #bx_cr_token_rm}

지정된 토큰을 하나 이상 제거합니다. 

```
bx cr token-rm TOKEN [TOKEN...]
```
{: codeblock}

**매개변수**
<dl>
<dt>TOKEN</dt>
<dd>(선택사항) TOKEN은 `bx cr token-list`에 표시되는 토큰의 고유 ID 또는 토큰 자체일 수 있습니다. 여러 개의 토큰을 지정할 수 있으며, 이는 공백으로 분리되어야 합니다. </dd>
</dl>


## bx cr vulnerability-assessment (bx cr va)
{: #bx_cr_va}

이미지에 대한 취약성 평가 보고서를 봅니다. 

```
bx cr vulnerability-assessment IMAGE [IMAGE...]
```
{: codeblock}

**매개변수**
<dl>
<dt>IMAGE</dt>
<dd>보고서를 가져오려는 이미지에 대한 `namespace/image:tag` 형식의 전체 레지스트리 경로입니다. 이 보고서는 이미지에 알려진 패키지 취약점이 있는지 알려줍니다. 다음 운영 체제가 지원됩니다.

<ul>

<li>Alpine</li>
<li>CentOS</li>
<li>Debian</li>
<li>Red Hat Enterprise Linux(RHEL)</li>
<li>Ubuntu</li>
</ul>

자세한 정보는 [취약성 관리자로 이미지 보안 관리](../../../services/va/va_index.html)를 참조하십시오. 

</dd>

</dl>
