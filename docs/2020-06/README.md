---
title: VTEX IO Release Notes - June 2020
description: "See what is new in VTEX IO for June 2020"
date: "2020-07-16"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2020-06/README.md"
---

# VTEX IO Release Notes - June 2020

Welcome to the VTEX IO Release Notes for June 2020, team! 

I know home office can be ~~extremely~~ a little bit tiring, but I do hope you will be able to set some time aside from your busy workweek to **catch up with VTEX IO latest news**. 

Notice: i'm not saying this only because I'm the one writing the VTEX IO release notes, you know... it's actually because the past month of June really brought us some goodies worth looking at asap, such as:

- :rocket: The new Sitemap app
- :heavy_plus_sign: The 404 pages improvement
- :bug: The Clear button (from mobile filter sidebar) bug fix

Check out the last month's key changes below:

## Features :rocket:

- **Sitemap** - One long awaited tool for SEO is finally out of the oven: manage your website's sitemap file from now on using the new [VTEX IO Sitemap app](https://vtex.io/docs/components/functional/vtex.store-sitemap/). 

- **Image zooming in a modal** - Open a modal for product image zooming whenever the Product Images component (`product-image` block) is clicked on. The instructions for setting up this new feature are available in the Advanced configuration section of the [Product Image block documentation](https://vtex.io/docs/components/all/vtex.store-components/productimages/).

- **Confirmation modal on Minicart**  - Using the [Modal Layout app](https://vtex.io/docs/components/all/vtex.modal-layout/), you can now display a confirmation modal when users decide to remove an item from the minicart. Learn how to configure the confirmation modal in your store by accessing the [Creating modals using icons](https://vtex.io/docs/recipes/templates/creating-modals-using-icons/) documentation.

- **VTEX IO Service Worker management** - Activate and deactivate the native VTEX IO service worker according to your store needs! This feature is a must if you are dealing with a third solution service worker. For more info, access the [Managing VTEX IO native service worker](https://vtex.io/docs/recipes/store-management/deactivating-the-vtex-io-native-service-worker/) documentation. 

## Improvements :heavy_plus_sign:

- **404 pages** - The 404 pages feature was remodeled. It was already possible to natively enable 404 pages for nonexistent product pages and for URLs that have more than one invalid segment. But in addition to that, you can now also allow 404 pages when URLs have a single invalid path segment. Cheers to that! Learn more about this setup in the [Enabling 404 pages](https://vtex.io/docs/recipes/store-management/enabling-404-pages/) documentation.  

- **Checkbox buttons customization**  - New CSS Handles were added to the VTEX Styleguide in order to simplify the Checkbox button customization, such as those ones used in filters from the search results page, namely `vtex-checkbox__box-wrapper`, `vtex-checkbox__box`, and `vtex-checkbox__input`. For further details, do not forget to check out the [VTEX Styleguide](https://styleguide.vtex.com/). 

- **Price Range component customization**  - A new CSS Handle called `vtex-slider__base-internal` was also added to the VTEX Styleguide in order to simplify the customization of the Price Range component, rendered on the Search Result page. As previously recommended, you can access the [VTEX Styleguide](https://styleguide.vtex.com/) for more info. 

- **Search bar in modals** -  Displaying a search bar in a modal using the [Modal Layout app](https://vtex.io/docs/components/all/vtex.modal-layout/) and the  [Search Result](https://vtex.io/docs/components/all/vtex.search-result/) block `search-bar` was already possible. Now, however, the modal is immediately closed when a search is performed by users, enhancing their navigation experience.

- **Product Specifications customization** - It became possible to apply CSS classes for each product specification displayed on the interface, allowing for their independent customization. This marvel of a release is all thanks to the way CSS Handles (used by the [Product Specifications](https://vtex.io/docs/components/all/vtex.store-components/productspecifications/) block) currently behave when inspected. 

- **Product Summary Name heading tags**  - Forget about when a single heading tag was mandatory: using the new `tag` prop, you can now choose which heading tag should be applied when rendering the Product Summary Name block.  Don't forget to check out the [block documentation](https://vtex.io/docs/components/all/vtex.product-summary/product-summary-name/). 

- **Add To Cart Button text label** - We really mean to empower our users: decide which text should be displayed on the Add To Cart Button using its new props `text` and `unavailableText`. For more, access the [Add To Cart Button documentation](https://vtex.io/docs/components/all/vtex.add-to-cart-button/). 

- **Add To Cart Button behavior** - One more for the Add To Cart Button: thanks to its new prop `onClickBehavior`, you can now set the button's behavior once it is clicked on, defining whether it will redirect users to the product page or directly add the given product to the minicart.  Check out more in the [Add To Cart Button documentation](https://vtex.io/docs/components/all/vtex.add-to-cart-button/).

*Still with us? We are just half way there! Hold on tight, because we still have some great improvements to show you:*

- **Product Summary Buy Button behavior** - We're really improving some buttons here, aren't we? The `product-summary-buy-button` block, exported by the Product Summary app, has a new prop called `buyButtonBehavior` that defines the button's behavior when clicked on. Understand which behaviors are accepted by accessing the [Product Summary Buy Button documentation](https://vtex.io/docs/components/all/vtex.product-summary/product-summary-buy-button/).

- **Open Graph meta tags** -  Open Graph meta tags (used by Facebook) are now available in the `store.home`, `store.product`, and `store.search` templates (respectively home, product, and search result pages). These tags are extremely useful when these pages are shared on Facebook, since they're used to display rich previews to users. 

- **CSS Handles for Search Result** - A VTEX IO release notes is not a proper one if it does not include new CSS Handles. `filterBreadcrumbsItem` and `filterBreadcrumbsItemName` were added to the [Search Result app](https://vtex.io/docs/components/all/vtex.search-result/), allowing for the customization of filter breadcrumbs on mobile devices. 

- **CSS handles for Search Bar** - Another CSS Handles release to make you smile: the [Search Bar block](https://vtex.io/docs/components/all/vtex.store-components/searchbar/), exported by the [Store Components app](https://vtex.io/docs/components/all/vtex.store-components@3.119.6/), gained new handles responsible for customizing the search bar component specifically when it is opened and/or filled out by users. 

- **Quantity badge behavior on Minicart** - The `minicart.v2` block, part of the Minicart app (v2), received a new prop called `itemCountMode`. This new prop is responsible for defining the quantity badge's behavior when displaying the number of items added to the Minicart.  Understand which behaviors are accepted by accessing the [Minicart app documentation](https://vtex.io/docs/components/all/vtex.minicart/).

- **Minicart icon** - Flexibility is what we aimed for this past month! Thanks to the new `MinicartIcon` prop, you can now change the Minicart icon (v2) by choosing from the icons exported by the [Store Icons app](https://vtex.io/docs/components/all/vtex.store-icons/). Check out the [Minicart documentation](https://vtex.io/docs/components/all/vtex.minicart/) in order to learn how to use this new prop. 

- **Progress bar on the search results page** - The `search-products-progress-bar` block, responsible for displaying a progress bar for product results on the search results page, can now be declared as a child of the `search-result` block from the previous version of the [Search Result app](https://vtex.io/docs/components/all/vtex.search-result/). Previously, it only could be declared as a child of the `search-result-layout` block pertaining to current version of the app. 

## Bug fixes :bug:

- **[Clear button from mobile filter sidebar](https://github.com/vtex-apps/search-result/pull/376)** - The Filter sidebar's `Clear` button was not properly working on mobile devices, since it was not properly clearing filters applied by users. This behavior has been fixed and the button now clears every checked filter.  

- **[Assembly options selection](https://github.com/vtex-apps/product-customizer/pull/67)** - Previously, assembly options were only selected if the user clicked on the Radio button/checkbox. In order to improve user experience, assembly options are now duly selected whenever users select them (whether using the buttons or not). 

- **[Newsletter's email address field](https://github.com/vtex-apps/store-components/pull/790)** - Spaces unintentionally added to the [Newsletter](https://vtex.io/docs/components/all/vtex.store-components@3.119.6/newsletter/)'s email address field were invalidating user subscriptions. The component no longer accepts spaces in the field, thus improving user experience.

- **[Search Result's custom query](https://github.com/vtex-apps/search-result/pull/359)**  - The `search-result-layout.customQuery` block, exported by the [Search Result app](https://vtex.io/docs/components/all/vtex.search-result/) and responsible for performing custom queries to the Search API, was not properly working when declared in a column built by the [Flex Layout app](https://vtex.io/docs/components/all/vtex.flex-layout/). This unwanted behavior is now fixed. 

## Praises :sparkles:

We would not be able to deliver so many amazing results during this last month if it were not for the following outstanding contributors:

-   [BeatrizMiranda](https://github.com/BeatrizMiranda)  _from ACCT_
-   [gustavopvasconcellos](https://github.com/gustavopvasconcellos) _from ACCT_
-   [ygorneves10](https://github.com/ygorneves10) _from Corebiz_
-   [igorpoubel](https://github.com/igorpoubel) _from Corebiz_

Thank you, team :muscle:
