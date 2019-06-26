# SKU Selector component

From now on, stores with products that require more than two SKU specifications can show all available specification types and its options using the VTEX's SKU Selector component.

## What has changed

Our [SKU Selector component](https://github.com/vtex-apps/store-components/blob/master/react/components/SKUSelector/README.md) used to work properly with products that had only one or two SKU specifications.
 
When a product had SKUs with more than two specifications, the SKU Selector component would only show up the first two specifications returned by the API and hide the others.

For example: when using this component to select a SKU with three specifications (_Color_, _Size_ and _Attribute_), it would only show up the first two specifications (_Color_ and _Size_). 

![image](https://user-images.githubusercontent.com/52087100/60180207-d8b47e80-97f5-11e9-8f28-6d00fb9f155a.png)

With this improvement, the component is now compatible with any quantity of SKU specification. As it is shown below, following the example stated before, __all__ three specifications can now be shown up:

![image](https://user-images.githubusercontent.com/52087100/60180243-ee29a880-97f5-11e9-8f77-e5a15bd5cab6.png)

## Key advantage

__All__ SKU specifications are now fully visible when using VTEX's SKU Selector component. 

## What you need to do

This improvement is available since store-components@3.44.0. Therefore, if your store uses the major 3.x of store-components, this is already available for you.

:eyes: The prop `“hideImpossibleCombinations"` was created with default value `true`. If set to `false`, the option that when combined with others leads to no SKU will be rendered with opacity 20% and it will be unclickable. When set to `true`, that option won't be shown up.

## Side effects

SKUs with too many specifications may have some performance hits.
