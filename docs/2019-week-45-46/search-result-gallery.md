---
title: Search Result Gallery
description: "During the Black Friday week, the e-commerce gods have bestowed the blessing upon the Gallery component, making it responsive and willing to accept different values for (almost) any existing device."
date: "11/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/search-result-gallery.md"
---

# Search Result Gallery

The Search Result Gallery component's `maxItemsPerRow` prop just became **responsive**. In addition to sending a single value, it now allows an object to send different values for different devices. 

## What has changed 

Previously, the prop only allowed a single value, valid for all the store's layouts. Therefore, the number of items displayed in the search results gallery by row was always the same, irrespective of which device was used.

From now on, you can establish values for **different devices** by using an object. The same Gallery can therefore display a different number of items per search results row, based on the user's device and the layout breakpoint that is being applied. 

### How it works

By using this object, you can specify the user device, as shown below:

```
maxItemsPerRow = { 
desktop: 5, 
tablet: 3, 
phone: 2, 
},
```

Alternatively, you can separate mobile (phone & tablet) and desktop values: 

```
maxItemsPerRow = { 
desktop: 5, 
mobile: 3, 
},
```
 
## Main advantages

Users access the desired website using portable devices such as phone or tablets with increased frequency, no longer being dependent of desktop computers for that.

Therefore, making a component flexible to responsive values is both **important** and **strategic**, helping businesses keep **up-to-date with current e-commerce user demands**.

## What you need to do 

To apply this improvement to your store, [**Search Result**](https://vtex.io/docs/app/vtex.search-result) version **3.39.0** or higher must be installed.
