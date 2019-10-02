---
title: ProductSummaryBrand component
description: "Render brand data with your own customizations in your Shelf component."
date: "29/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---



# `ProductSummaryBrand` component

The new `ProductSummaryBrand` component make it possible to include brand data in the Shelf, as well as in other store components that use the Product Summary context. 

## What has changed

The `ProductBrand` component is responsible for rendering your store's brand data, such as brand name and logo. This component is able to render this information with the help of the **Product context**, place where product data is stored (and subsequently,  product brand data). 

The issue is that to render its data, the Shelf component uses the **Product Summary context** as storage. As a result, the `ProductBrand` is not declared on pages or in components that didn't use Product Context, such as Shelf or PDP. 

The `ProductSummaryBrand` was therefore created using Product Summary context to perform the `ProductBrand` function in pages and components that use this storage for rendering. 

<img width="590" alt="productsummarybrand-component" src="https://user-images.githubusercontent.com/52087100/63977079-316bf600-ca89-11e9-8f29-bcaad1807c38.png">


## How it works

The new component behaves in the same way as `ProductBrand`, however two of its props differ, namely `brandName` and `brandId`. These two props don’t have to be declared in the `ProductSummaryBrand` since it gets this data from the Product Summary context.

Therefore, you can configure the `ProductSummaryBrand` with the following props:

- `displayMode`: __string__ - you should choose between “logo” or “text”. This will define whether the product brand will be displayed by name or logo.

- `fallbackToText`: __boolean__ - This prop should only be used when `displayMode` is set to `logo`. It defines what should be done when the Brand Component should have displayed a brand logo but no image was registered in the VTEX Catalog. This prop is set as `true` by default, allowing the logo to be replaced with the brand name in those cases. When set as `false`, the store will not show the brand name instead of the brand logo.

- `height`: __number__ - it sets the logo height. It should only be used when `displaymode` is set to “logo”.

- `excludeBrands`: __array of strings__ - The brand names or brand IDs that are listed in the array will never be displayed by the Brand component. It is usually useful to hide default brand names/logos or test brand names/logos on the store front.

- `logoWithLink`:	**boolean** -	it sets if the brand logo will have a link that leads to the store's brand page. 

:eyes: Remember that it is necessary to choose between “text” and “logo” in the ‘displaymode’ prop, meaning that __if you want to add both the Brand name and the Brand logo to to your Product Details page, the Brand component should be added twice__, setting the ‘displaymode’ prop to “logo” and “text” each time.


## Main advantages

Creating a brand component that uses the Product Summary context is very worthwhile. It not only allow brand data to be rendered on the Shelf component, but also allows it to be customized, with its own style, different from the style set for product data.

## What you need to do

To enable this new feature in your store, make sure the following installation are up-to-date:

- [**Store Components**](https://github.com/vtex-apps/store-components) version **3.63.0** or higher.

- [**Product Summary**](https://github.com/vtex-apps/product-summary) version **2.33.0** or higher.
