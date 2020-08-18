---
title: VTEX IO Release Notes - July 2020
description: "See what is new in VTEX IO for July 2020"
date: "2020-08-17"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-07/README.md"
---

# VTEX IO Release Notes - July 2020

Make room for the VTEX IO Release Notes - July 2020 version, team!  

It is time to step aside from all the world's craziness and restfully read the goodies brought to us in the past month by the VTEX IO team.   

Stretch your legs, take a deep breath and a sip of coffee: you are about to reach the high-point of your August home-office days with our ***latest news**!

Some of the key changes include:

- 🚀 The new `font-faces.css` file in Store Theme
- ➕ Product Price blocks for installment options
- ❌ Animation and Slider blocks deprecation
- 🐛 Related Products Shelf rendering on mobile devices fix

*And much more*. Cast you eyes on these freshly baked releases right now:

## Features 🚀

- **Cookie Script pixel app** - A VTEX [Cookie Script](https://cookie-script.com/) native integration is now available for your store, making your website cookies comply with GDPR and CCPA. Learn how to install it by accessing the [Cookie Script app documentation](https://developers.vtex.com/docs/vtex-cookie-script). 

- **Tawk.to pixel app** - Another pixel app on the front lines: a [Tawk.to](https://www.tawk.to/) native integration is also now available for your store. It allows you to monitor and chat with visitors on either your website, mobile app, or from a free customizable page. Learn how to install it in your VTEX account by accessing the [Tawk.to app documentation](https://developers.vtex.com/docs/vtex-tawk-to).

- **Elfsight pixel app**  - They say three is a charm, don't they? A VTEX [Elfsight](https://elfsight.com/?gclid=EAIaIQobChMI4Yejsrnh6gIVVQmRCh0UPgQJEAAYASAAEgIvR_D_BwE) native integration is available, providing widgets to increase sales, engage visitors, collect leads, and more. Learn how to install it in your VTEX account by accessing the [Elfsight app documentation](https://vtex.io/docs/components/pixel/vtex.elfsight/).

- **OneSignal pixel app** - What do we call it? Four is a blast? I think so! A [OneSignal](https://onesignal.com/) native integration is among us, providing web push notifications for customer engagement. Learn how to install it in your VTEX account by accessing the [OneSignal app documentation](https://vtex.io/docs/components/all/vtex.onesignal/).

- **New `font-faces.css` file in the Store Theme app** - Create a CSS global file specifically for your store's fonts and change your store's typography according to your business needs using your Store Theme app code. But keep in mind: the `font-faces.css` file is now mandatory when changing your store's typography using your store theme code, meaning you can no longer upload fonts directly in the app's CSS by overriding files. For more on this topic, access the [Customizing your store's typography](https://vtex.io/docs/recipes/style/customizing-your-stores-typography/) documentation.

## Improvements ➕

- **Product spot price in Google structured data** - The product spot price is now considered in the  `lowPrice`  field from Google structured data, used to understand and gather information about the content of the store page. This improvement is extremely useful for stores that use Google Shopping, since it will now be able to effectively fetch the product's lowest price (meaning the spot price). 

- **Product spot price on search results page**  - The product spot price is really deciding to come out. It is now displayed on the store's search results page (whether the store uses VTEX Intelligent Search or the former search solution). 

![spot-price-search-results](https://user-images.githubusercontent.com/52087100/90401143-ec631a00-e073-11ea-92c6-c95bf163da4b.png)
*Previously, the product spot price was only available for product detail pages.*

- **Order custom tax data in the `dataLayer` object** -  New fields were added to the `dataLayer` object, allowing the store's website to export data related to the order custom taxes. This improvement is extremely useful for stores wishing to handle order custom tax data in Google tracking mechanisms, such as Google Analytics.

- **Product Price blocks for installment options** - The Product Price component now displays all the available installment options according to the desired payment method, thanks to the new blocks `product-installments-list` and  `product-installments-list-item`. Previously, the Product Price component only rendered the max number of installments, regardless of the payment method. For more, do not forget to access the [Product Price app documentation](https://vtex.io/docs/components/all/vtex.product-price/).

- **Assets builder's file paths in CSS files**  - Media uploaded on Assets builder can now be referenced in your store theme CSS files by adding the accurate file path. Previously, file paths from Assets builder only worked in `blocks.json` and `blocks.jsonc` files. For more on this topic, check out the [Using the Assets Builder](https://vtex.io/docs/recipes/development/using-the-assets-builder/) documentation.

- **List price presentation on product selling price** - The `hasListPrice` prop was added to the `product-selling-price` block from the [Product Price app](https://vtex.io/docs/components/all/vtex.product-price/). It is responsible for defining whether the product should display its [list price](https://help.vtex.com/en/tutorial/prices-v2--tutorials_4393?locale=en) (if any) on its selling price or not. 

![rn-no-list-price](https://user-images.githubusercontent.com/52087100/90403203-fc302d80-e076-11ea-972d-25ed247092c4.png)
*Product selling price with no list price being displayed.*

![rn-with-list-price](https://user-images.githubusercontent.com/52087100/90403199-f9353d00-e076-11ea-92c8-5ff3d1d339cb.png)
*Product selling price with the list price also being displayed.* 

- **Submenu customization per user navigation [CSS Handles]** - New CSS Handles with modifiers (`submenuWrapper--isOpen`  and `submenuWrapper--isClosed`) were added to the [Menu app](https://vtex.io/docs/components/all/vtex.menu/), making it possible to create animation effects when the submenu opens and closes according to the user navigation. For more on how to properly use CSS Handles, access the [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization) documentation.

![submenu-handle](https://user-images.githubusercontent.com/52087100/90402269-98f1cb80-e075-11ea-9331-923a21655df2.png)
*Notice how the menu animation showed above only works because the `submenuWrapper--isClosed` Handle is being applied.* 

- **Shelf slide dot customization [CSS Handle]** - A new CSS Handle (`dot--isActive`) was added to the [Shelf app](https://vtex.io/docs/components/all/vtex.shelf/), enabling the customization of the shelf active slide dot.

![shelf-handle](https://user-images.githubusercontent.com/52087100/90402463-db1b0d00-e075-11ea-8a05-740609e7015e.png)
*The shelf slide dot highlights the shelf slide currently being hovered on by users.*

We already are half way through! Hold on tight, some marvelous improvements still await you:

- **Filter Navigator customization on mobile devices [CSS Handles]** - New CSS Handles were added to the [Search Result app](https://vtex.io/docs/components/all/vtex.search-result/) to enable the Filter Navigator component customization on mobile devices. They are, namely: `accordionFilterContainer` , `accordionFilterContent`, `filterBreadcrumbsContent`, and `filterBreadcrumbsText`. 

- **Search results page customization per display mode [CSS Handles]**  - It became possible to apply CSS classes to search results according to the way they are displayed on the interface! This release marvel is all thanks to the way `galleryItem` CSS Handle (exported by the [Search Result app](https://vtex.io/docs/components/all/vtex.store-components/productspecifications/)) presently behaves when inspected.  It now accepts an HTML modifier  (`{displayMode}`) meaning that the handle name changes according to the display mode used to render search results. 

![release-displaymode-modifier](https://user-images.githubusercontent.com/52087100/90401469-5bd90980-e074-11ea-97d7-9ab0774af624.png)
*In the example above, the CSS Handle `galleryItem` presents itself as `galleryItem-inline` when inspected. Notice that the new Handle name is defined according to the display mode set on the search results page.*

- **Product Images' active slide dot customization [CSS Handles]** -  A new CSS Handle (`swiperBullet--active`) was added to the [Product Images block](https://vtex.io/docs/components/all/vtex.store-components/productimages)(from the [Store Components app](https://vtex.io/docs/components/all/vtex.store-components/)), enabling the customization of the active slide dot. This handle is extremely useful for scenarios where the Product Images block is used to build a slider component, such as a [Carousel](https://vtex.io/docs/recipes/templates/building-a-carousel-using-slider-layout).

![rn-swiper-product-images](https://user-images.githubusercontent.com/52087100/90403392-4dd8b800-e077-11ea-857c-334396b6ece8.png)
*The slider active dot highlights the slide currently being hovered on by users.*

- **Search result's Order By customization [CSS Handles]** - A new CSS Handle (`orderByOptionItem--selected`) was added to the [Search Result app](https://vtex.io/docs/components/all/vtex.search-result/), allowing you to customize the item selected by users on the page's Order by component. 

![rn-order-by-handle](https://user-images.githubusercontent.com/52087100/90404114-4bc32900-e078-11ea-8e33-259d9c9db50c.png)

- **Seller Selector context** - Other VTEX Store Framework apps can now use the context exported by the [Seller Selector app](https://vtex.io/docs/components/all/vtex.seller-selector/) (`SellerContext`) regarding seller data by using the `import { SellerContext } from 'vtex.seller-selector'` expression in the Store Theme code.

 - **Breadcrumb structured data** - Previously, neither the [Breadcrumb app](https://vtex.io/docs/components/all/vtex.breadcrumb/) nor the store itself provided the `position` and `itemListElement` data necessary to guide search engines to the current page position in the store category tree. The Breadcrumb app is now configured to have [structured data](https://developers.google.com/search/docs/guides/intro-structured-data), improving your store's SEO.

## Removals ⛔

- **Back button as modal closing button** - The browser's Back button no longer works as a modal closing button when configuring the [Modal Layout app](https://vtex.io/docs/components/all/vtex.modal-layout/). This feature was extremely useful for users from mobile devices since the modal opened in them works as a brand new page. In the meantime, it was leading users to a poor experience when using desktop devices since the Back button wasn't taking users to the previous page as expected. Instead, it only closed modals (if any on the page). In order to improve the website navigation, this feature was removed, meaning that the Modal Layout now depends on its own button in order to be properly closed.

## Deprecations ❌

- **Animation and Slider blocks** - The [Animation](https://github.com/vtex-apps/store-components/blob/master/docs/Animation.md) and the [Slider](https://github.com/vtex-apps/store-components/blob/master/docs/Slider.md) blocks, pertaining to the [Store Components app](https://vtex.io/docs/components/all/vtex.store-components/) were deprecated. Although support for both blocks is still provided, it is strongly recommended to update your store theme with the [Slider Layout](https://vtex.io/docs/components/layout-blocks/vtex.slider-layout/) block in order to keep up with the Slider component evolution.  

## Bug fixes 🐛

- **[Product variation sorting on SKU Selector](https://github.com/vtex-apps/store-resources/pull/123)** - Previously, the SKU Selector rendered in a Product Summary Component ([`product-summary-sku-selector` block](https://vtex.io/docs/components/all/vtex.product-summary/product-summary-sku-selector/)) did not respect the Catalog data when displaying product variations. As a result, product variations didn't have a specific sorting when displayed to users, leading to a poor UX.  This unexpected behavior is now fixed and the SKU Selector now presents the variations according to how they are ordered in the Catalog module.

- **[`hideImpossibleCombinations` prop behavior](https://github.com/vtex-apps/store-components/pull/828)** - Before this fix, [SKU Selector](https://vtex.io/docs/components/all/vtex.store-components/sku-selector/)'s `hideImpossibleCombinations` prop was not properly hiding impossible specifications (specifications that can't be chosen according to the filter previously selected) when defined as `true` in certain scenarios. In addition, when the prop value was  `false`, impossible specifications were not being displayed by the component in an intuitive way. These behaviors are now fixed and the prop is working as expected, improving user experience when using the SKU Selector component. Check out this [link](https://www.loom.com/share/2f11b9f6ae6c4bcf9f23380d3f8bf9eb) to watch a practical demonstration of this bug and its fix.

- **[Slider Layout's slide navigation](https://github.com/vtex-apps/slider-layout/pull/34)** - The [Slider Layout app](https://vtex.io/docs/components/all/vtex.slider-layout/) has gone through fundamental changes in order to improve its usability and therefore the user's experience on it. Previously, the component was showing a mobile delay (mobile users were facing a delay when sliding across products by swiping instead of using the arrow buttons) and a rewind effect (due to the lack of an infinite scroll feature, the component was presenting a rewind effect, taking users back to the *first* displayed product when the *last* one was presented). Both issues were addressed and fixed! Cheers to that! Now the Slider Layout automatically works with a smooth slide transition (infinite scroll effect) and also quickly responds to user interaction on mobile devices.

- **[Related Products Shelf rendering on mobile devices](https://github.com/vtex-apps/shelf/pull/227)**  - Due to an implementation detail in the `isMobile` prop, the [Related Products Shelf component](https://vtex.io/docs/components/all/vtex.shelf/) was only being rendered in its desktop mode, even when displayed on mobile devices. This undesirable behavior is now fixed and the Related Products Shelf is working for mobile users as expected.

## Praises ✨

We would not have been able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

- [BeatrizMiranda](https://github.com/BeatrizMiranda)  *from ACCT*
- [Matheus Araujo](https://github.com/MatheusR42) *from Corebiz*
- [Sahan Jayawardana](https://github.com/sahanljc) *from Clouda Inc*

Thank you, team! 💪


