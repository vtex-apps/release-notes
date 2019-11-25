---
title: Search query
description: "Shall we celebrate search query's independence from the facets query? Even when the latter doesn't return any results, the former renders data fetched by the `productSearch` query, providing users with search results regardless."
date: "11/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/search-query.md"
---

# Search query

The `search` query now **returns search results** to users even when the `facets` query doesn't find any. 

## What has changed

The `search` query is formed by two other queries: `productSearch` and `facets`. Previously, when the `facets` query didn't return results, the `search` query automatically ignored data fetched by the `productSearch` and instead displayed to users a 404 not found. 

With this `search` query improvement, the data fetched by `productSearch` is shown to users even when the `facets` query doesn't return anything. 

In practice, the `search` returns to the user the complete product page, but without the filters in the left corner of the screen (fetched by `facets`).

## Main advantages 

The former behavior's main problem was that it curtailed user access to relevant data about their query because of a performance error from the `facets`. 

Therefore, this release's biggest advantage is **improving user experience**, which, even if having to deal with an incomplete filter-less search results page, can still browse through the returned products. 

## What you need to do

Rejoice with me: you don't need to do **anything**! This improvement is already available to all platform stores.
