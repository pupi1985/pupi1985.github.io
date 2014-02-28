---
title: Fake Cron
subtitle: Fires events after a certain amount of requests or in a time-based manner (daily, weekly, monthly)
description: Fires events after a certain amount of requests or in a time-based manner (daily, weekly, monthly)
product_code: FC
layout: product
image: /img/FC-code.png
price: 0
wiki_url: https://github.com/pupi1985/q2a-fake-cron
download_url: https://github.com/pupi1985/q2a-fake-cron/archive/refs/heads/master.zip
sort_order: 11
features:
    - label: Ability to fire events faking time events
      icon: fa-cloud
    - label: Events can be fired by counting server requests
      icon: fa-plus
    - label: Events can be fired in a certain frequency (e.g. daily)
      icon: fa-calendar-alt
---

This is a simple plugin that is mostly intended for developers. Basically, Q2A has no support for cron, although it allows its integration. However, configuring a cron process is something the average user does not know how to do. So I thought that, although cron is irreplaceable, a workaround could be implemented that would work for most scenarios in which cron is needed.

So suppose you need to perform an action. Let's take, for instance, a table clean up. You could perform a DELETE statement on every request. Or maybe you could implement a counter that would execute the DELETE statement after a given amount of requests, in order to decrease server load.

Well, this plugin does exactly that. It fires an event after a given amount of requests. So all it is needed is to register an event module and make sure it listens to the event the plugin fires. This way, you just need to focus on the actions you need to perform (the DELETE) and how often you want them to be run (every 400 requests).

Additionally, the plugin can fire events on a daily, weekly and monthly basis. These events are, again, generated based on a request, however, they are limited to run only once per time period.

Again, the plugin does not care at all about time. Only about server requests, which may or may not be the same for the actions needed by other plugins.

Plugin features:
 * An event is fired every a 100 requests
 * An event is fired once daily, weekly and monthly (provided a request has been performed)
 * Avoids performing a given operation (checking files, running database queries, sending an email, checking server status, etc) on each request
 * No need of core hacks or plugin overrides
 * Simple installation

Plugin notes:
 * This plugin is no replacement of cron and does fire any event based on the time factor
 * The plugin is intended to be installed by Q2A admins but actually used by developers
 * There are several technical details in the GitHub repository that should not be overlooked
 * Works on Q2A version 1.6 and later
