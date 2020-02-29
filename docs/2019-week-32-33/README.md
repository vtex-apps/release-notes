---
title: VTEX IO Highlights - Week 32&33/2019
description: "See what is new in VTEX IO Week 32&33/2019"
date: "2019-08-22"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-32-33/README.md"
---

# VTEX IO Highlights - Week 32&33/2019

Welcome to the VTEX IO weekly release notes!

Since we were slightly behind schedule with the release, this week’s release notes come in a **double feature format** to put us back on track again!

Without further ado, here’s a sneak peek at key changes made in the last couple of weeks:

> :bell: Keep up-to-date with VTEX IO release notes! Simply click on **Releases only** in this page’s upper right corner **Watch** box.

### New features :rocket:

- [Internal URLs link in banners](internal-urls-link-in-banners.md) - Easily link internal URLs to a banner with the help of CMS’s new Storefront field.
- [accessiBe first party app](accessibe-first-party-app.md) - Get your hands on a first-party integration with the accessiBe solution.
- [Extension points on Order Placed page](extension-points-on-the-order-placed-page.md) - Customize a store’s Order Placed page using extension points.

### Deprecations :x:

- [Pages Settings tab](pages-settings-tab.md) - The Pages Settings tab no is longer available in the CMS section.

### Improvements :heavy_plus_sign:

- [Performance da plataforma](platform-performance.md) - Understand what the VTEX IO performance improvement key points were.
- [Drawer component](drawer-component.md) - Customize your store Drawer’s behavior and appearance using the component’s 3 new props and CSS handles.
- [Breadcrumb on mobile mode](breadcrumb-on-mobile-mode.md) - Make the Breadcrumb component available for mobile users.
- [Image thumbnails](image-thumbnails.md) - Choose whether a product’s thumbnail images will be displayed vertically or horizontally.
- [Custom pages URL changes](custom-pages-url.md) - New browser filter prop which allows custom pages to keep the URLs unchanged even when filters are applied.
- [Search Result](search-result.md) - Display how many items the user is seeing and how many items are left on the search results page.
- [Minicart component](minicart-component.md) - The new Minicart component prop enables redirecting users to any page the retailer chooses when clicking the “Finish Shopping” button.

### Notable bug fixes :bug:

- [Subscription on unavailable products](https://github.com/vtex-apps/store-components/pull/545) - Adding email notifications for when unavailable products are again available no longer gives users an error.
- [Telemarketing Login](https://github.com/vtex-apps/telemarketing/pull/52) - Before this fix, when logging in to a store which had a telemarketing profile, users would encounter problems in rendering the Menu component, which would have stayed behind the Search Bar.
- [Buy-button redirect](https://github.com/vtex-apps/store-discussion/issues/64) - The Buy Button no longer redirects users to an empty cart when the request to add a product to the cart take too long. ℹ️This behavior only was enabled when `isOneClickBuy` was set to `true`.
- _Timeout errors in canonical routes_ - To avoid timeout errors, the canonical routes response wait time was increased. :information_source: This bug fix Pull Request was performed is a private VTEX repository.
- [Storefront carousel schema](https://github.com/vtex-apps/carousel/pull/82) - Carousel schema was reordered in the Admin’s Storefront section in order for image uploads to be displayed first.
- [Icon button inside forms](https://github.com/vtex/styleguide/pull/742) - With this bug fix, you can use an icon button inside a `<form>` without it automatically becoming a submit, saving the form when clicked.
- [Duplicated Minicart items](https://github.com/vtex-apps/minicart/pull/174) - When the same item is repeatedly added by a user to the Minicart, the component will henceforth take the added quantity into account without displaying any bugs.
- [External URLs assignment](https://github.com/vtex-apps/store-discussion/issues/81) - When specified in a `menu-item block` , external URLs no longer lose their query string.
