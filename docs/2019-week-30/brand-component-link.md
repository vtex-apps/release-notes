---
title: href on brand component
description: "Our brand component now supports a url that takes the user to the store's brand page."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# href on brand component

Our brand component now supports a url that takes the user to the store's brand page. The brand component may be placed on the PDP, showing the brand name or icon and can now also hold the link to the store's brand page.

## What has changed

It wasn't possible to make the product brand logo redirect to the store's brand page, but that is now possible with the `logoWithLink` prop in the Product Brand. Previously, the image/text was never clickable.

## Main advantages

The component can become more interactive.  The user can now land on the brand page more easily.

## What you need to do

1 - Make sure the app `store-components` installed in your store: https://github.com/vtex-apps/store-components/

2 - Add the `product-brand` component to your store's product details page: https://github.com/vtex-apps/store-components/blob/master/react/components/ProductBrand/README.md

3 - Add the prop `logoWithLink` to it through blocks.json, and set it as `true`.

Example:

```
  "product-brand": {
    "props": {
      "logoWithLink": true //Default value is false. If true, the logo on the PDP will have the brand's link
    }
  }
```