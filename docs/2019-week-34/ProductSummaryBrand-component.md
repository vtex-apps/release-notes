---
title: `ProductSummaryBrand` component
description: “waiting for proper translation”
date: “29/08/2019"
git: “https://github.com/vtex-apps/release-notes”
---


# `ProductSummaryBrand` component

The new `ProductSummaryBrand` component make it possible to include brand data in the Shelf, as well as in other store components that use the Product Summary context. 

## What has changed

The `ProductBrand` component is responsible for rendering your store's brand data, such as brand name and logo. This component is able to render this information with the help of the **Product context**, place where product data is stored (and subsequently,  product brand data). 

The issue is that to render its data, the Shelf component uses the **Product Summary context** as storage. As a result, the `ProductBrand` is not declared on pages or in components that didn't use Product Context, such as Shelf or PDP. 

The `ProductSummaryBrand` was therefore created using Product Summary context to perform the `Product Brand` function in pages and components that use this storage for rendering. 

<img width="590" alt="productsummarybrand-component" src="https://user-images.githubusercontent.com/52087100/63977079-316bf600-ca89-11e9-8f29-bcaad1807c38.png">


## How it works

For a brand's data to be correctly rendered through `ProductSummaryBrand`, two new `ProductBrand` component props (`brandName` and `brandId`) must be filled out. 

Filling out these props will allow brand data to reach your store through an external source (such as Product Summary context) instead of the Product context. 

## Main advantages

Creating a brand component that uses the Product Summary context is very worthwhile. It not only allow brand data to be rendered on the Shelf component, but also allows it to be customized, with its own style, different from the style set for product data.

## What you need to do

To enable this new feature in your store, make sure the following installation are up-to-date:

- [**Store Components**](https://github.com/vtex-apps/store-components) version **3.63.0** or higher.

- [**Product Summary**](https://github.com/vtex-apps/product-summary) version **2.33.0** or higher.
