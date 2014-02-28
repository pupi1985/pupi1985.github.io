---
title: Advanced Search
subtitle: Extends the way in which Q2A searches for posts and allows the user to get better results when searching
description: Extends the way in which Q2A searches for posts and allows the user to get better results when searching
product_code: AS
layout: product
image: /img/AS-search-page.png
price: 40
wiki_url: https://bitbucket.org/pupi1985/q2a-advanced-search-public
sort_order: 3
features:
    - label: Filter posts by specific fields
      icon: fa-filter
    - label: Force and exclude words in search results
      icon: fa-search
    - label: Quick search reference widget
      icon: fa-window-maximize
---

The Advanced Search plugin gives users the ability to find what they're looking for. The plugin got inspired by and resembles [StackOverflow](https://stackoverflow.com)'s search, the #1 Q&A site in the world.

How Q2A searches for posts is a bit obscure and can only be fully understood by looking at the code. In short, it matches the query string against all posts that have at least one word from the query string in the title, content, tag or even as a username. Then it ranks everything based on a fixed criteria, such as if the word is in a title it's twice as important as if it's in an answer.

The issue with the default search is that it generates a huge amount of matches and doesn't allow the user to be more specific such as only looking for words in the title of a question or looking for content within a particular tag. These issues are the ones that the Advanced Search plugin aims to tackle.

Plugin features include:

 * Filter posts by question title, tags, author or content
 * Ability to force and exclude words or tags in the results
 * Combine tag, title, content, username searches in a single query
 * New ways of filtering questions (amount of views, amount of answers, score, close status and selected answer status)
 * A Small and handy widget can be included for a quick reference
 * External users support

Here are some examples of useful searches that should give a better idea of what the plugin does:

 * **tag:math square triangle** - matches posts with the words **square** or **triangle** within the **math** tag
 * **+tag:programming-language +tag:c# user:john** - matches posts with both tags **programming-language** and **c#** created by the user **john**
 * **content:break -title:car isaccepted:true** - matches posts that have the word **break** only in the content of the post, that don't have the word **car** in the question title and that have an answer accepted
 * **tag:electronics -tag:computing isclosed:false views:100** - matches posts within the **electronics** tag that are not tagged as **computing**, that are not closed and that have at least **100** views
