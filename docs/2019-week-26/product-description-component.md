# Product Description component

With the prop `collapseContent`, our [Product Description](https://github.com/vtex-apps/store-components/blob/master/react/components/ProductDescription/README.md) component now can be configured to either display a whole product description or a description preview with a call to action button to show the whole content.

## What has changed

Before this prop was created, the product description was always cropped when it was too long. It was not possible to set a default that would display the whole product description.

![product-description-showmore-button](https://user-images.githubusercontent.com/52087100/60601061-cdc69480-9d87-11e9-84cd-490696f625db.png)


## Main advantages

This improvement delivers a more flexible solution that serves different layouts needs. The retailer is now able to decide whether the product description should be collapsed when too long (as it was previously) or displayed in full, thereby ensuring the user has a better shopping experience.  

## What you need to do 

To set this improvement up in your store, follow the steps below:

1. Make sure that your store has at least version 3.49.0 of the app [Store Components](https://github.com/vtex-apps/store-components) installed.

2. Set the prop `collapseContent` to `false` in the `product-description` block that should be set on your [Product Details](https://github.com/vtex-apps/product-details) page, thereby ensuring that the full content of a product description will always be displayed, regardless of its size.

:eyes: If the prop is set to `true`,  a "_Show More_" button will be displayed whenever the product description is too long and collapsed. 
