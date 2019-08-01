---
title: Full category tree for GTM events
description: "Every Google Enhanced Ecommerce event used by our Tag Manager solution now sends the whole product category tree."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Full category tree for GTM events

Every Google Enhanced Ecommerce event used by our Tag Manager solution now sends the whole product category tree. You can use this new information in your Google Analytics.

## What has changed

In the every event's category field, we now send the full category tree, instead of the simple category.

### How it works

Example: [https://storetheme.vtex.com/apparel---accessories/hats/caps](https://storetheme.vtex.com/apparel---accessories/hats/caps)

For this product, we would send the information:

```
{
...
	category: “caps”,
...
}
```  
We now send the full category tree:

```
{
...
	category: “apparel---accessories/hats/caps”,
...
}
```

It immediately reflects upon the store's Google Analytics.

## Main advantages

The user can now undertake a better analysis of categories navigation, since the full tree is available.

## What you need to do

All the events related to the products already have the category tree info.

## Side effects

You might notice that the category structure shown in your Google Analytics has changed.