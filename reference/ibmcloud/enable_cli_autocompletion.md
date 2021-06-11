---

copyright:
  years: 2018, 2020
lastupdated: "2020-08-03"

keywords: cli, shell autocompletion, bash, linux shell, macos shell, autocompletion, autocompletion support, shell

subcollection: cli

---

{:codeblock: .codeblock} 
{:shortdesc: .shortdesc}
{:tip: .tip}

# Enabling shell autocompletion for {{site.data.keyword.cloud_notm}} CLI (Linux and macOS only)
{: #shell-autocomplete}

Starting from version `0.7.0`, the {{site.data.keyword.cloud}} Command Line Interface installers don't enable shell autocompletion automatically. To have the autocompletion support, you need to manually enable it. The autocompletion scripts are installed in the following locations:

* `Bash` autocompletion: `/usr/local/ibmcloud/autocomplete/bash_autocomplete`
* `Zsh` autocompletion: `/usr/local/ibmcloud/autocomplete/zsh_autocomplete`

## Enabling autocompletion for Linux
{: #shell-autocomplete-linux}

* If you're using `Bash`, add 
`[[ -f /usr/local/ibmcloud/autocomplete/bash_autocomplete ]] && source /usr/local/ibmcloud/autocomplete/bash_autocomplete` into one of the following files:

  * For Login shell: `~/.bash_profile`
  * For Non-login shell: `~/.bashrc`
  
* If you're using `Zsh`: add 
`source /usr/local/ibmcloud/autocomplete/zsh_autocomplete` into `~/.zshrc`.

## Enabling autocompletion support for macOS
{: #shell-autocomplete-macos}

* If you're using `Bash`: add 
`source /usr/local/ibmcloud/autocomplete/bash_autocomplete` into `~/.bash_profile`.

* If you're using `Zsh`: add 
`source /usr/local/ibmcloud/autocomplete/zsh_autocomplete` into `~/.zshrc`.
