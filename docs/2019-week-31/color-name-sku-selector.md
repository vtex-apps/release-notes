# Color name on Sku Selector


Display the name of the SKU color above its image on the SKU Selector.


## What has changed 

When the user had to select a product's color on the Product Details page, he had to rely only on the product's image to understand how it looked. It's possible now to display the name of the color of the SKU beside the variation's name, in order to help the user to choose among the available options.

<img width=160 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62787485-309fff80-ba9b-11e9-85c5-e08528688f8f.png">


## Key advantage

By seeing the color's name along with the product's image, the user can understand better the difference among all variations and leans to make the correct choice

## What you need to do


__1.__ Make sure your store has at least the __3.59.0__ version of the [Store Components](https://github.com/vtex-apps/store-components) app installed.


__2.__ Make sure you have the [Sku Selector](https://github.com/vtex-apps/store-components/tree/master/react/components/SKUSelector) component in your [Product Details](https://github.com/vtex-apps/product-details) page block.


__3.__ Configure your Sku Selector block with the `showValueNameForImageVariation` prop. When set as `true`, the component shows the color name for the selected SKU variation. :warning: Default value is `false`.





