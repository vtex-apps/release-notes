---
title: Change image on Hover 
description: "The Product Summary component now supports a native hover effect to replace the main product's image with a secondary one."
date: "09/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Change image on Hover

The [Product Summary](https://github.com/vtex-apps/product-summary) component, available in the Shelf and Search Results components, now supports a native hover effect to replace the main product's image with a secondary one.

<img width=200 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62786798-bae76400-ba99-11e9-9713-69bb996cf842.gif">

## What has changed 

Prior to this new feature, the product's image in the Shelf and the Search Results components would always be static. Now another image added to the main product's SKU can be displayed when the user hovers over the product image with the mouse. 

## Main advantage 

Using this effect brings your user additional interactivity and a custom experience.

## What you need to do

__1.__ In your catalog, add an specific tag to the image that will be displayed as the secondary hover image. This can be done by following [this tutorial](https://help.vtex.com/tracks/catalog-101--5AF0XfnjfWeopIFBgs3LIQ/17PxekVPmVYI4c3OCQ0ddJ).

__2.__ To enable the effect, you must open the __Storefront__ section in admin. Go to your store's admin, click on __CMS__ and then on Storefront.

__3.__ Go to the Product Summary Image component of the block you want to add this effect to. First find the block you want to edit, for example, the shelf shown below. Click on the arrow to show its subcategories and then on the arrow of the component Product Summary that has appeared. Lastly, select on the __Product Summary Image__ component.

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62786941-00a42c80-ba9a-11e9-99bc-54aaeb022848.png">

__4.__ Label the tag that you have already added as secondary image in the catalog by filling out the __Hover Image Label__ field.

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62787039-38ab6f80-ba9a-11e9-9a73-9fadbca1d8f0.png">

__5.__ Click on __Save__.
