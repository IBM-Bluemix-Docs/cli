---

copyright:
  years: 2020
lastupdated: "2020-08-03"

keywords: cli, quotes, quotation, quotation marks, strings, double quotation mark, single quotation mark, double quote, single quote, json, string

subcollection: cli

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:pre: .pre}

# Using quotation marks with strings in {{site.data.keyword.cloud_notm}} CLI
{: #quote-strings}

Depending on the operating system that you're running {{site.data.keyword.cloud}} Command Line Interface on, you use either single or double quotation marks in the command. Linux&trade;, macOS, the Windows&trade; command prompt (`cmd.exe`), and Windows&trade; PowerShell have different quotation-escaping requirements when you run commands. This difference impacts how you pass strings on the {{site.data.keyword.cloud}} command line, including JSON content.
{: shortdesc}

For Linux, macOS, or PowerShell, use single quotation marks ('). For the Windows command prompt, use double quotation marks ("). A JSON string requires double quotation marks around each name and value in the JSON structure. For more information, see the following examples.

## Windows command prompt
{: #quote-windows}

For a Windows command prompt, use double quotation marks to surround the JSON data structure. Additionally, you must escape each double quotation mark that is inside the JSON structure by using a backslash before each double quotation mark.

```
ibmcloud resource service-instance-create my-service-instance db-service lite us-south -p "{\"units\":1}"
```
{: codeblock}

## Linux or macOS
{: #quote-linux}

For Linux or macOS, use single quotation marks to surround the JSON data structure.

```
ibmcloud resource service-instance-create my-service-instance db-service lite us-south -p '{"units":1}'
```
{: codeblock}

## Windows PowerShell
{: #quote-powershell}

For PowerShell, use single quotation marks to surround the JSON data structure. Additionally, you must escape each double quotation mark that is inside the JSON structure by using a backslash before each double quotation mark.

```
  ibmcloud resource service-instance-create my-service-instance db-service lite us-south -p '{\"units\":1}'
```
{: codeblock}
