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

A CLI do {{site.data.keyword.registrylong}} é um plug-in para gerenciar seu registro e seus recursos para sua conta. {{site.data.keyword.Bluemix_notm}}
{: shortdesc}

**Pré-requisitos**
* Antes de executar os comandos de registro, efetue login no {{site.data.keyword.Bluemix_notm}} com o comando `bx login` para gerar um token de acesso e autenticar sua sessão.

Para descobrir sobre como usar a CLI do {{site.data.keyword.registrylong_notm}}, veja [Configurando um registro de imagens privado](../../../services/Registry/index.html).

<table summary="Gerenciar {{site.data.keyword.registrylong_notm}}y">
<caption>Tabela 1. Comandos para gerenciar o {{site.data.keyword.registrylong_notm}} no {{site.data.keyword.Bluemix_notm}}
</caption>
 <thead>
 <th colspan="5">Comandos para gerenciar o registro</th>
 </thead>
 <tbody>
 <tr>
 <td>[bx cr api](#bx_cr_api)</td>
 <td>[bx cr build](#bx_cr_build)</td>
 <td>[bx cr info](#bx_cr_info)</td>
 <td>[bx cr image-inspect](#bx_cr_image_inspect)</td>
 <td>[bx cr image-list (imagens bx cr)](#bx_cr_image_list)</td>
 </tr>
 <tr>
 <td>[bx cr image-rm](#bx_cr_image_rm)</td>
 <td>[bx cr login
](#bx_cr_login)</td>
 <td>[bx cr namespace-add](#bx_cr_namespace_add)</td>
 <td>[bx cr namespace-list (namespaces bx cr)](#bx_cr_namespace_list)</td>
 <td>[bx cr namespace-rm](#bx_cr_namespace_rm)</td>
 </tr>
 <tr>
 <td>[bx cr plano](#bx_cr_plan)</td>
 <td>[bx cr plano de upgrade](#bx_cr_plan_upgrade)</td>
 <td>[bx cr pricing](#bx_cr_pricing)</td>
 <td>[bx cr cota](#bx_cr_quota)</td>
 <td>[bx cr de cota configurado](#bx_cr_quota_set)</td>
 </tr>
 <tr>
 <td>[bx cr token-add](#bx_cr_token_add)</td>
 <td>[bx cr token-get](#bx_cr_token_get)</td>
 <td>[bx cr token-list (tokens bx cr)](#bx_cr_token_list)</td>
 <td>[bx cr token-rm](#bx_cr_token_rm)</td>
 <td>[Bx cr vulnerabilidade de avaliação (que va bx)](#bx_cr_va)</td>
 </tr>
 </tbody></table>



## bx cr api
{: #bx_cr_api}

Retorna os detalhes sobre o terminal de API de registro com relação ao qual os comandos são executados.

```
bx cr api
```
{: codeblock}


## bx cr build
{: #bx_cr_build}

Constrói uma imagem do Docker no {{site.data.keyword.registrylong_notm}}.

```
bx cr build [--no-cache] [--pull] [--quiet | -q] [--build-arg value ...] --tag value DIRECTORY
```
{: codeblock}

**Parâmetros**
<dl>
<dt>DIRECTORY</dt>
<dd>O local de seu contexto de compilação, que contém o Dockerfile e os arquivos de pré-requisito.</dd>
<dt>--no-cache</dt>
<dd>(Opcional) Se especificado, camadas de imagem em cache de construções anteriores não serão usadas nesta compilação.</dd>
<dt>--pull</dt>
<dd>(Opcional) Se especificado, a imagem base será puxada mesmo se uma imagem com uma tag de correspondência já existir no host de construção.</dd>
<dt>--quiet, -q</dt>
<dd>(Opcional) Se especificado, a saída de construção será suprimida, a menos que ocorra um erro.</dd>
<dt> --build-arg value</dt>
<dd>(Opcional) Especifique um argumento de construção adicional no formato 'KEY=VALUE'. Múltiplos argumentos de compilação podem ser especificados, incluindo este parâmetro, múltiplas vezes. O valor de argumentos de compilação fica disponível como variáveis de ambiente quando você especifica uma linha ARG que corresponde à chave em seu Dockerfile.</dd>
<dt>--tag value, -t value</dt>
<dd>O nome completo da imagem que você deseja construir, que inclui a URL do registro e o namespace.</dd>
</dl>


## bx cr info
{: #bx_cr_info}

Exibe o nome e a conta do registro ao qual você está conectado.

```
bx cr info
```
{: codeblock}


## bx cr image-inspect
{: #bx_cr_image_inspect}

Exibe detalhes sobre uma imagem específica.

```
bx cr image-inspect [--format FORMAT] IMAGE [IMAGE...]
```
{: codeblock}

**Parâmetros**

<dl>
<dt>--format FORMAT</dt>
<dd>(Opcional) Formata os elementos de saída usando um modelo Go.

Para obter mais informações, veja [Visualizando informações sobre as imagens](../../../services/Registry/registry_cli_reference.html#registry_cli_listing).

</dd>
<dt>IMAGE</dt>
<dd>O caminho de registro completo para a imagem que você deseja inspecionar, que está no formato `namespace/image:tag`. Se uma tag não for especificada no caminho da imagem, a imagem identificada como `latest` será inspecionada. É possível inspecionar múltiplas imagens listando cada caminho de registro privado no comando com um espaço entre cada caminho.</dd>
</dl>


## bx cr image-list (imagens bx cr)
{: #bx_cr_image_list}

Exibe todas as imagens na conta do {{site.data.keyword.Bluemix_notm}}.

```
 bx cr image-list [--no-trunc] [-q, --quiet] [--include-ibm] [--format FORMAT]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>--no-trunc</dt>
<dd>(Opcional) Não truncar as compilações de imagem.</dd>
<dt>-q, --quiet</dt>
<dd>(Opcional) Cada imagem é listada no formato: `repository:tag`.</dd>
<dt>--include-ibm</dt>
<dd>(Opcional) Inclui imagens públicas fornecidas pelo {{site.data.keyword.IBM_notm}} na saída. Sem essa opção, somente imagens privadas serão listadas, por padrão.</dd>
<dt>--format FORMAT</dt>
<dd>(Opcional) Formata os elementos de saída usando um modelo Go.

Para obter mais informações, veja [Visualizando informações sobre as imagens](../../../services/Registry/registry_cli_reference.html#registry_cli_listing).

</dd>
</dl>


## bx cr image-rm
{: #bx_cr_image_rm}

Exclui uma ou mais imagens especificadas do seu registro.

```
bx cr image-rm IMAGE [IMAGE...]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>IMAGE</dt>
<dd>O caminho de registro completo para a imagem que você deseja remover, no formato `namespace/image:tag`. Se uma tag não for especificada no caminho da imagem, a imagem identificada como `latest` será excluída por padrão. É possível excluir múltiplas imagens listando cada caminho de registro privado no comando com um espaço entre cada caminho.</dd>
</dl>


## bx cr login
{: #bx_cr_login}

Esse comando executa o comando `docker login` no registro. O comando `docker login` é necessário para poder executar os comandos `docker push` ou `docker pull` para o registro. Esse comando não é necessário para executar outros comandos `bx cr`. Se o Docker não estiver instalado, esse comando retornará uma mensagem de erro.

```
bx cr login
```
{: codeblock}


## bx cr namespace-add
{: #bx_cr_namespace_add}

Inclui um namespace em sua conta do {{site.data.keyword.Bluemix_notm}}.

```
bx cr namespace-add NAMESPACE
```
{: codeblock}

**Parâmetros**
<dl>
<dt>NAMESPACE</dt>
<dd>O namespace que deseja incluir. O namespace deve ser exclusivo em todas as contas do {{site.data.keyword.Bluemix_notm}} na mesma região.</dd>
</dl>


## bx cr namespace-list (namespaces bx cr)
{: #bx_cr_namespace_list}

Exibe todos os namespaces pertencentes à sua conta do {{site.data.keyword.Bluemix_notm}}.

```
bx cr namespace-list
```
{: codeblock}


## bx cr namespace-rm
{: #bx_cr_namespace_rm}

Remove um namespace de sua conta do {{site.data.keyword.Bluemix_notm}}. As imagens nesse namespace são excluídas quando o namespace é removido.

```
bx cr namespace-rm NAMESPACE
```
{: codeblock}

**Parâmetros**
<dl>
<dt>NAMESPACE</dt>
<dd>O namespace que deseja remover.</dd>
</dl>


## Cr bx plano
{: #bx_cr_plan}

Exibe seu plano de precificação.

```
Cr bx plano
```
{: codeblock}


## bx cr plan-upgrade
{: #bx_cr_plan_upgrade}

Faz upgrade para o plano padrão.

Para obter informações sobre planos, veja [Planos de registro](../../../services/Registry/registry_overview.html#registry_plans).

```
bx cr plan-upgrade [PLAN]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>PLANO</dt>
<dd>O nome do plano de precificação para o qual você deseja fazer upgrade. Se PLAN não for especificado, o padrão será `standard`.</dd>
</dl>


## bx cr pricing
{: #bx_cr_pricing}

O comando foi removido. É possível usar a calculadora de precificação para calcular o custo estimado, consulte [Estimando custos para o {{site.data.keyword.registrylong_notm}}](../../../services/Registry/registry_overview.html#registry_plan_billing).


## Cota cr bx
{: #bx_cr_quota}

Exibe suas cotas atuais para tráfego e armazenamento e informações de uso com relação a essas cotas.

```
Cota cr bx
```
{: codeblock}


## -cr bx conjunto de cota
{: #bx_cr_quota_set}

Modifique a cota especificada.

```
bx cr quota-set [--traffic VALUE] [--storage VALUE]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>-- tráfego VALUE</dt>
<dd>(Opcional) Muda sua cota de tráfego para o valor especificado em megabytes. A operação falhará se você não estiver autorizado a configurar o tráfego ou se configurar um valor que exceda o seu plano de precificação atual.</dd>
<dt>-- armazenamento VALUE</dt>
<dd>(Opcional) Muda sua cota de armazenamento para o valor especificado em megabytes. A operação falhará se você não estiver autorizado a configurar cotas de armazenamento ou se configurar um valor que exceda o seu plano de precificação atual.</dd>
</dl>


## bx cr token-add
{: #bx_cr_token_add}

Inclui um token que pode ser usado para controlar o acesso a um registro.

```
bx cr token-add [--description VALUE] [-q, --quiet] [--non-expiring] [--readwrite]
```

{: codeblock}


**Parâmetros**
<dl>
<dt>--description VALUE</dt>
<dd>(Opcional) Especifica o valor como uma descrição para o token, que é exibida quando você executa `bx cr token-list`. Se o seu token for criado automaticamente pelo {{site.data.keyword.containerlong_notm}}, a descrição será configurada para o nome do Cluster do Kubernetes. Nesse caso, o token é removido automaticamente quando o cluster é removido.</dd>
<dt>-q, --quiet</dt>
<dd>(Opcional) Exibe o token somente, sem nenhum texto circundante.</dd>
<dt>--non-expiring</dt>
<dd>(Opcional) Cria um token com acesso que não expira. Sem esse conjunto de parâmetros, o acesso por meio de um token expirará após 24 horas, por padrão.</dd>
<dt>--readwrite</dt>
<dd>(Opcional) Cria um token que concede acesso de leitura e gravação. Sem essa opção, o acesso será somente leitura, por padrão.</dd>
</dl>


## bx cr token-get
{: #bx_cr_token_get}

Recuperar o token especificado do registro.

```
bx cr token-get TOKEN
```

{: codeblock}

**Parâmetros**
<dl>
<dt>TOKEN</dt>
<dd>(Opcional) O identificador exclusivo do token que você deseja recuperar.</dd>
</dl>


## bx cr token-list (tokens bx cr)
{: #bx_cr_token_list}

Exibe todos os tokens que existem para sua conta do {{site.data.keyword.Bluemix_notm}}.

```
bx cr token-list --format FORMAT
```
{: codeblock}

**Parâmetros**
<dl>
<dt>--format FORMAT</dt>
<dd>(Opcional) Formata os elementos de saída usando um modelo Go.

Para obter mais informações, veja [Visualizando informações sobre as imagens](../../../services/Registry/registry_cli_reference.html#registry_cli_listing).

</dd>
</dl>

## bx cr token-rm
{: #bx_cr_token_rm}

Remover um ou mais tokens especificados.

```
bx cr token-rm TOKEN [TOKEN...]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>TOKEN</dt>
<dd>(Opcional) TOKEN pode ser o próprio token ou o identificador exclusivo do token, conforme mostrado em `bx cr token-list`. É possível especificar múltiplos tokens e devem ser separados por um espaço.</dd>
</dl>


## Bx cr vulnerabilidade de avaliação (que va bx)
{: #bx_cr_va}

Visualize um relatório de avaliação de vulnerabilidade para uma imagem.

```
Bx cr vulnerabilidade de avaliação IMAGEM [ IMAGEM ... ]
```
{: codeblock}

**Parâmetros**
<dl>
<dt>IMAGE</dt>
<dd>O caminho de registro completo, no formato `namespace/image:tag`, para a imagem da qual você deseja obter um relatório. O relatório indica se a imagem em quaisquer vulnerabilidades de pacote conhecidas. Os seguintes sistemas operacionais são suportados:

<ul>

<li>Alpine</li>
<li>CentOS</li>
<li>Debian</li>
<li>Red Hat Enterprise Linux (RHEL)</li>
<li>Ubuntu</li>
</ul>

Para obter mais informações, consulte [Gerenciando a segurança de imagens com o Vulnerability Advisor](../../../services/va/va_index.html).

</dd>

</dl>
