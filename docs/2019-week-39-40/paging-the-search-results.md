---
title: Paging the Search Results
description: "Gain more agility with a URL for each of the loaded search results page!"
date: "10/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/paging-the-search-results.md"
---

#  Paging the Search Result

The Search Results page URL now reflects the exact page loaded by the user. 

![search-result-pagination-als](https://user-images.githubusercontent.com/52087100/66756478-7ea4fb00-ee70-11e9-8ba3-305f8e3bac83.gif)

## What has changed

Now, every time you trigger the Search Results page to fetch more results, whether through a button or infinite scrolling, the page URL will change.

Previously, the component could not enable this behavior. Independent of the search result pages loaded and accessed by the user, the URL stayed the same. 

## Main advantages

Since the URL will now reflect the loaded page, it becomes possible to share a specific search results page through a simple link. 

In addition, you can freely click on a product when navigating through a search results page because the new URL format allows you to return to the exact page you were on before! 

## What you need to do

To enable this feature in your store, have the [<code>search-result</code>](https://vtex.io/docs/components/search/vtex.search-result) component version **3.33.0** or higher [installed](https://vtex.io/docs/recipes/store/installing-an-app).
