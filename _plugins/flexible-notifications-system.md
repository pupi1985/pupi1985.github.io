---
title: Flexible Notifications System
subtitle: Allows users to receive notifications in a flexible and efficient way
description: Allows users to receive notifications in a flexible and efficient way
product_code: FNS
layout: product
image: /img/FNS-notification.png
price: 0
wiki_url: https://github.com/pupi1985/q2a-pupi-fns
download_url: https://github.com/pupi1985/q2a-pupi-fns/releases/latest
sort_order: 9
features:
    - label: Show notifications to users
      icon: fa-bell
    - label: Easy integration with plugins and themes
      icon: fa-puzzle-piece
    - label: High performance
      icon: fa-gauge-high
---

In the world of Q2A, I wear three different hats, each with its own set of needs:

 * As a plugin developer, I need a simple and extensible way to show custom notifications to users
 * As a theme developer, I need to easily integrate notifications plugins to my themes
 * As a user, I need to see my notifications in a simple and fast way (including RTL and mobile)

So I decided to develop a plugin that would tackle these 3 issues.

The main plugin features are:

 * Generates notifications for users based on Q2A's events (e.g. an answer is added to a user's question)
 * Efficient database access
 * Avoids many database accesses by utilizing the core's built-in caching mechanisms (memcached is, by far, the fastest)
 * Allows plugins to extend the notifications from the core easily
 * Allows themes to replace the look and feel of the plugin
 * Tracks read/unread notifications
 * The built-in UI and the internal notification tracking logic are decoupled
 * Even though the features might sound a bit "technical" take into account 2 out of the main needs I mentioned above are mainly intended for developers. This will allow other developers to extend and integrate with this plugin easily.

By the way, this is what the built-in UI looks like:

You can give it a try downloading it from the GitHub project page.