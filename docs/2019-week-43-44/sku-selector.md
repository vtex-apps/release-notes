---
title: SKU Selector
description: "The SKU Selector is fully loaded this week: it can not only display exclusive images, but also be wholly displayed on the Shelf and even in the Search Results page. Check out the details here!"
date: "11/11/2019"
git: "https://github.com/vtex-apps/release-notes/edit/master/docs/2019-week-43-44/sku-selector.md"
---

# SKU Selector

O SKU Selector component obteve dois importantes improvements nas ultimas semanas:

- It can be now **displayed on Product Summary components** such as the Shelf.

![product-summary-sku-selector](https://user-images.githubusercontent.com/52087100/68625690-87f9a580-04b8-11ea-835d-009ac768805f.gif)

- Your **images can be changed natively**, without the need to replicate a miniature of the image set in the catalog. 

![sku-selector-image-custom](https://user-images.githubusercontent.com/52087100/68700719-20992f80-0564-11ea-955a-d65c5a5808be.png)

## What has changed 

Previously, in addition to not being able to display the SKU selector in components that use Product Summary, such as the Shelf, **the images used were unchangeable**. 

You could not set the SKU selector to display custom images. The component would always use a miniature of the product image, as given in the catalog.

Now, you can choose **special images** for the SKU selector, in addition to having it **appear on the Shelf and Search Results Page** - two components that use Product Summary data.

## Main advantages

Displaying the SKU Selector on Shelves and Search Result pages was a longtime requisite retailers had, as they wanted to make existing **buying options visible to shoppers before the product was accessed**. 

In addition, the use of exclusive images in the SKU selector **enriches** the component, making it **more flexible** to the layout needs retailers may have.

## What you need to do 

If you want the SKU selector to be displayed on Shelves and Search Result Pages, you can access the Product Summary SKU Selector [**documentation**](https://vtex.io/docs/app/vtex.product-summary/product-summary-sku-selector). 

For more on the SKU selector images, access the recipe [**Configuring custom images for the SKU Seletor**](https://vtex.io/docs/recipes/layout/configuring-custom-images-for-the-sku-selector).
