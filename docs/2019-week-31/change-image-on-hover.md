# Show secondary product image on hover


The [component product-summary](https://github.com/vtex-apps/product-summary), available in the shelf and search-result components, now supports a native hover effect to replace the main product's image by a secondary one

<img width=200 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62786798-bae76400-ba99-11e9-9713-69bb996cf842.gif">





## What has changed 


Prior to this new feature, the product's image on shelf and search-results component would always be static. It's possible now to show another image registered on the main product's SKU when the user hovers over the product image with the mouse. Using this effect brings extra interactivity and a custom experience to your user.


## What you need to do
__1.__ In your catalog, add an specific label to the desired images that will be shown on as the scondary image on hover. It can be done by following [this tutorial](https://help.vtex.com/tracks/catalog-101--5AF0XfnjfWeopIFBgs3LIQ/17PxekVPmVYI4c3OCQ0ddJ)


__2.__ To enable the effect, you must open the Store Front in your admin page. Go to your store's admin, click on CMS, and then Store Front.

__3.__ Go to the Product Summary Image component of the block you want to add the effect. To do so, first find the block you want to edit, for example, the shelf shown below. Then, click on the arrow of the desired component to show its children, then click on the arrow of the component "Product Summary" that might have shown up, and finaly click on the component "Product Summary Image".

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62786941-00a42c80-ba9a-11e9-99bc-54aaeb022848.png">


__4.__ Set the name of the label that you already registered on your secondary images on the catalog over the field "Hover Image Label"

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62787039-38ab6f80-ba9a-11e9-9a73-9fadbca1d8f0.png">


__5.__ Click on Save