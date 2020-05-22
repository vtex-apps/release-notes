---
title: VTEX IO Release Notes - April 2020
description: "See what is new in VTEX IO for April 2020"
date: "2020-05-20"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-04/README.md"
---

# VTEX IO Release Notes - April 2020

The VTEX IO Release Notes is here, team!

Thrilled to announce that this April's Release Notes brings a ton of beautiful releases to enlighten your cloudy days at home.

Let me share an insider's tip with you: *schedule a time of your day to go through it all*... you don't want to get left behind on the **latest key changes on the platform**!

Get a sneak peek at last month's releases:

## Features :rocket:

- [**Overlay Layout app**](https://vtex.io/docs/components/all/vtex.overlay-layout@0.1.2/) - A layout app that provides you blocks to create a dropdown, select or a tooltip component in your store. Sounds amazing and simple... and it actually is!

- [**Condition Layout app**](https://vtex.io/docs/components/all/vtex.condition-layout@1.1.7/) -  You now get to define different layouts for the same page. This one seems like magic but it's not: choose predefined conditions and have the power to decide if a block should be rendered or not.

- [**Seller Selector app**](https://vtex.io/docs/components/all/vtex.seller-selector@0.1.0/) - Marketplace stores will really enjoy from this one: use this app and display the number of [sellers](https://help.vtex.com/tutorial/what-is-a-seller--5FkLvhZ3Few4CWWIuYOK2w) available for each product, enabling users to compare prices and add the desired product to their cart.

- [**Quickorder app**](https://vtex.io/docs/components/all/vtex.quickorder@0.7.2/) - Designed for B2B scenarios, the Quickorder app is here to speed up buying processes by offering tools to process large orders in bulk.

- [**Google Customer Reviews pixel app**](https://vtex.io/docs/components/pixel/vtex.google-customer-reviews@1.0.2/) - A native integration for [Google's service](https://support.google.com/merchants/answer/7124326?hl=en) that collects feedback from customers who’ve made a purchase on your site is now a couple configs away.

- [**Cookiebot pixel app**](https://vtex.io/docs/components/pixel/vtex.cookiebot@2.0.1/) - The native integration for the [Cookiebot solution](https://www.cookiebot.com/) is live. This pixel app is responsible for that handling the privacy and cookie policy for your store.

- [**Iubenda pixel app**](https://vtex.io/docs/components/pixel/vtex.iubenda@0.2.1/) - Three is a charm, isn't it? This pixel provides native integration with the [Iubenda solution](https://www.iubenda.com/en/?utm_source=adwords&utm_medium=ppc&utm_campaign=aw_brand_global_exact&utm_term=iubenda&utm_content=336331123145&gclid=EAIaIQobChMI-ufW1Yid6QIVEYGRCh1zHAmFEAAYASAAEgLP_fD_BwE) that also handles the privacy and cookie policy for your store.

- [**Trustpilot pixel app**](https://vtex.io/docs/components/pixel/vtex.trustpilot@1.0.2/) - Yep, that's right. Fourth pixel app of the evening. This one is for a native integration with the [Trustpilot solution](https://www.trustpilot.com/), responsible for providing your store with review and rating tools.

- [**VTEX Intelligent Search**](https://help.vtex.com/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb) - Get to know the VTEX Intelligent Search application for e-commerce. The new solution provides search components and a brand new Search Engine to assist  customers during their purchase journey in VTEX IO stores. Take a look!

## Improvements :heavy_plus_sign:

- **Public app documentation** - Publish an app on the VTEX IO platform and win a public documentation slot in VTEX IO Docs! This functionality is not new, but its communication is: from now on, Toolbelt (version `2.101.0` or higher) will display the public documentation's link each time an app is successfully published!

- **Toolbelt's commands** - The VTEX IO CLI has undergone an improvement: now, every command has its own `--help` flag. When running `vtex {commandName} --help` in the terminal, you can expect the command's documentation to be shown! 

- **CSS Handles** - Let's talk about good news related to [CSS Handles](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization) for the [Rich Text](https://vtex.io/docs/components/all/vtex.rich-text@0.10.0/) (`tableTr`, `tableTh` and `tableTd`), [Drawer](https://vtex.io/docs/components/all/vtex.store-drawer@0.12.1/) (`opened`, `closed` and `moving`) and the Filter Navigator block (`filtersWrapper` and `filtersWrapperMobile` ) from the [Search Results](https://vtex.io/docs/components/all/vtex.search-result@3.59.0/) app.

- **Product Quantity's unit measurements** - The [Product Quantity app](https://vtex.io/docs/components/all/vtex.product-quantity@1.4.1/) now works with different unit measurements... that's right. Previously, the component would only display products by number of `units`. Now, the default for the new component is to always effortlessly display the product's defined measurement unit, such as `kg`.

- **Modal Layout triggering** - No more repeated content: the modal content displayed from the [Modal Layout](https://vtex.io/docs/components/all/vtex.modal-layout@0.4.2/) app can now be triggered just once during the user session thanks to the new `trigger` prop.

- **Aspect Radio on Product Summary Images** - The [Product Summary Image](https://vtex.io/docs/components/all/vtex.product-summary@2.54.1/product-summary-image/) block has two new props (`maxHeight` and `aspectRatio`) that help display your images in a uniform manner, irrespective of their original size. 
  
- **`search-products-progress-bar` block** - The [Search Results](https://vtex.io/docs/components/all/vtex.search-result@3.59.0/) app now has a new block called`search-products-progress-bar`, which is responsible for displaying a progress bar indicating the total amount of products fetched in the search comparing to the amount being displayed on the page.

- **Sandbox URL** - When using a [Sandbox](https://vtex.io/docs/components/all/vtex.sandbox@0.5.0/) component, it is now possible to open a URL in the same browser tab in which you are navigating.

*Still with us? I hope so, my friend, because our team wasn't fooling around in April...*

- **`back-to-top-button` block** - Brand new [`back-to-top-button`](https://vtex.io/docs/components/all/vtex.store-components@3.114.6/backtotopbutton/) block from the Store Components app redirects users to the top of the page when clicked on. 

- **Query strings in the Store Link's URLs** - Say hello to query string attributes in the [Store Link](https://vtex.io/docs/components/all/vtex.store-link@0.5.1/) blocks! These are now allowed in the URLs used by the component.

- **Event Configurations** - In the [Release Notes for March](https://vtex.io/docs/releases/2020-03/README/), we announced that the Configurations builder allows you to [develop service configuration apps](https://vtex.io/docs/recipes/development/developing-service-configuration-apps/) mainly through routes. Now, the Builder also works with events, which means that you can use the last one to add configurations in your service app.

- **`product-spot-price` block** - The [Product Prices app](https://vtex.io/docs/components/all/vtex.product-price@1.3.0/) just got lucky and gained a new block responsible for rendering the product spot price (the `product-spot-price`) if this price differs from the product selling price.

- **Infocard markdown texts** - Good news: [Infocard block](https://vtex.io/docs/components/all/vtex.store-components@3.114.6/infocard/) has a new prop called `textMode` that supports markdown texts in bold and italic!

- **Infocard links** - Another one for the [Infocard](https://vtex.io/docs/components/all/vtex.store-components@3.114.6/infocard/): the new props `callToActionLinkTarget` and `linkTarget` allow you to control whether the block's links will redirect users to a new browser page or not.

## Removals :no_entry:

- **`vtex install` command** - The `vtex install` command underwent changes to improve the installation flow of apps: now, whenever both version's major and minor have been defined through the command, you'll need to also define the desired patch, meaning that commands such as `vtex install vtex.render-server@8.0.x` won't be able to install the app. To know more about how to properly install an app using Toolbelt, check out our documentation on [installing an app](https://vtex.io/docs/recipes/development/installing-an-app/).

## Notable bug fixes :bug:

- [**Mobile Filter Navigator**](https://github.com/vtex-apps/search-result/pull/334) - A 'close' button was missing by mobile users in the `filter-navigator` block . Now, that button is present once again and users are able to apply or clear filters and finally close the filters window.

- [**Quantity Selector on Shelf**](https://github.com/vtex-apps/product-quantity/pull/13) - The Quantity Selector from the [Product Quantity app](https://vtex.io/docs/components/all/vtex.product-quantity@1.4.1/) was not working when displayed on a Shelf. Although users were choosing a desired quantity for a certain product, this was not being reflected in the Minicart. Now, everything is working as it should.

## Praises :sparkles:

We would not be able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

- [BeatrizMiranda](https://github.com/BeatrizMiranda)
- [felipeireslan](https://github.com/felipeireslan)
- [leoWorkingGood](https://github.com/leoWorkingGood)
- [Lucasayb](https://github.com/lucasayb)
- [marcosewbank](https://github.com/marcosewbank)
- [rayra-alencar](https://github.com/rayra-alencar)

Thank you, team! :muscle:

