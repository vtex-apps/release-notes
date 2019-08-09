# Color name on Sku Selector


Display the name of the color above its image on the SKU Selector


## What has changed 


When the user had to select its product's color on the Product Details Page, he had to rely only on the product's image to understand how it looked. It's possible now to display the name of the color of the SKU beside the variation's name , in order to help the user to choose among the available options.

<img width=160 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62787485-309fff80-ba9b-11e9-85c5-e08528688f8f.png">


## Key advantage
By seeing the color's name along with the product's image, the user can understand better the difference among all variations and leans to make the correct choice


## What you need to do


__1.__ Make sure your store has at least the 3.59.0 version of the app [Store Components](https://github.com/vtex-apps/store-components) installed.


__2.__ Make sure you have the component [Sku Selector](https://github.com/vtex-apps/store-components/tree/master/react/components/SKUSelector) to your [Product Details](https://github.com/vtex-apps/product-details) page block.


__3.__ Configure your Sku Selector block with the following prop:


- `showValueNameForImageVariation`: __boolean__ -  If `true`, show the name for the selected image variation to the right of the variation name. Default value is `false`





