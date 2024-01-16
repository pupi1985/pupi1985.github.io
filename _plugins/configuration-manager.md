---
title: Configuration Manager
subtitle: Allows users to import and export Q2A configuration
description: Allows users to import and export Q2A configuration
product_code: COMA
layout: product
image: /img/COMA-settings.png
price: 0
wiki_url: https://github.com/pupi1985/q2a-pupi-coma
download_url: https://github.com/pupi1985/q2a-pupi-coma/releases/latest
sort_order: 10
features:
    - label: Export Q2A configuration
      icon: fa-file-download
    - label: Several export options to limit exporting secrets, emails, URLs, etc
      icon: fa-filter
    - label: Import Q2A configuration
      icon: fa-file-upload
---

This plugin allows users to share their Q2A configuration with others. This is particularly useful when trying to identify issues with the Q2A core or plugins.

The general workflow of the plugin would be:

 1. A user who needs support installs the plugin and exports their Q2A configuration
      * Optionally, the user can open the exported file with a text editor and change any setting inside (in case private information has been exported)
 1. The user asks for support (e.g. asking a question here) and includes their Q2A configuration file by a simple attach process
 1. The person providing support can either open the text file to get more insight about the configuration or even import it to their own test environment

The plugin provides some simple filters such as removing values that are known to contain secrets, emails, URLs, etc. However, that doesn't mean the plugin will hide an email address or a site name included in the free text of the sidebar.

You can give it a try downloading it from the GitHub project page.

Plugin features:
 * Export Q2A configuration
 * Several export options to limit exporting secrets, emails, URLs, etc
 * Import Q2A configuration
 * Internationalization support
 * No need for core hacks or plugin overrides
 * Simple installation
