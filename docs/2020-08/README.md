---
title: VTEX IO Release Notes - August 2020
description: "See what is new in VTEX IO for August 2020"
date: "2020-09-18"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-08/README.md"
---

# VTEX IO Release Notes - August 2020

It may make a delayed entrance, but it never fails: it's finally here guys :pray:

Did you know that August is called the month of chagrin by some in Brazil? Nonsense....  VTEX IO is here to prove them wrong with this month's release notes. 

A lot of freshly baked wonder-cakes are finally out of our development oven, among which:

- 🚀 The new Disclosure Layout app
- ➕ Change in the app deploying time
- ❌ Product Specifications block deprecation

Wonderful right? And it is not just because I wrote everything here... this month's release notes is so blissful that is would change anyone's mood. Have a closer look:

## Features 🚀

- **Disclosure Layout app** - The Disclosure Layout app is finally among us! The new layout app is responsible for creating a layout structure based on disclosure triggers, as shown below. For more details on the new app, access the [Disclosure Layout documentation](https://vtex.io/docs/components/layout-blocks/vtex.disclosure-layout/).

![disclosure-layout-gif](https://user-images.githubusercontent.com/52087100/93628124-6ca2d500-f9bc-11ea-9a47-cae413459a05.gif)

- **Product Highlights app** - The Product Highlights app is here to allow you to display highlight badges on products according to the collection or promotion they are linked to. To learn how to configure it in your store, check out the [Product Highlights app documentation](https://vtex.io/docs/components/all/vtex.product-highlights/).

![product-highlight](https://user-images.githubusercontent.com/52087100/93628222-91974800-f9bc-11ea-93a1-a9bb7420456a.png)

- **Product Specifications app** - Aiming to bring you more flexibility when using the Product Specifications component, our product team developed the Product Specifications app, replacing the former [Product Specifications block](https://github.com/vtex-apps/store-components/blob/master/docs/ProductSpecifications.md) exported by the [Store Components app](https://vtex.io/docs/app/vtex.store-components). Its setup is just a few clicks away: check out the new [Product Specifications app documentation](https://vtex.io/docs/components/all/vtex.product-specifications/)!

![product-specification](https://user-images.githubusercontent.com/52087100/93628330-c73c3100-f9bc-11ea-95fb-e6974b73774e.png)

- **Product Price block for seller name** - A new block responsible for displaying the seller name next to the product price is among us! Learn how to configure the `product-seller-name` block in your store by accessing the [Product Prices app documentation](https://vtex.io/docs/components/all/vtex.product-price/).

![block-seller](https://user-images.githubusercontent.com/52087100/93628529-15513480-f9bd-11ea-84ee-47ccb84de0db.png)

## Improvements ➕

- **Slider Layout's elements positioning** - The Slider Layout has gained a new prop called `centerMode`, which is responsible for defining how slider elements are positioned on the screen for each device. One of its possible values is `center` which allows you to display your slider element in a centered way to your users, as shown below. This improvement is extremely useful for Shelves and other components that use the Slider Layout for rendering product data. 

![RN-](https://user-images.githubusercontent.com/52087100/93630391-5f87e500-f9c0-11ea-8402-d2f1eba22659.png)

- **Filters display on Search Result page**  -  Thanks to the new `openFiltersMode` prop, you can now define how many filters a user can concomitantly open on the Filter Navigator component.  For more details, access the [Search Result app documentation](https://vtex.io/docs/components/all/vtex.search-result/)!

![filter-selection](https://user-images.githubusercontent.com/52087100/93628732-72e58100-f9bd-11ea-8600-32c0551e4b43.gif)

*Note that only one filter can be opened at any time. In the example above, the prop `openFiltersMode` is declared as `one`.*

- **Bazaar Voice info in Google structured data** -  From now on, user review data fetched by the Bazaar Voice app is considered in Google's structured data, used to understand and gather information about the content of the store's page. This improvement is extremely useful for SEO purposes since google will now be able to effectively fetch product reviews and display them on search result pages.

![bazaar-voice-structured-data](https://user-images.githubusercontent.com/52087100/93628800-8d1f5f00-f9bd-11ea-80fa-41d463991072.png)

- **Markdown interpretation by Assets Builder** - The [Assets Builder](https://vtex.io/docs/recipes/development/using-the-assets-builder) now supports assets whose URLs are built using markdown. This improvement is extremely useful and relevant since block props use the markdown structure to declare media on components.

- **App deploying time**  - Aiming to strengthen the security of our development process, published apps will now have to wait 7 minutes until they become ready to be deployed. Note the following: if this timing is not respected, an `Invalid state transition` error will be received from Toolbelt. For more on this process, check out the [Publishing an app](https://vtex.io/docs/recipes/development/publishing-an-app) documentation.

- **`pageInfo` event on search results page** - Retailers can now benefit from the new search results page event: the `pageInfo`.  Your store's new taggable event is triggered whenever the search results page content is changed due to user interaction, namely: selecting new filters, reordering the results, and clicking on the `Show More` button.

- **EAN in Google Analytics events** - The EAN (product identifier) data is now included in the `addToCart` event. In practice, this means that the VTEX Store Framework now provides EAN data to Google Analytics events, allowing for a deeper analysis and extra integrations.

- **Dynamic content on Slider Layout** - The Slider Layout has gained full dynamic content support! Previously, the component couldn't behave as expected with a dynamic number of slides i.e. when slides were added and removed according to user interaction (as in the case with product-comparison components). The Slider Layout is now adapted to always work as it is configured, regardless of its new content.

- **Minicart v2 automatic display** - A trigger responsible for automatically opening the Minicart v2 on the interface can now be set by using any desired store event and the block's new `customPixelEventId` and `customPixelEventName` props! A long-awaited scenario, in which this new release is extremely useful, is to automatically open the Minicart component whenever the `Add To Cart button` is clicked on by users. Brace yourselves because the wait has finally come to an end: to prettify this release, the `add-to-cart-button` block has also gained a new prop called `customPixelEventId` to broadcast an event of its own when it is clicked on. In practice, this means that you can now set up both `add-to-cart-button` and `minicart.v2` blocks to configure this behavior in your store, displaying the options to move to checkout or  just keep shopping to your users.

*Hold on tight, my friend! Some amazing improvements related to store customization still await you:*

- **Image's non-active dots customization [CSS Handle]** - Previously, we had no CSS handles that would enable users to select and customize non-active dots in the `product-images` block (from [Store Components app](https://vtex.io/docs/app/vtex.store-components/)). Thanks to the new `swiperBullet` and `swiperBullet--active` CSS Handles, an image's non-active dots can now be selected and customized. For more on this, access the [Product Images block documentation](https://vtex.io/docs/components/all/vtex.store-components/product-images/) and our documentation on [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization/).

![image-dot-non-active](https://user-images.githubusercontent.com/52087100/93629085-0fa81e80-f9be-11ea-8fa9-eebbd82bca58.png)

*In the image above only the first image dot, which was currently selected (or active), had both `vtex-store-components-3-x-swiperBullet`  and `vtex-store-components-3-x-swiperBullet--active` CSS classes. The second image dot, which was not active, did not have any CSS class which basically meant that users could not select it for customization.*

- **Product Specifications block customization [CSS Handles]**  - New CSS Handles, namely `specificationsTableRow`, `specificationsTableHead`, and `specificationsTableBody`, were added to the [Product Specifications block](https://github.com/vtex-apps/store-components/blob/master/docs/ProductSpecifications.md), exported by the [Store Components app](https://vtex.io/docs/app/vtex.store-components/), in order to grant you more flexibility while customizing the component's elements.

![css-handles-product-specifications](https://user-images.githubusercontent.com/52087100/93629133-2c445680-f9be-11ea-8170-39ca1b04a780.png)

***Caution**: As previously informed, the Product Specifications block was deprecated and replaced with the Product Specifications app. This release only applies to the former.*

- **Drawer overlay customization [CSS Handles]** -  The Drawer app has gained two new CSS Handles, namely `overlay` and `overlay--visible`, responsible for allowing retailers to customize the overlay structure used by the mobile component. For further details, access this [practical example recorded on loom](https://www.loom.com/share/d4da3624507e464281caae057496a426), as well as the [Drawer app documentation](https://vtex.io/docs/components/all/vtex.store-drawer/).

 - **`nth-child` CSS Selector with step size** - `:nth-child` selectors with step size, such as `:nth-child(2n)` are now allowed when customizing your store with CSS! For more on customizing your store with CSS and HTML selectors, access [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization/#best-practices).
 
## Deprecations ❌

- **Product Specifications block** - The [Product Specification block](https://github.com/vtex-apps/store-components/blob/master/docs/ProductSpecifications.md), pertaining to the [Store Components app](https://vtex.io/docs/app/vtex.store-components/) was deprecated. Although support for this block is still provided, we strongly recommend you to update your store theme with the [**Product Specifications app**](https://vtex.io/docs/components/all/vtex.product-specifications@1.0.1/) in order to benefit from greater flexibility and to keep up with the component's evolution.

## Bug fixes 🐛

- **[Sum of installments without interest on search results page](https://github.com/vtex-apps/search-resolver/pull/84)** - Previously, the search query was presenting price errors when displaying product data on the search results page. As shown in the image below, the sum of installments without interest was higher than the product price itself, leading to a poor and frustrating user experience. The search query for this page was fixed and the bug removed, meaning that the sum of installments without interest is now displayed mathematically correct on search results pages as well as on the product details page.

![installments-bug](https://user-images.githubusercontent.com/52087100/93629964-8abe0480-f9bf-11ea-9141-42e699c1aee1.png)

## Praises ✨

We would not be able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

- [BeatrizMiranda](https://github.com/BeatrizMiranda)  *from ACCT*
- [Lucas Pacheco](https://github.com/lucaspacheco-acct) *from ACCT*
- [Marcos Ewbank](https://github.com/marcosewbank) *from ACCT*
- [Gabriel Carafizi](https://github.com/carafizi1) *from ACCT*
- [Gustavo Vasconcellos](https://github.com/gustavopvasconcellos) *from ACCT*
- [Jayendra](https://github.com/Jayendra88) *from Clouda*

Thank you, team! 💪


