---
title: Navigation arrows on Product image thumbnails 
description: "Users may now navigate on product images thumbnails by clicking on arrows"
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Navigation arrows on Product image thumbnails

Our product-image component now supports navigation arrows on image thumbnails. It is used to improve the PDP UX . Users now receive a hint that the product has more thumbnails to navigate through and are able to navigate through them easily.

## What has changed

Before these arrows, when a user tried to see more images on thumbnails, a scroll bar would show up, which wasn't a nice experience.

## Main advantages

The user now has a better experience when navigating through the product images.

## What you need to do

1 - Make sure your store has the app store-components installed https://github.com/vtex-apps/store-components/

2 - Add the component product-images to your store's product details page https://github.com/vtex-apps/store-components/blob/master/react/components/ProductImages/README.md

3 - Add the prop “displayThumbnailsArrows” and set it as `true` in  blocks.json. 

Example:

```
  "product-images": {
    "props": {
      "displayThumbnailsArrows": true
    }
  }
```

If you need a more comprehensive PDP example, our store-theme has this feature already implemented:
https://github.com/vtex-apps/store-theme/blob/master/store/blocks/product.json

See PR reference and images here: https://github.com/vtex-apps/store-components/pull/531

See issue references/images here: https://github.com/vtex-apps/store-discussion/issues/57

See an implemented example here: https://shop.samsung.com.ar/galaxy-j4-plus/p
