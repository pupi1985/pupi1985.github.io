---
title: Maximum Tag Length
subtitle: Limits the amount of characters allowed per each question tag
description: Limits the amount of characters allowed per each question tag
product_code: MTL
layout: product
image: /img/MTL-settings.png
price: 0
wiki_url: https://github.com/pupi1985/q2a-maximum-tag-length
download_url: https://github.com/pupi1985/q2a-maximum-tag-length/releases/latest
sort_order: 14
features:
    - label: Users can configure the maximum tag length in the settings
      icon: fa-cogs
    - label: Questions that contain long tags cannot be asked
      icon: fa-tag
    - label: No core hacks or plugin overrides needed
      icon: fa-file-code
---

The core doesn't provides a few checks on tags, but focus on the amount of tags. It doesn't focus on tag length. This brings the issue of users creating long tags (either by mistake or on purpose) that are hard to delete.

This plugin just checks the amount of characters in question tags does not exceed a given limit.

![Plugin settings](/img/MTL-settings.png)

If a question exceeds the limit, an error id displayed:

![Question error](/img/MTL-question-error.png)

These are the plugin features:

 * Does not allow posting or editing questions that have a character count that exceeds a given amount
 * Internationalization support. Spanish translation included
 * No need of core hacks or plugin overrides
 * Simple installation
