---
title: href on brand component
description: "Now our brand component supports url that takes the user to the brand's page on the store."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# href on brand component

Now our brand component supports url that takes the user to the brand's page on the store. The brand component may be placed at PDP, and it shows the brand name or icon, and now, it can also hold the link to the store's brand page.

## What has changed

It wasn't possible to make the product brand logo redirect to the brand page in the store, but that is possible now with the logoWithLink prop in the ProductBrand. Before, the image/text was never clickable.

## Main advantages

The component can become more interactive. Now the user can land the brand page more easily.

## What you need to do

1 - Make sure you have the app `store-components` installed in your store: https://github.com/vtex-apps/store-components/

2 - Add the component `product-brand` to your store's product details page: https://github.com/vtex-apps/store-components/blob/master/react/components/ProductBrand/README.md

3 - Add the prop `logoWithLink` to it on the blocks.json, and set it as `true`.

Example:

```
  "product-brand": {
    "props": {
      "logoWithLink": true //Default value is false. If true, the logo on the PDP will have the brand's link
    }
  }
```
