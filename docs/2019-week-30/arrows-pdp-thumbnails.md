---
title: Navigation arrows on Product images thumbnails 
description: "Users may now navigate on product images thumbnails by clicking on arrows"
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Navigation arrows on Product images thumbnails

Now our product-image component support navigation arrows on image thumbnails. It is used to improve the UX of the PDP. Now users have a hint that the product has more thumbnails to navigate through, and are able to navigate through them easily.

## What has changed

Before this arrows, when a user tried to see more images on thumbnails, a scroll bar would show up, which wasn't a nice experience.

## Main advantages

Now the user has a better experience when navigating throught the images of the product.

## What you need to do

1 - Make sure you have the app store-components installed in your store https://github.com/vtex-apps/store-components/

2 - Add the component product-images to your store's product details page https://github.com/vtex-apps/store-components/blob/master/react/components/ProductImages/README.md

3 - Add the prop “displayThumbnailsArrows” to it on the blocks.json, and set it as `true`. 

Example:

```
  "product-images": {
    "props": {
      "displayThumbnailsArrows": true
    }
  }
```

If you need a more complete example of PDP, our store-theme already has this feature implemented:
https://github.com/vtex-apps/store-theme/blob/master/store/blocks/product.json

See reference and images here on this PR: https://github.com/vtex-apps/store-components/pull/531

See reference/images here for the issue: https://github.com/vtex-apps/store-discussion/issues/57

See implemented example here: https://shop.samsung.com.ar/galaxy-j4-plus/p

