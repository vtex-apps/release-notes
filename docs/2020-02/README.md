---
title: VTEX IO Release Notes - February 2020
description: "See what is new in VTEX IO February 2020"
date: "2020-03-16"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-02/README.md"
---

# VTEX IO Release Notes - February 2020

I don't know if it was the extra day we had due to the leap year or the Carnival rest (or should I say *party*? :grimacing:), but something is certain: our wonderful development team was truly inspired in February! 

Brace yourselves... This month's VTEX IO Release Notes is here and you'll need to muster all the energy you can to catch up with everything that has been prepared for you. I really do mean it! Just check it out:

## Special announcements :speaker:

- **Exception for the CSS Selectors deprecation**: Previously, no blocks could be customized by CSS Selectors, remember? This breaking change and the reasons that led to it were announced in the [Release Notes for weeks 43 and 44 of 2019](https://vtex.io/docs/releases/2019-week-43-44/css-selectors-deprecation). Now, this scenario has undergone further changes. Apps that are not yet flexible will be able to CSS Selectors as an exception. They are: `vtex.my-account@1.x`, `vtex.my-orders@3.x` and `vtex.login@2.x`,

- **Changes to the VTEX IO Closed Beta list workflow** -  VTEX IO now has a new workflow to require platform development permissions! [Find out more details](https://vtex.io/docs/releases/2020-02/vtex-io-closed-beta-list) about the change and what you will need to do from now on.

## Features 🚀

- **VTEX init** - The creation of new storefronts using the VTEX IO Store Framework will limit itself to the `store` option when running the `vtex init` command. `store` is a basic boilerplate, unlike the previous Store Theme that already had a lot of preset configurations and customization. Good news for Store Framework beginners!

- **Assets Builder** - A brand new Builder to handle assets that are used in your theme's blocks. Magical! Check out the recipe on [how to configure and use it](https://vtex.io/docs/recipes/development/using-the-assets-builder). 

- **Modal Layout** - The Modal Layout is out and ready for use. Find out how to create modals for your store in its [documentation](https://vtex.io/docs/components/layout-blocks/vtex.modal-layout/).

- **Sticky Layout** -  Endless praise to our dev team that deliver not just one, but two new Layouts releases. You are now able to fix elements in place on the interface, thereby making blocks follow user navigation when scrolling thanks to the [Sticky Layout](https://vtex.io/docs/components/layout-blocks/vtex.sticky-layout/)! 

- **Shelf** - Have you heard the latest? Shelf block is now configured with [Slider Layout](https://vtex.io/docs/apps/layout-blocks/vtex.slider-layout). When listing context, you'll be able to display the desired products in an easier and more practical way. Find out how by reading the [documentation](https://vtex.io/docs/components/content-blocks/vtex.shelf/)!

Still with us? It gets better...

- **Components Debugger** - If you thought you had problems decrypting each component's Handles, the dog days are now over because the Components Debugger has landed. Check out the recipe on [using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization) and begin using the Components Debugger now. 

- **Toolbelt** - A notification is now triggered in your terminal when the `vtex link` command is not running anymore, meaning when your link has died. Can I get an amen? But remember: this new feature is only valid for MAC and Linux at the moment. 

- **Alexa Certify Code** - Natively integrate with Amazon's [Alexa solution](https://vtex.io/docs/components/all/vtex.alexa-certify-code/) now! 

- **Braspag Cybersource Fingerprint** - Make way for there is yet another pixel bringing native integration. It is the  [Braspag's Cybersource anti-fraud](https://vtex.io/docs/components/all/vtex.cybersource-fingerprint/)!

- **UserData Event** -  It's up and running, yes! [Set up the Google Tag Manager UserData Event](https://vtex.io/docs/recipes/store-management/setting-up-google-tag-manager) in your store and verify data related to your store logged in users using the Google Analytics.

## Improvements ➕

- **SEO** - Bad SEO practices? Not here. New URLs that are generated based on a change in a product/category/brand name are no longer indexed by Google even if the content is invalid. Instead, a redirect is created from the old URL to the new one.

- **Order Placed** - Previously, [Order Placed](https://vtex.io/docs/components/content-blocks/vtex.order-placed/readme) was a big monolithic block. Now, Order Placed v2 is launched. Broken into small and customizable blocks, it allows you to customize the order placed page as you wish! Yay! 

- **React app dependencies** - The wise Toolbelt will now automatically update an App React's dependencies located in the app's `package.json` file to keep them in line with Render's dependencies list. Find out more details on this improvement [here](https://vtex.io/docs/releases/2020-02/react-app-dependencies)!

 - **SVG's size** - The `viewbox` prop for [Store Icons](https://vtex.io/docs/components/all/vtex.store-icons/) now accepts other values aside from 16x16px for the following block icons: `search-bar`, `login` and `minicart`.  

- **Header layout** - Making a header layout change when scrolling it sounds unrealistic to you? Let me break it to you... it's not! Open the [Header documentation](https://vtex.io/docs/components/content-blocks/vtex.store-header/) to see for yourself. 

- **Login interface** - New prop for the following area:  `logInButtonBehavior`. It sets the Login block interface either to  `popover` or  `link` . Find out more about its implementation by accessing the [Login documentation](https://vtex.io/docs/components/all/vtex.login/). 

Breathe in and relax, because we still have more... 

- **CSS Handles** - Our constantly acclaimed CSS Handles release is also present this month with new CSS Handles for the [Search Result](https://vtex.io/docs/components/content-blocks/vtex.search-result/) page.

- **Shelf IDs** - The [Shelf](https://vtex.io/docs/components/content-blocks/vtex.shelf/) `trackingId` prop now enables you to identify, using a Shelf ID, which Shelf actually had its content accessed and triggered the Google Analytics event. 

- **Product Images** - Deciding where to position product video on Product Images thumbnails is not an impossible task anymore thanks to the [Product Image](https://vtex.io/docs/components/content-blocks/vtex.store-components/product-images)'s new `contentOrder` prop.  

- **Search Bar** - Previously, you couldn't keep the search icon after entering a text in the search bar. Boring... this scenario changed once the `DisplayMode` prop arrived. Check out the [documentation](https://vtex.io/docs/components/content-blocks/vtex.store-components/search-bar)! 

## Notable bug fixes 🐛

- **[Minicart on hover](https://github.com/vtex-apps/minicart/pull/208)** - Several issues were solved with this one: 1) hovering now only works on desktop mode; 2) When hovered, the Minicart remains open for as long as the user is interacting with it; 3) If the Minicart icon is clicked on, it will behave normally and will be closed when the user clicks outside its area. The Minicart previously had run into some trouble and none of the above were functioning properly...

- **[Measures for product images](https://github.com/vtex-apps/store-theme/pull/197)** - The [Product Summary Image](https://vtex.io/docs/components/content-blocks/vtex.product-summary/product-summary-image) now ensures that the images displayed take up the same space on the interface, having identical measures, regardless of their original size in the Catalog thanks to the new props `height` and `width`. 

- **[Locale Switcher](https://github.com/vtex-apps/locale-switcher/pull/17)** - Long time no see, Locale Switcher... Previously, the block would disappear when the binding default language was used during navigation. Everything was now solved and the block is always present on the interface.

- **Product Impression event** - The Product Impression Event failed to be triggered in two different scenarios: in incomplete [Search Results product aisles]((https://github.com/vtex-apps/search-result/pull/307)) and on the [Related Products Shelf](https://github.com/vtex-apps/shelf/pull/211). everything is working as intended now (and everything triggered as it should be). 

- **[SKU Selector](https://github.com/vtex-apps/product-summary/pull/237)** - Users were being redirected to the SKU page without choosing at least a product specification when on the Shelf or Search Results pages. The new `initialState` prop now comes with the `empty` default value and thus users will only be redirected after choosing specification for the SKU in question.

- **[Product Summary Image](https://github.com/vtex-apps/product-summary/pull/236)** - The `mainImageLabel`, which defines which product image should be present on the Product Summary, didn't change even when users interacted with the SKU Selector. This confused users, since the image didn't necessarily portray the product specifications chosen by the user. This has now changed: the `mainImageLabel` only appears in the product summary when no specification has been selected, meaning that the `initialState` is `empty` (default behavior, thanks to the bug fix above hehe).

