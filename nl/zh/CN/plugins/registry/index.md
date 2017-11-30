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

{{site.data.keyword.registrylong}} CLI 是一个插件，用于为您的 {{site.data.keyword.Bluemix_notm}} 帐户管理您的注册表及其资源。
{: shortdesc}

**先决条件**
* 运行注册表命令之前，请先使用 `bx login` 命令登录到 {{site.data.keyword.Bluemix_notm}}，以生成访问令牌并对会话进行认证。

要了解如何使用 {{site.data.keyword.registrylong_notm}} CLI，请参阅[设置专用映像注册表](../../../services/Registry/index.html)。

<table summary="管理 {{site.data.keyword.registrylong_notm}}">
<caption>表 1. 用于在 {{site.data.keyword.Bluemix_notm}} 上管理 {{site.data.keyword.registrylong_notm}} 的命令</caption>
 <thead>
 <th colspan="5">用于管理注册表的命令</th>
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

返回有关对其运行命令的注册表 API 端点的详细信息。

```
bx cr api
```
{: codeblock}


## bx cr build
{: #bx_cr_build}

在 {{site.data.keyword.registrylong_notm}} 中构建 Docker 映像。

```
bx cr build [--no-cache] [--pull] [--quiet | -q] [--build-arg value ...] --tag value DIRECTORY
```
{: codeblock}

**参数**
<dl>
<dt>DIRECTORY</dt>
<dd>构建上下文的位置，其中包含 Dockerfile 和必备文件。</dd>
<dt>--no-cache</dt>
<dd>（可选）如果指定此项，那么不会在此构建中使用从先前构建中高速缓存的映像层。</dd>
<dt>--pull</dt>
<dd>（可选）如果指定此项，那么即使构建主机上已存在具有匹配标记的映像，也会拉取基本映像。</dd>
<dt>--quiet, -q</dt>
<dd>（可选）如果指定此项，那么除非发生错误，否则将禁止构建输出。</dd>
<dt> --build-arg value</dt>
<dd>（可选）以“KEY=VALUE”格式指定其他构建自变量。可以通过多次包含此参数来指定多个构建自变量。指定与 Dockerfile 中的键相匹配的 ARG 行时，构建自变量的值可用作环境变量。</dd>
<dt>--tag value, -t value</dt>
<dd>要构建的映像的全名，包括注册表 URL 和名称空间。</dd>
</dl>


## bx cr info
{: #bx_cr_info}

显示您登录到的注册表的名称和帐户。

```
bx cr info
```
{: codeblock}


## bx cr image-inspect
{: #bx_cr_image_inspect}

显示有关特定映像的详细信息。

```
bx cr image-inspect [--format FORMAT] IMAGE [IMAGE...]
```
{: codeblock}

**参数**

<dl>
<dt>--format FORMAT</dt>
<dd>（可选）使用 Go 模板设置输出元素的格式。有关更多信息，请参阅[查看有关映像的信息](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)。

</dd>
<dt>IMAGE</dt>
<dd>要检查的映像的完整注册表路径，格式为 `namespace/image:tag`。如果未在映像路径中指定标记，那么会检查标记为 `latest` 的映像。可以通过在命令中列出每个专用注册表路径（各路径之间用空格分隔）来检查多个映像。</dd>
</dl>


## bx cr image-list (bx cr images)
{: #bx_cr_image_list}

显示 {{site.data.keyword.Bluemix_notm}} 帐户中的所有映像。

```
 bx cr image-list [--no-trunc] [-q, --quiet] [--include-ibm] [--format FORMAT]
```
{: codeblock}

**参数**
<dl>
<dt>--no-trunc</dt>
<dd>（可选）不截断映像摘要。</dd>
<dt>-q, --quiet</dt>
<dd>（可选）列出每个映像，格式为：`repository:tag`。</dd>
<dt>--include-ibm</dt>
<dd>（可选）在输出中包含 {{site.data.keyword.IBM_notm}} 提供的公共映像。不使用此选项时，缺省情况下仅列出专用映像。</dd>
<dt>--format FORMAT</dt>
<dd>（可选）使用 Go 模板设置输出元素的格式。有关更多信息，请参阅[查看有关映像的信息](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)。

</dd>
</dl>


## bx cr image-rm
{: #bx_cr_image_rm}

从注册表中删除指定的一个或多个映像。

```
bx cr image-rm IMAGE [IMAGE...]
```
{: codeblock}

**参数**
<dl>
<dt>IMAGE</dt>
<dd>要除去的映像的完整注册表路径，格式为 `namespace/image:tag`。如果未在映像路径中指定标记，那么缺省情况下会删除标记为 `latest` 的映像。可以通过在命令中列出每个专用注册表路径（各路径之间用空格分隔）来删除多个映像。</dd>
</dl>


## bx cr login
{: #bx_cr_login}

此命令将对注册表运行 `docker login` 命令。必须运行 `docker login` 后，才能对注册表运行 `docker push` 或 `docker pull` 命令。无须运行此命令，即可运行其他 `bx cr` 命令。如果未安装 Docker，那么此命令会返回错误消息。

```
bx cr login
```
{: codeblock}


## bx cr namespace-add
{: #bx_cr_namespace_add}

向 {{site.data.keyword.Bluemix_notm}} 帐户添加名称空间。

```
bx cr namespace-add NAMESPACE
```
{: codeblock}

**参数**
<dl>
<dt>NAMESPACE</dt>
<dd>要添加的名称空间。名称空间在同一区域中的所有 {{site.data.keyword.Bluemix_notm}} 帐户之间必须唯一。</dd>
</dl>


## bx cr namespace-list (bx cr namespaces)
{: #bx_cr_namespace_list}

显示 {{site.data.keyword.Bluemix_notm}} 帐户拥有的所有名称空间。

```
bx cr namespace-list
```
{: codeblock}


## bx cr namespace-rm
{: #bx_cr_namespace_rm}

从 {{site.data.keyword.Bluemix_notm}} 帐户中除去名称空间。除去名称空间时，会删除此名称空间中的映像。

```
bx cr namespace-rm NAMESPACE
```
{: codeblock}

**参数**
<dl>
<dt>NAMESPACE</dt>
<dd>要除去的名称空间。</dd>
</dl>


## bx cr plan
{: #bx_cr_plan}

显示价格套餐。

```
bx cr plan
```
{: codeblock}


## bx cr plan-upgrade
{: #bx_cr_plan_upgrade}

升级到标准套餐。

有关套餐的信息，请参阅[注册表套餐](../../../services/Registry/registry_overview.html#registry_plans)。

```
bx cr plan-upgrade [PLAN]
```
{: codeblock}

**参数**
<dl>
<dt>套餐</dt>
<dd>要升级到的价格套餐的名称。如果未指定 PLAN，那么缺省值为 `standard`。</dd>
</dl>


## bx cr pricing
{: #bx_cr_pricing}

已除去此命令。您可以使用定价计算器来计算估算成本。请参阅[估算 {{site.data.keyword.registrylong_notm}} 的成本](../../../services/Registry/registry_overview.html#registry_plan_billing)。


## bx cr quota
{: #bx_cr_quota}

显示流量和存储的当前配额，以及那些配额的使用情况信息。

```
bx cr quota
```
{: codeblock}


## bx cr quota-set
{: #bx_cr_quota_set}

修改指定配额。

```
bx cr quota-set [--traffic VALUE] [--storage VALUE]
```
{: codeblock}

**参数**
<dl>
<dt>--traffic VALUE</dt>
<dd>（可选）将流量配额更改为指定的值（以兆字节为单位）。如果您无权设置流量或者您设置的值超出当前价格套餐，那么操作将失败。</dd>
<dt>--storage VALUE</dt>
<dd>（可选）将存储配额更改为指定的值（以兆字节为单位）。如果您无权设置存储配额或者您设置的值超出当前价格套餐，那么操作将失败。</dd>
</dl>


## bx cr token-add
{: #bx_cr_token_add}

添加可用于控制对注册表的访问权的令牌。

```
bx cr token-add [--description VALUE] [-q, --quiet] [--non-expiring] [--readwrite]
```

{: codeblock}


**参数**
<dl>
<dt>--description VALUE</dt>
<dd>（可选）指定作为令牌描述的值，在运行 `bx cr token-list` 时会显示此值。如果令牌是由 {{site.data.keyword.containerlong_notm}} 自动创建的，那么描述会设置为 Kubernetes 集群名称。在这种情况下，除去集群时，会自动除去令牌。</dd>
<dt>-q, --quiet</dt>
<dd>（可选）仅显示令牌，不包括任何周围的文本。</dd>
<dt>--non-expiring</dt>
<dd>（可选）创建具有不到期访问权的令牌。未设置此参数时，缺省情况下令牌的访问权在 24 小时后到期。</dd>
<dt>--readwrite</dt>
<dd>（可选）创建用于授予读和写访问权的令牌。不使用此选项时，缺省情况下访问权为只读。</dd>
</dl>


## bx cr token-get
{: #bx_cr_token_get}

在注册表中检索指定的令牌。

```
bx cr token-get TOKEN
```

{: codeblock}

**参数**
<dl>
<dt>TOKEN</dt>
<dd>（可选）要检索的令牌的唯一标识。</dd>
</dl>


## bx cr token-list (bx cr tokens)
{: #bx_cr_token_list}

显示针对您的 {{site.data.keyword.Bluemix_notm}} 帐户存在的所有令牌。

```
bx cr token-list --format FORMAT
```
{: codeblock}

**参数**
<dl>
<dt>--format FORMAT</dt>
<dd>（可选）使用 Go 模板设置输出元素的格式。有关更多信息，请参阅[查看有关映像的信息](../../../services/Registry/registry_cli_reference.html#registry_cli_listing)。

</dd>
</dl>

## bx cr token-rm
{: #bx_cr_token_rm}

除去指定的一个或多个令牌。

```
bx cr token-rm TOKEN [TOKEN...]
```
{: codeblock}

**参数**
<dl>
<dt>TOKEN</dt>
<dd>（可选）TOKEN 可以是令牌本身，也可以是令牌的唯一标识，如 `bx cr token-list` 中所示。可以指定多个令牌，令牌之间必须用一个空格分隔。</dd>
</dl>


## bx cr vulnerability-assessment (bx cr va)
{: #bx_cr_va}

查看映像的漏洞评估报告。

```
bx cr vulnerability-assessment IMAGE [IMAGE...]
```
{: codeblock}

**参数**
<dl>
<dt>IMAGE</dt>
<dd>您要获取其报告的映像的完整注册表路径，格式为 `namespace/image:tag`。报告将告知您映像是否具有任何已知的包漏洞。以下是支持的操作系统：

<ul>

<li>Alpine</li>
<li>CentOS</li>
<li>Debian</li>
<li>Red Hat Enterprise Linux (RHEL)</li>
<li>Ubuntu</li>
</ul>

有关更多信息，请参阅[使用漏洞顾问程序管理映像安全性](../../../services/va/va_index.html)。

</dd>

</dl>
