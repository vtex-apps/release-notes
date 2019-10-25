---
title: Product Summary
description: "Did you enjoy the SKU Selector release? So check out our Product Summary release as well: more props para define image sizes!"
date: "10/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/product-summary.md"
---

# Product Summary

Similar to the SKU Selector, the Product Summary component gained **two new props** the define the height and width of its images: `height` and `width`. 

![product-summary-image](https://user-images.githubusercontent.com/52087100/67565345-98113700-f6fb-11e9-820a-22359dc206de.png)

## What has changed

Before the improvement, Product Summary images dimensions could only be set through CSS classes. 
The image dimensions are now established in the block itself (`product-summary-image`), through the use of props.

In addition, these dimensions are **responsive**, since the props can have different and exclusive values for either `desktop` or `mobile`. 

## Main advantages

Defining a fixed size image in a block and resizing it through the CSS defined image dimensions is detrimental to a store's performance, since the image is loaded with one size only to then be rendered with another. 

In extreme cases where files that were very large were set through CSS as smaller or vice-versa, the store may face image quality loss.

The image is now loaded with the exact render size (neither greater nor smaller), not only improving **performance** and ** image quality**, but also earning the store **more Lighthouse points**.

## What you need to do 

Make sure you store is running the [**Product Summary**](https://vtex.io/docs/app/vtex.product-summary) app version **2.37.0** or higher.
