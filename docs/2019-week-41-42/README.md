---
title: VTEX IO Release Notes - Week 41&42/2019
description: "See what is new in VTEX IO Week 41&42/2019"
date: "2019-10-25"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/README.md"
---

# VTEX IO Release Notes - Week 41&42/2019

Hey team! One more VTEX IO Release Notes coming your way.

In tune with the Halloween spirit, quick disclosure: more so than ghosts and zombies, my worst fear is not knowing what is going on with VTEX IO 😨 I'm betting you dread the same thing!

Therefore, take a deep breath, relax and banish your fears, because we have a new Release Notes and it's full of delicious treats:

### New features :rocket:

- [Responsive Layout](https://vtex.io/docs/releases/2019-week-41-42/responsive-layout) - Should we start calling ourselves the gods of layout components? The Responsive Layout allows different layouts per breakpoint! It is so awesome and versatile that you'll think it's really godlike.
- [New way to create CSS Handles](https://vtex.io/docs/releases/2019-week-41-42/css-handles-component-development) - Devs, celebrate with me: this release is about a more advantageous, easy and brand new way to create CSS Handles for store components.

### Deprecation ❌

- [Infinite scroll on the flexible search results page](https://vtex.io/docs/releases/2019-week-41-42/infinite-scroll-on-flexible-search-result-page) - No one wants a bad UX, right? Therefore, this deprecation is already deployed and you'll now understand why.

### Improvements :heavy_plus_sign:

- [Platform performance](https://vtex.io/docs/releases/2019-week-41-42/platform-performance) - Understand what were the VTEX IO performance improvement key points for week 41 and 42 of 2019.
- [CSS Handles](https://vtex.io/docs/releases/2019-week-41-42/css-handles) - If you just knew just how much effort our team is putting into making CSS Handles a reality for all store components, you would go to sleep dreaming about CSS Classes. Check out our latest CSS Handles releases!
- [SKU Selector](https://vtex.io/docs/releases/2019-week-41-42/sku-selector) - New SKU Selector props that will allow you to define image height and width without needing to resort to CSS customization. Enhanced performance and practicality in a single improvement: a dream come true.
- [Product Summary](https://vtex.io/docs/releases/2019-week-41-42/product-summary) - Did you enjoy the SKU Selector release? So check out our Product Summary release as well: more props to define image sizes!

### Notable bug fixes :bug:

- [Buy Button redirect](https://github.com/vtex-apps/product-summary/pull/192) - The Buy Button should redirect the user to the PDP regardless of the SKU availability, since users must always know which SKU they are adding to the cart, right? But this wasn't what the button was doing before this fix! It added an SKU to the user's cart, by itself.

- [Price Range loading](https://github.com/vtex-apps/search-result/pull/253) - Any change to the Price Range by the user now triggers a reload symbol, providing a better UX. In addition, the search result pagination now resets when any change to the component is performed. Before this bug fix, these two scenarios were not a reality... how awful!

- [`mailto` and `tel` tags in Menu Item]() - When editing your store's content with Site Editor, you might have come across the `tel:` and `mailto:` tags that could not be read as `href` in a menu item. Now, they are working as originally intended! At long last!

- [Tablet layout grid](https://github.com/vtex-apps/search-result/pull/255) - The Search Result component layout dimensions were not responsive to Tablet devices. They took on mobile dimensions, leading to content decentralization and very weird blank columns on the screen. This layout bug has been fixed.

- [Similar categories in Breadcrumb](https://github.com/vtex-apps/search-graphql/pull/12) - Similar categories to those of the product were being displayed in the Breadcrumb component. Nothing against similar categories, but Breadcrumb isn't the place for that, right? Only the main category tree is now displayed in the component, due to data being fetched in the product's `categoryId`.

- [Image thumbnail gallery arrows in PDP](https://github.com/vtex-apps/store-components/pull/604) - On the Product Details Page, arrows in product thumbnail images were broken when in horizontal mode. These only worked correctly in vertically displayed images! The arrows now understand that they should properly function in both display directions and this bug has been fixed.

- [Site Editor infinite loading](https://github.com/vtex-apps/admin-pages/pull/292) - To allow users to edit a store's blocks using an interface, Site Editor needed to query the code's up-to-date data. Whenever this query encountered an error, the loading symbol was forever displayed to the user, which became confused, poor soul! The loading has now been replaced with an error message, improving the Site Editor UX.
