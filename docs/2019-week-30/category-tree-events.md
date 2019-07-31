---
title: Full category tree on GTM events
description: "Now, every event of Google Enhanced Ecommerce used by our Tag Manager solution sends the whole category tree of the product."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Full category tree on GTM events

Now, every event of Google Enhanced Ecommerce used by our Tag Manager solution sends the whole category tree of the product. You can use that new information on your Google Analytics.

## What has changed

On the category field of every event we now send the full category tree, instead of the simple category.

### How it works

Example: [https://storetheme.vtex.com/apparel---accessories/hats/caps](https://storetheme.vtex.com/apparel---accessories/hats/caps)

For this product we would send the information:

```
{
...
	category: “caps”,
...
}
```  
Now we send the full category tree:

```
{
...
	category: “apparel---accessories/hats/caps”,
...
}
```

It reflects immediately on the Google Analytics of the store.

## Main advantages

Now the user can make better analysis on categories navigation, since the full tree is available.

## What you need to do

All the events related to the products already have the category tree info.

## Side effects

You might notice that the category structure that is shown in your google analytics has changed.
