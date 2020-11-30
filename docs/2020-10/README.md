---
title: VTEX IO Release Notes - October 2020
description: "See what is new in VTEX IO for October 2020"
date: "2020-11-24"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-10/README.md"
---

# VTEX IO Release Notes - October 2020

While Santa Claus is still not in town, the **VTEX IO Release Notes for October 2020** is the one in charge of delivering lots of goodies for you and delight your home-office days with :sparkles:*joy*:sparkles:!

A tough ask, I know, since there is no end to this terrible and long-lasting virus in our gift basket, but I promise you that our team has prepared some rewards almost as long-awaited as that, such as:

- 🚀 The new Store Locator app
- ➕ Time optimization for hotfix deploys
- 🐛 The fix in the `Add to cart` button performance
 
Caught your attention? 
 
What a question... surely it did! Check out what October 2020 has brought us: 

## Features 🚀

- **Blueknow pixel app** - A new pixel app is out of the oven for the [Blueknow solution](https://www.blueknow.com/en/), responsible for using big data techniques and digital merchandising to provide recovery of lost sales, onsite retargeting, customized recommendations, and more! Check out the [app documentation](https://vtex.io/docs/components/all/vtex.blueknow/) in order to learn how to set it up in your store!

- **Kelkoo pixel app** - The more native integrations, the better: get ready for the [Kelkoo](https://www.kelkoogroup.com/) native integration! The new [pixel app](https://vtex.io/docs/components/all/vtex.kelkoo/) is here to help your store with incremental e-commerce leads!

- **Store Locator app** - If adding information regarding pickup points to your store sounded complicated, it's water under the bridge! The Store Locator is among us to untie the knots in this setup - check out its [documentation](https://vtex.io/docs/components/all/vtex.store-locator/) now!

![store-list](https://user-images.githubusercontent.com/52087100/100130205-33299280-2e61-11eb-9493-cddbee147839.png)

- **Newsletter app** - Display a newsletter subscription form for your store users using the [Store Newsletter app](https://vtex.io/docs/components/all/vtex.store-newsletter/)! Leveraging from the former [Newsletter block](https://github.com/vtex-apps/store-components/blob/master/docs/Newsletter.md) (from the [Store Components app](https://vtex.io/docs/components/all/vtex.store-components/)), this latest and prettier one is here to let bygones be bygones and upgrade your store!

![newsletter-demo](https://user-images.githubusercontent.com/27777263/96277790-1c169b80-0fab-11eb-99cb-6b55ea7f5b7f.png)

- **Condition Layout v2** - The Condition Layout as we know was remodeled in order to achieve a clearer logic when setting the conditions to build your store's layout. In addition to its new [documentation](https://vtex.io/docs/components/all/vtex.condition-layout/), do not forget to access the [migration guide](https://github.com/vtex-apps/condition-layout/blob/master/docs/MIGRATION-GUIDE.md), specially prepared to help you with this upgrade!

## Improvements ➕

- **Time optimization for hotfix deploys** - The VTEX IO team has finally made it possible to warp time exactly as those kids from Dark did in order to deploy your hotfixes in less than 7 minutes! Using the Toolbelt's `2.118.0` version or newer, you can now run `vtex deploy --force` in your terminal when needed. But take note: the `--force` flag is only recommended for hotfixes! Normal deploys should use the `vtex deploy` as usual, since the 7 minutes are fundamental for testing your store's performance.

- **CSS and GraphQL query optimization** - It's what I always say: If it contains performance improvements, then we can call it a good VTEX IO Release Notes! Glad to say that our team has worked really hard on CSS and GraphQL query optimizations and that these are already natively enabled in your store. For more info, check out our documentation on [best practices for optimizing performance](https://vtex.io/docs/recipes/store-management/best-practices-for-optimizing-performance/)!

- **Store performance natively enabled** - If performance improvements are great and loved by everyone, shouldn't they be natively enabled? The VTEX IO team thinks the answer to that is a resounding yes! From now on, all new accounts using the platform will automatically inherit all the currently available store performance best practices. 

- **Sorting products by their collection** - Display products on your store's search results page according to the collection in which they were first sorted! Yep, that's right: the `order-by` block, part of the Search Result app, now works with products' colletions (`OrderByCollection`). Do not forget to learn more about it in the [Search Result documentation](https://vtex.io/docs/components/all/vtex.search-result/)!

- **Error message for JSON parsing** - The lack of additional information was part of the developers' routine whenever something went wrong with parsing the app's JSON files. But not anymore: file and error line references will from now on be displayed in the error message.

![error-message-json-parsing](https://user-images.githubusercontent.com/52087100/100130161-2311b300-2e61-11eb-8e80-75ced8a892ac.png)

- **Render Runtime's typings** - These really are the glory days for VTEX IO developers: you can now count on a marvelous auto-complete feature in your IDE by running the `vtex setup --typings` command to add the Render Runtime's types to your app. For more info, check out the [Render Runtime documentation](https://github.com/vtex-apps/render-runtime)!

- **Error message for Store Form's schema** - Error messages were added to the Store Form app in order to warn developers whenever the JSON schema was invalid, i.e. built with an inaccurate structure! What more can I say? It is safe to claim that the dog days are (*almost*) over for VTEX IO developers!

 - **Submenu navigation** -  Opened submenus are now natively closed whenever another submenu is clicked/hovered on. Previously, the shift between submenus was so fluid that users were not able to notice when content changed - now that's what I call a smooth experience! This behavior was enhanced as shown below:
 
![submenu-closing](https://user-images.githubusercontent.com/52087100/100130209-34f35600-2e61-11eb-85b7-06f9672b2624.gif)

- **Filters closing** - Let's make room for the new `closeOnOutsideClick` prop from the [Search Result](https://vtex.io/docs/components/all/vtex.search-result/)'s `filter-navigator.v3` block, responsible for defining whether the component should be closed with an outside click (as shown below) or not!

![filter-outside-click](https://user-images.githubusercontent.com/52087100/100130163-23aa4980-2e61-11eb-8d85-da15a8ba5103.gif)

- **Zendesk's chat button** - A new Zendesk's chat button was developed to lazy-load the default and heavier one provided by the solution. The replacement button, exported by the [Zendesk Chat pixel app](https://vtex.io/docs/components/all/vtex.zendesk-chat/), can add 15 and 30 points to your Lighthouse score for mobile and desktop devices, respectively. And it gets better: you can also customize the button in your account's admin page.

- **Quantity Selector in dropdown mode** - The Quantity Selector block, exported by the [Product Quantity app](https://vtex.io/docs/components/all/vtex.product-quantity/), can now be rendered as a dropdown thanks to its new prop: the `selectorType`! 

![quantity-selector-dropdown](https://user-images.githubusercontent.com/52087100/100130169-24db7680-2e61-11eb-80f9-1ab98dbc148f.png)

- **Decimal place customization** - Customization is power and we do know that! CSS Handles were added to the product price's decimal places, allowing you to display them half a character above the normal line, and/or in a smaller font.

- **Sitemap extension** - Shall we talk about *SEO* now? Your store's Sitemap can now be extended by other apps, meaning new files can now be natively added to the Sitemap's root XML. Want to know more? Access the [Store Sitemap app documentation](https://vtex.io/docs/components/functional/vtex.store-sitemap@2.13.3/) to keep up with the latest!

## Bug fixes 🐛

- [**`addToCart` event with inaccurate currency value**](https://github.com/vtex-apps/facebook-pixel/pull/16) - The `addToCart` event was displaying misleading data on product prices, harming Facebook tracking tools. The bug was quickly fixed and the currency values are now fetched as they ought to be!

- **[Inconsistency between values in the Minicart](https://github.com/vtex-apps/checkout-summary/pull/38)** - The total value displayed in the Minicart was ignoring the value passed to the `totalizersToShow` prop, generating a mismatch between the values listed and their final sum. This crazy math was adjusted by our team and the total value now respects the vallue passed to the prop!

- **Broken Product Quantity on IE11** - Internet Explorer 11 is one of the browsers supported by the Store Framework, but it seems to me that the [Product Quantity](https://vtex.io/docs/components/all/vtex.product-quantity/) component didn't get that until now... silly component! This disruptive behavior had been fixed and the component now works perfectly for IE11 users as well. 

![quantity-selector-ie11](https://user-images.githubusercontent.com/52087100/100130171-260ca380-2e61-11eb-95da-d9beeacfbc54.png)

- [**Unwanted product specifications being displayed**](https://github.com/vtex-apps/search-resolver/pull/115) - Although we have a checkbox in the Catalog module to set whether a specification should be displayed on the product details page or not, this info was not properly handled in our Product Specifications component. But not anymore: unwanted specifications are now blocked from being displayed when you select this option. This is what I call power of choice, my friends!

- [**`Add to cart` button performance**](https://github.com/vtex-apps/add-to-cart-button/pull/50) - Shopping experience was being harmed because of the unexpected extra time needed to redirect users to the Minicart once the `Add to cart` button was clicked on. Our wonderful team deployed a series of performance fixes and small improvements, such as adding a native loading bar to the page, in order to enhance navigation during the shopping experience! 

- [**Product Highlights**](https://github.com/vtex-apps/product-highlights/pull/4) - The Product Highlights app misunderstood its concept and was displaying *all* collections as highlighted in the store. The undesired behavior was properly fixed, with the component now only displaying collections that have the highlight feature turned on!

## Docs :page_facing_up:

Documentation is the **key**! Check out below our out-of-the-oven docs: 

### Recipes

- [Consulting B2B order statuses](https://vtex.io/docs/recipes/store-management/consulting-b2b-order-statuses/)
- [Safely enabling performance settings](https://vtex.io/docs/recipes/store-management/safely-enabling-performance-settings/)
- [Indicating alternate versions of localized pages in cross-border stores](https://vtex.io/docs/recipes/store-management/indicating-alternate-pages-in-cross-border-stores/)
- [Displaying asynchronous prices](https://vtex.io/docs/recipes/templates/displaying-asynchronous-prices/)

### Concepts

- [Properties](https://vtex.io/docs/concepts/properties/)
- [Composition](https://vtex.io/docs/concepts/composition/)

## Praises ✨

We would not be able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

- [Julio Moreira](https://github.com/juliomoreira) *from B80ne*
- [Gabriel Sampaio](https://github.com/gasampaiosouza) *from econverse*
- [Gustavo Vasconcellos](https://github.com/gustavopvasconcellos) *from ACCT*
- [Felipe Ireslan](https://github.com/felipeireslan) *from ACCT*
- [khrizzcristian](https://github.com/khrizzcristian) 
- [mariusfiliutamindcell](https://github.com/mariusfiliutamindcell)

Thank you, team :muscle:
