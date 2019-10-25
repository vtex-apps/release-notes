---
title: SKU Selector
description: "New SKU Selector props will allow you to define image height and width without needing to resort to CSS customization. Enhanced performance and practicality in a single improvement, a dream come true!"
date: "10/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/sku-selector.md"
---

# SKU Selector

The SKU Selector component gained **two new props** that define the height and width of its images: `imageHeight` e `imageWidth`. 

![sku-selector-image](https://user-images.githubusercontent.com/52087100/67565083-ed991400-f6fa-11e9-952c-b29675a8b98b.png)

## What has changed

Before the improvement, an SKU Selector's image size could only be set through CSS classes. 

The image dimensions are now established in the block itself (`sku-selector`), through the use of props.

## Main advantages

Defining a fixed size image in a block and resizing it through the CSS defined image dimensions is detrimental to a store's performance, since the image is loaded with one size only to then be rendered with another.

In extreme cases where files that were very large were set through CSS as smaller or vice-versa, the store may face image quality loss.

The image is now loaded with the exact render size (neither greater nor smaller), not only improving **performance** and **image quality**, but also earning the store **more Lighthouse points**.

## What you need to do 

Make sure you store is running the [**Store Components**](https://vtex.io/docs/app/vtex.store-components) app version **3.72.0** or higher.
