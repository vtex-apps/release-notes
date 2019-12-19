---
title: Sku Selector
description: "Retailers always want power and control over their blocks. Not that I'm judging them, since they're more than right to want as much flexibility as possible for their stores. Therefore, meeting demand, new SKU Selector props (`initialSelection` and `displayMode`) are now here to get rid of block rigidity."
date: "12/19/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-47-48-49-50-51/sku-selector.md"
---

# Sku Selector

The Sku Selector block was given **two new props**: 

- `displayMode`: responsible for defining whether the block will be displayed in **buttons** by default (as the product variation images are) or by **dropdown-list**. 

- `initialSelection`: controls the **user initial selection** in the SKU Selector when a product page is loaded. 

## What has changed

Previously, the SKU Selector was always displayed in a button format, as shown in the image below:

![sku-selector-botoes](https://user-images.githubusercontent.com/52087100/71180509-1946ff00-2251-11ea-9606-3e7943df5be0.gif)

With these two new props, the SKU Selector can now be displayed as a drop-down list as well: 

![sku-selector-dropdown](https://user-images.githubusercontent.com/52087100/71180513-1946ff00-2251-11ea-8ec1-fa589ddc4ba4.gif)

In addition, you now can define the block's behavior when users get to the product page. Previously, the SKU Selector automatically selected the given variation for the user. Now, you can define between the following options for the SKU Selector behavior: 

- Selecting the variations referring to the first available SKU fetched (default behavior);
- Selecting the first image variation fetched (such as color);
- Not selecting variations automatically. 

## Key advantages 

Before the two new props, there was no flexibility whatsoever in terms of format and initial block behavior when the product page was loaded. 

The rigidity of the SKU Selector did not leave room to **address some business scenarios**, such as the need for another form to display long texts within the default buttons. Therefore, the new props **expand the block's applicability**, better **meeting retailer needs** and desires when it comes to the behavior of their store.

## What you need to do 

The `initialSelection` prop can be used starting with [**Store Components**](https://vtex.io/docs/components/all/vtex.store-components/) version **3.82.0**, while the `displayMode` prop is only available from version **3.91.0**  onwards of the same app. 

Don't forget to access the [**SKU Selector**](https://vtex.io/docs/components/all/vtex.store-components/sku-selector) documentation to know further about the new possible values and behaviors.
