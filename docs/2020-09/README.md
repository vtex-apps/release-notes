---
title: VTEX IO Release Notes - September 2020
description: "See what is new in VTEX IO for September 2020"
date: "2020-10-23"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-09/README.md"
---

# VTEX IO Release Notes - September 2020

Just in time: **the VTEX IO Release Notes for September 2020 is finally *among us***!

That being said, your task list from now on consists of:

- Read our hot-off-the-press news.
- Implement the latest and best configs in your store.
- Spread the word to your crewmates about the newest VTEX IO Release Notes.

Easy-peasy... and let me tell you this: our team has prepared so many delightful releases that I'm 100% sure that the above tasks will be done even before tiredness gets to you! No sabotage is allowed!

Shall we?

## Features :rocket:

- **Store Video app** - The Store Video app has arrived, allowing you to display video assets on your store pages with divine features such as auto-play, loop, and mute. It gets even better: the app also supports YouTube, Vimeo, and other third-party players! What are you waiting for? Check out now the [documentation](https://vtex.io/docs/components/content-blocks/vtex.store-video/)!

![store-video](https://user-images.githubusercontent.com/52087100/97001317-8d57d080-150e-11eb-989e-e09b8e61c079.png)

- **Product SKU Attributes block** -  The [Store Component app](https://vtex.io/docs/components/content-blocks/vtex.store-components/)'s brand new block is here to allow you to effortlessly display product SKU attributes. Learn more about it in the [Product SKU attributes documentation](https://vtex.io/docs/components/content-blocks/vtex.store-components/productskuattributes/)!

![product-sku-attributes](https://user-images.githubusercontent.com/52087100/97001314-8cbf3a00-150e-11eb-85c3-b538c42d5d22.png)

- **Facebook Domain Verification app** - The Facebook Domain Verification adds a meta-tag containing the Facebook verification code to your homepage `<head>`, which is used by Facebook for checking your website's ownership. The new app is more than ready to be installed: access its documentation [here](https://vtex.io/docs/components/pixel/vtex.facebook-domain-verification/)!

- **Auto-complete for `product-context` properties** - The TypeScript types of the `vtex.product-context` app are working! Now, if you develop a React app that depends on them, you might run `vtex setup --typings` to have auto-complete and other juicy features that types provide. 

## Improvements :heavy_plus_sign:

- **Performance optimization** - If there is one thing that everyone dreams about, it's performance optimization! With that in mind, the VTEX IO team has prepared a bunch of new configs for you, such as *partial fetching of facets on the search results page* and *CSS concatenation*. The best part is that they are just a couple of clicks away: check out now the documentation on [improving your store's performance](https://vtex.io/docs/recipes/store-management/improving-your-stores-performance/) and apply our best practices in your store!

![cms-store-advanced](https://user-images.githubusercontent.com/52087100/97001256-76b17980-150e-11eb-827f-b91928f4ddf6.png)

- **Repetitive purchase of products** - Before this release, adding the same product to the [Minicart v2](https://vtex.io/docs/components/content-blocks/vtex.minicart/) multiple times was kind of a big challenge for store users. Due to the `Item already on cart` error message, displayed whenever the `Add to cart` button was clicked on more than once, users were being blocked from having a smooth shopping experience. Good thing that loss in sales is not something we condone, nor want. Therefore, users are now able to click on the [Add to cart button](https://vtex.io/docs/components/content-blocks/vtex.add-to-cart-button/) as many times as desired! Cheers to that!

![add-to-cart-loop](https://user-images.githubusercontent.com/52087100/97001241-73b68900-150e-11eb-888f-38a03f042835.gif)

- **Filtering payment methods in the search query** - Thanks to two new props, namely `includedPaymentSystems`  and `excludedPaymentSystems`, it finally became possible to define which payment methods should and should not be taken into account in the search query when displaying the installment options to your store users. Access the [Search Results app documentation](https://vtex.io/docs/components/content-blocks/vtex.search-result/) now and learn how to set these props up in your search results page!

- **Power Review app internationalization** - The [Power Review app](https://vtex.io/docs/components/pixel/vtex.powerreviews/) now works properly with international stores! When globalizing your brand, you no longer need to worry about user reviews in different languages: from this release onward, reviews are automatically fetched, translated, and displayed according to the store locale set by users.

- **Radio and Radiogroup customization** - The Radio and Radiogroup [VTEX Styleguide](https://styleguide.vtex.com/#/Introduction) components have gained these new CSS Handles to call their own: `vtex-radiogroup__fieldset`, `vtex-radiogroup__legend`, `vtex-radiogroup__label`, `vtex-radiogroup__radioContainer`, and `vtex-radiogroup__error`, thus allowing you to customize several store components that are built using them, including [Store Form](https://vtex.io/docs/components/content-blocks/vtex.store-form/) and [Newsletter](https://vtex.io/docs/components/content-blocks/vtex.store-components/newsletter).

- **Sales channel parameter in the `productsByIdentifier` query** - A new parameter was added to the [`productsByIdentifier` search query](https://github.com/vtex-apps/search-graphql/blob/master/graphql/schema.graphql#L216), allowing your custom components to fetch and display products according to the desired sales channel.

- **Item ID as product identifier** - From now on, the [Product Identifier app](https://vtex.io/docs/components/content-blocks/vtex.product-identifier/) also accepts item IDs as product identifiers. Before this release, only Product Reference, Product ID, SKU EAN, and SKU Reference ID were accepted as valid to be displayed on the component.

![product-identifier](https://user-images.githubusercontent.com/52087100/97001233-6ef1d500-150e-11eb-8949-fb5bb60fd306.png)

## Bug fixes :bug:

- [Title attribute missing in image components](https://github.com/vtex-apps/store-image/pull/24) - The title attribute was nowhere to be found in store images. Poor little guy! It was linked to the incorrect HTML element when components were rendered - `a` instead of `img`. This behavior is now fixed and the title attribute can be properly found and tracked.

- [SKU Selector frozen on slider component](https://github.com/vtex-apps/slider-layout/pull/46) - The SKU Selector had its product data frozen when rendered on slider components. In this previous and ugly scenario, users could only update the data displayed either when scrolling the page or when changing the slide currently hovered on. The good thing is that we are close to summer in Brazil and the SKU Selector was defrosted just in time: it is now working as expected!

## Docs :page_facing_up:

Documentation is **key**! Check out our out-of-the-oven docs below : 

### Tracks

- [Desenvolva componentes usando VTEX IO e React](https://vtex.io/docs/getting-started/desenvolva-componentes-usando-vtex-io-e-react/1/) (*Develop components using VTEX IO and React*) - Currently only available in Portuguese!

### Recipes

- [Using events to trigger side effects on store components](https://vtex.io/docs/recipes/templates/using-events-to-trigger-side-effects-on-store-components/)
- [Cross-border store content internationalization](https://vtex.io/docs/recipes/store-management/cross-border-stores-content-internationalization/)
- [Managing landing pages in cross-border stores](https://vtex.io/docs/recipes/store-management/managing-landing-pages-in-cross-border-stores/)
- [Creating robots files for cross-border stores](https://vtex.io/docs/recipes/store-management/creating-robots-files-for-cross-border-stores/)
- [Checking your store’s binding ID](https://vtex.io/docs/recipes/store-management/checking-your-store-binding-id/)
- [Multi-language stores](https://vtex.io/docs/recipes/store-management/multi-language-stores/)
- [Migrating CMS settings after a theme major update](https://vtex.io/docs/recipes/development/migrating-CMS-settings-after-major-update/)
- [Running IO scripts in any VTEX store](https://vtex.io/docs/recipes/development/running-IO-scripts-in-any-VTEX-store/)

### Concepts

- [Billing Option](https://vtex.io/docs/concepts/billing-options/)
- [Cross-border stores](https://vtex.io/docs/concepts/cross-border-stores/)
- [Slots](https://vtex.io/docs/concepts/slots/)

## Praises :sparkles:

We would not be able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

- [Marcos Ewbank](https://github.com/marcosewbank) *from ACCT*
- [Raissa Campos](https://github.com/raissacmp) *from ACCT*
- [Lucas Pacheco](https://github.com/lucaspacheco-acct) *from ACCT*
- [Gabriel Carafizi](https://github.com/carafizi1) *from ACCT*
- [Erislandio](https://github.com/Erislandio) *from ACCT*



