# Product Identifier component

It is possible to now display a product identifier on your Product page, Shelf and Search Results.

<img width="211" alt="product-identifier-component" src="https://user-images.githubusercontent.com/52087100/60997935-62a03380-a32e-11e9-9c3b-754fdc01ec7d.png">

The new [Product identifier component](https://github.com/vtex-apps/product-identifier) can be configured to display the following product identifier options:

- Product Reference

- Product ID

- SKU EAN

- SKU Reference


## What has changed

Prior to this release, the products/SKU IDs and references weren’t available anywhere else on the store’s site.

## Main advantages

By displaying an official ID or Reference, the user can easily refer to the product or SKU through any of the store’s available communication channel, improving their buying experience.

In addition, this component is useful for providing extra flexibility in the store layout since it can be placed anywhere when combined with the Product page flex layout.


## What you need to do

To add Product Identifier to your store, follow the steps below:

__1.__ Add `"vtex.product-identifier": "0.x"` to your `manifest.json` dependencies

__2.__ Place the `product-identifier` block anywhere inside your `store.product` or `product-summary.shelf` blocks in the `blocks.json` file

__3.__ Customize the field label and the ID type that should be shown on the store front

[Read more in the app README](https://github.com/vtex-apps/product-identifier)
