---
title: Temporary User Block
subtitle: Allows users to be blocked for a period of time and then be automatically unblocked
description: Allows users to be blocked for a period of time and then be automatically unblocked
product_code: TUB
layout: product
image: https://bitbucket.org/repo/ngjoq7K/images/992760182-preview.png
price: 30
wiki_url: https://bitbucket.org/pupi1985/q2a-temporary-user-block-public
sort_order: 5
features:
    - label: Blocks users temporarily
      icon: fa-user-clock
    - label: Users can provide a block reason
      icon: fa-tag
    - label: Blocked users can be notified
      icon: fa-bell
---

Q2A makes it easy to get rid of a user that is not behaving properly in a site. With a few clicks the user can be blocked and their posts hidden or even removed. In most cases, blocking users in this way is the right way to go.

However, this leaves aside a few things:

 * There is no way to see why a user was blocked
 * In order to *warn* a user and block them for a short period of time, it is needed to manually set the reminder to go to the user profile and unblock them later

The *Temporary User Block* plugin tackles exactly those 2 issues. It does so by asking some additional information to the user whenever a block is being performed. The information is requested in a popup displayed whenever the *Block* button is pressed:

![Temporary user block](https://bitbucket.org/repo/ngjoq7K/images/992760182-preview.png)

The user selects the period for the block (8 hours in this case), optionally inputs a reason for it and selects whether to send the blocked user an email notification with this information. After confirming the information, the user is immediately blocked. However, once the 8-hour period finishes, the user will be automatically unblocked.

This should serve as *warnings* for users who still have a chance to become productive members of a community and also would help administrators understand better why a moderator blocked a given user.

Here is a complete list of features:

 * Allows users to be blocked either permanently or temporary
 * Users are able to include a reason for the block that is displayed in the user profile
 * Both kind of blocks can send a block email notification to the blocked user
 * Temporary blocks can be configured in hours and days
 * A countdown is displayed in the user profile showing the user how much time left they have before getting unblocked
 * Once the countdown reaches zero, the temporary blocked user is unblocked
 * Admin options allow to set the block reason length as well as what user levels should be able to see the additional profile fields
