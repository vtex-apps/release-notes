---
title: VTEX IO Release Notes - March 2020
description: "See what is new in VTEX IO for March 2020"
date: "2020-04-15"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-03/README.md"
---

# VTEX IO Release Notes - March 2020

Welcome to the March 2020 VTEX IO Release Notes, team.

We've a difficult few days but **together we'll make it**. April is finally here, and with it the hope of positive change and a brand new Release Notes, straight from our world famous oven of ideas :bulb:

Lending credence to the idea the March was not all bad news, we've prepared a Release Notes to show what our team has been up to and to brighten these gray, lonely days a bit.

So wash your hands, sing Happy Birthday twice and cast your eyes on this beauty:

## Features :rocket:

- **Product Gifts app** - A brand new app to display all gifts available to a given product in your catalog. Check out the [documentation](https://vtex.io/docs/components/all/vtex.product-gifts@0.2.0/) and implement this in your store today! 

- **Product Price app** - The [product price block](https://vtex.io/docs/components/all/vtex.store-components/product-price), as we knew it from Store Components app, is now brand new and much more flexible in a new app called Product Price. Give the [documentation](https://vtex.io/docs/components/all/vtex.product-price@1.2.1/) a good read and implement the various blocks that are exported by this app with just a few clicks. 

- **Checkout UI Settings app** - Forget the admin's interface: the new Checkout UI Settings app is here to customize your VTEX IO store's Checkout UI through scripts. Get to know more about its advantages and inner workings by reading the [documentation](https://vtex.io/docs/apps/functional/vtex.checkout-ui-settings@0.0.3). 

- **Configurations Builder** - A service app's configurations can now be allocated as an independent app on the platform, leveraging from the functionality of workspaces, versioning and much more. It may seem complex, but it's not. Have a look at the documentation on how to use the builder to [develop service configuration apps](https://vtex.io/docs/recipes/development/developing-service-configuration-apps/). 

## Improvements :heavy_plus_sign:

- **`menu-item` block from Menu** - The `menu-item` block is not a child composition, which means that menu items don't require a limited list of potential blocks that can declared as their children anymore - as mentioned in the [January 2020 Release Notes](https://vtex.io/docs/releases/2020-01/README/). Due to this change, `menu-item`s can henceforth declare any other Store Framework block in their array as children, granting more [Menu](https://vtex.io/docs/components/all/vtex.menu@2.24.1) customization. 

- **CSS Handles** - New CSS Handles available for the [Search Result](https://vtex.io/docs/components/all/vtex.search-result@3.53.1)'s  `filter-navigator` v3 and for the Store Components' [`sku-selector`](https://vtex.io/docs/components/all/vtex.store-components@3.109.0/sku-selector)! Don't forget to check the CSS Handles table for each documentation!

- **URL structure** - Most of the `map` parameters were removed from URLs, aiming to empower SEO on the platform. Only the `b` parameter was kept on the `map`, due to potential ambiguities between brands and categories. If previously we had something like `storecomponents.myvtex.com/shirts/t-shirts/green/Womens?map=c,c,c,specificationFilter_149,specificationFilter_151`, now we have `storecomponents.myvtex.com/shirts/t-shirts/for-whom_Womens/color_green`. Now this is what I call an improvement, team! 

- **Login** - New `accountOptionLinks` and `termsAndConditions` props for the area responsible for displaying specific account option links to replace the `My Account` and a markdown text below the login options to warn users about Terms & Conditions, respectively. Both are also editable using the admin's Site Editor! Whoopi-ty-doo! Check the [Login app documentation](https://vtex.io/docs/components/all/vtex.login/) for more info on each change.

- **Slider Layout** - `fullWidth`, `autoplay` and `itemsPerPage` props are now available for edition using the admin's Site Editor. Each respectively: 1) defines whether the slides take up the full available width or not; 2) controls the auto-play feature; 3) defines how many slides should be displayed on each device. Access the [documentation](https://vtex.io/docs/components/layout-blocks/vtex.slider-layout@0.11.0/) for more info on each one!

- **Filter Navigator** - The `initiallyCollapsed` prop, which was only accepted by the `filter-navigator.v2`, can now also be configured using `filter-navigator.v3`! Check the [Search Result app documentation](https://vtex.io/docs/components/all/vtex.search-result@3.55.2/).

- **Performance improvements** - We have a significant performance increase for you due to platform changes. The first is related to the [Locale-Switcher](https://vtex.io/docs/components/all/vtex.locale-switcher@0.5.5/). The app and its blocks are now loaded only when under direct interaction with users, thereby decreasing page loading time. The second refers to the Order Form optimization. You can now optimize how your store fetches and uses the Order Form and therefore ensure a smoother navigation experience for your users. If this peaked your interest, have a look at the recipe on [**enabling the Order Form optimization**](https://vtex.io/docs/recipes/store-management/enabling-order-form-optimization/).

- **Store Form** - While the Store Form was incredible and wonderful before, the JSON Schema compatibility was restricted to [Master Data v2](https://help.vtex.com/tutorial/master-data-v2--3JJ1mlzuo88w22gO0gy0QS). Water under the bridge. Thanks to this release, users can now create JSON Schemas that are compatible with Master Data v1 as well! Check out the [documentation](https://vtex.io/docs/components/all/vtex.store-form@0.3.4/).

- **Outline-color** - The `outline-color` CSS property was added to your theme's `style.json` file. It means that you can set a unique default value that can be applied throughout the store for the line that is drawn around all components when they are highlighted on the interface. Previously, you could only set the component's customization in focus individually [using Handles](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization).

## Bug Fixes :bug:

- **Duplicated blocks**: Store Framework was passively accepting a block being declared twice in your store's theme (as long as one was a `.json` file and the other a `jsonc`). This led to various bugs, since only one of the two was going to be effectively rendered... but the developer didn't know which one. An error message is now displayed in Toolbelt whenever the theme is linked and duplicate blocks are present. 

- **[Sensitive Menu](https://github.com/vtex-apps/menu/pull/91)**: It was easy to mistakenly change the Menu you were navigating on since the Hover was way too sensitive. This is now fixed and you can expect a better user experience when using the Menu. Check out the before and after below.

Previously:

![menu-sensitive-before](https://user-images.githubusercontent.com/52087100/79347405-0cd66880-7f0a-11ea-9511-9f39cb62c819.gif)

Now:

![menu-sensitive-after](https://user-images.githubusercontent.com/52087100/79347935-ad2c8d00-7f0a-11ea-8a3f-91356555709f.gif)

- **[`utm_source` on orderForm](https://github.com/vtex-apps/add-to-cart-button/pull/12)** - The expected behavior is for the Add to Cart button to input the `utm_source` data (contained in the user's session) to orderForm, the JSON responsible for storing all the date of an order on the platform. Unfortunately, this was not being done before... but it is now. Cheers!

- **[Specifications Badges](https://github.com/vtex-apps/product-specification-badges/pull/6)** - All the [Specifications Badges](https://vtex.io/docs/app/vtex.product-specification-badges@0.1.0) of a product must be made available to the user... however only the first one configured was being displayed. This fix changes that and now all badges are displayed accordingly.

- **[Telemarketing functionality](https://github.com/vtex-apps/store-graphql/pull/451)** - When a Telemarketing user added products to the cart using a client's account and then switched accounts, the Minicart did not reset, meaning that the OrderForm JSON continued to save the information pertaining to the previous account. This has been fixed: the cart is reset and the OrderForm data is cleared every time the Telemarketing user logs out of an account.
