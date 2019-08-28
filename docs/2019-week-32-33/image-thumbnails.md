---
title: Image thumbnails 
description: "The Product Images component now allows a product’s thumbnails to be displayed either vertically or horizontally on the page."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Image thumbnails

Thanks to the new `thumbnailsOrientation` prop, the [Product Images](https://github.com/vtex-apps/store-components/blob/master/react/components/ProductImages/README.md) component now allows a product’s thumbnails to be displayed either vertically or horizontally on the page.

## What has changed

Previously, it was not possible to choose how a product’s thumbnail images were set on a store’s page. The only possible behavior was to have them vertically.

The `thumbnailsOrientation` prop now allows a product’s page thumbnail images to be custom positioned according to your store’s needs:

- **Vertical** (default value)

<img width="473" alt="thumbnails-image-vertical" src="https://user-images.githubusercontent.com/52087100/63535192-4378f200-c4e7-11e9-8f27-17280583a1af.png">

- **Horizontal**

<img width="360" alt="thumbnails-image-horizontal" src="https://user-images.githubusercontent.com/52087100/63535269-74592700-c4e7-11e9-813e-b873164666b9.png">

## Main advantages

The new prop allows the retailer to be able to choose the best way to position thumbnails for its users, avoiding that an unwanted default behavior be forced onto the product’s page layout.

## What you need to do

To be able to customize your store’s thumbnail position, have version __3.61.0__ or higher of [**Store Components**](https://github.com/vtex-apps/store-components) installed.
