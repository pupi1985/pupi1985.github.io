---
title: Dynamic Mentions
subtitle: Allows users to be mentioned using the @user syntax
description: Allows users to be mentioned using the @user syntax
product_code: DM
layout: product
image: https://bitbucket.org/repo/x8x6e9X/images/4111031239-2.png
price: 30
wiki_url: https://bitbucket.org/pupi1985/q2a-dynamic-mentions-public
sort_order: 8
features:
    - label: Tag users in posts using the @user syntax
      icon: fa-at
    - label: Email notifications to mentioned users
      icon: fa-envelope
    - label: On-Site Notifications plugin integration
      icon: fa-bell
---

I'd like to compare Q2A with [StackOverflow.com](https://stackoverflow.com), which is the kind of platform I believe Q2A should aim to become, and try to see what makes it better to steal some ideas. Clearly, user mentions, in the form of **@user**, with a UI-friendly solution came up so I decided to create a nicely looking plugin that would take care of this.

This should sum everything up:

![Dynamic mention animation](https://bitbucket.org/repo/x8x6e9X/images/3015656445-1.gif)

The animated sequence shows how typing an **@** character followed by a couple of additional characters triggers the display of a popup to select users. The admin can configure this popup to be filled with only the users involved in the question thread or every user in the site.

![Dynamic mention dropdown](https://bitbucket.org/repo/x8x6e9X/images/4111031239-2.png)

Mentioning a user not only creates a link to the user's profile but also can notify them about the mention. The admin can configure two kinds of notifications. One is an email notification. The other one is a notification by means of the [On-Site Notifications plugin](https://github.com/q2apro/q2apro-on-site-notifications). This notification system is very useful when trying to involve other users into a thread.

One additional feature that is worth mentioning is that the admin can set a minimum user level that will be allowed to create mentions to other users. That way the admin can restrict the feature just to Editors and above.

Here is a complete list of features:

 * Easily transform a username into a clickable link when writing a post (mention)
 * Users can be selected from a popup list of matched users
 * An additional user field can be displayed in the popup (e.g. the full name of the user)
 * Mentions can be used in questions, answers and comments
 * Full and basic editors can be selected for each kind post
 * On-Site Notifications plugin integration that allows receiving a notification to mentioned users
 * The admin can choose to enable sending email notifications to mentioned users
 * User permits can be configured to allow a minimum user level allowed to generate mentions
 * Does not require any core hack and does not modify the core tables structure
