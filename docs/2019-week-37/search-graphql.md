---
title: Search GraphQL 
description: "The `store-graphql` morphed into `search-graphql`, which took over responsibility for your store's GraphQL search related queries."
date: "09/23/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-37/search-graphql.md"
---

# Search GraphQL 

The giant `store-graphql` app was segmented and gave way to the new `search-graphql` app. 

## What has changed 

**Previously, the** `store-graphql` **was a monolith app** responsible for sending GraphQL queries to all [VTEX APIs](https://help.vtex.com/developer-docs), meaning that all information required by the store's front end would necessarily go through `store-graphql`. 

The issue was that the constant and rapid platform evolution meant that the app centralized a very large number of different requests, from getting product data from the Search API (a fast operation having a short timeout and a lot of cache) to adding items in the cart (whose timeout is long due to the delay in Checkout responsiveness along with the inexistent cache, since it's a operation performed by the user). 

Such a scenario resulted in a long code base to meet all the demands required by an increasingly complex front. Therefore, the app had to begin its segmentation process, which started by creating the `search-graphql` app.  

This means that henceforth **all related search queries in** `store-graphql` **will be deprecated and transferred to** `search-graphql` . Specifically: `products`, `productSearch`, `product`, `searchMetadata`, `facets` and `autocomplete`.

## Main advantages

`store-graphql` segmentation into smaller apps such as `search-graphql` aims to better define each app's functionalities. By specializing an app, we are able to:

- Facilitate its code review and support. 
- Set the app's parameters (such as `timeout`, `memória`, `cache` , etc) more adequately.
- Choose more precise metrics to manage and control its performance. 

## What you need to do

To send your queries through `search-graphql`, simply read and attentively follow the steps below:

1. [Install](https://vtex.io/docs/recipes/store/installing-an-app) `search-graphql` version **0.2.3** or higher in your store.
2. Add it as a dependency in your store's `manifest.json`. If your store only uses search related queries such as the above-mentioned, feel free to remove the `store-graphql` app from dependencies.
3.  If your store needs to use the queries of two apps, have **both** as dependencies in your store's `manifest.json`. In this case, you need to mention in each query (in `@context`) which app should be used, following the example below:

```
query Autocomplete($maxRows: Int, $inputValue: String) {
    autocomplete(maxRows: $maxRows, searchTerm: $inputValue) {
    autocomplete(maxRows: $maxRows, searchTerm: $inputValue)
        @context(provider: "vtex.search-graphql") {
        itemsReturned {
            thumb
            name
```

:warning: Fixes and improvements related to search queries should only be performed in `search-graphql` from now onwards.

:eyes: Notice that several deprecated fields, such as `categoriesIds` in `Product`, were removed. Therefore, these fields should also be removed from your queries. In any case, GraphQL will notify you about the removal once the query having the removed field is performed. 

## Side effects 

Nothing should be in the sense that once the code is transferred from one app repository to another.
