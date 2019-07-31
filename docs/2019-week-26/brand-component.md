# Brand component

A new component which shows either the product brand name or product brand logo was released.

## What has changed 

Before the release of this component, it was only possible to retrieve the product’s brand name through the [Product Name component](https://github.com/vtex-apps/store-components/blob/master/react/components/ProductName/README.md), meaning that it was not possible to show a brand name by itself in the Product Details page since the brand data would always be displayed alongside the product name. 

With Brand component, it is now possible to display not only the product’s brand name independently, but also the product’s brand logo, which was not available before.

![brand-component](https://user-images.githubusercontent.com/52087100/60600980-a374d700-9d87-11e9-9f57-e10cbe371577.png)

## Key advantage

The new component provides more flexibility to build your Product Details pages, by showing the product brand name and/or the brand logo in any position on the page with its own css customization.

## What you need to do

__1.__ Make sure your store has at least the 3.47.0 version of the app [Store Components](https://github.com/vtex-apps/store-components) installed.

__2.__ Add the component [Product Brand](https://github.com/vtex-apps/store-components/tree/master/react/components/ProductBrand) to your [Product Details](https://github.com/vtex-apps/product-details) page block.

__3.__ Configure your Product Details Page block with the following props:

- `displayMode`: __string__ - you should choose between “logo” or “text”. This will define whether the product brand will be displayed by name or logo.

- `fallbackToText`: __boolean__ - This prop should only be used when `displayMode` is set to `logo`. It defines what should be done when the Brand Component should have displayed a brand logo but no image was registered in the VTEX Catalog. This prop is set as `true` by default, allowing the logo to be replaced with the brand name in those cases. When set as `false`, the store will not show the brand name instead of the brand logo.

- `height`: __number__ - it sets the logo height. It should only be used when `displaymode` is set to “logo”.

- `excludeBrands`: __array of strings__ - The brand names or brand IDs that are listed in the array will never be displayed by the Brand component. It is usually useful to hide default brand names/logos or test brand names/logos on the store front.

:eyes: Remember that it is necessary to choose between “text” and “logo” in the ‘displaymode’ prop, meaning that __if you want to add both the Brand name and the Brand logo to to your Product Details page, the Brand component should be added twice__, setting the ‘displaymode’ prop to “logo” and “text” each time.
