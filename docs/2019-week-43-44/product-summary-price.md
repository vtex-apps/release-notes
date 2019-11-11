---
title: Product Summary Price 
description: "Who doesn't like to know how much they saved when buying a product? The Product Summary Price, knowing that the answer to that question if a resounding "everyone", now displays a product's absolute saving to users."
date: "11/11/2019"
git: "https://github.com/vtex-apps/io-documentation/edit/master/docs/en/Recipes/layout/building-a-carousel-through-lists-and-slider-layout.md"
---

# Product Summary Price 

The Product Summary Price component gained a **new prop**, `showDiscountValue`, which allows a product's absolute savings to be displayed to users. 

![product-summary-price](https://user-images.githubusercontent.com/52087100/68607074-95019f00-048e-11ea-9ab4-8573b93494b9.png)

## What has changed

Previously, it wasn't possible to display a product's saving using the Product Summary Price component.

The only way to show users what they were saving on a specific product was using the [`discountBadge`](https://vtex.io/docs/components/product-related/vtex.store-components/discount-badge). But, in any case, it only displayed that saving in percentage points.

## Main advantages 

In addition to clearly **showing users the economic advantages** of buying a specific product at a sale price, this release **eliminates complications** that arose from this process for retailers. 

Since we're dealing with a prop, this **configuration can be directly performed in the block itself**, without the need to resort to other components or customizations.  

## What you need to do

To configure this new prop, use [**Product Summary**](https://vtex.io/docs/app/vtex.product-summary) version **2.43.0** or higher in your store.
