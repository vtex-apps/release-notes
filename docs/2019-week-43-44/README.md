---
title: VTEX IO Release Notes - Week 43&44/2019
description: "See what is new in VTEX IO Week 43&44/2019"
date: "2019-11-13"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-43-44/README.md"
---

# VTEX IO Release Notes - Week 43&44/2019

Hey team! Another week is dawning!

The start of the week is always the perfect opportunity to set the pace for the week, month and even life, right? We always promise ourselves to start a new diet, or to better organize our tasks, come up with plans and so on...

Funny how we never seem to the energy to do these things on a **Friday** (we tend to have other priorities :smirk:).

Therefore, bask yourself in this **fresh energy** that only the start of the week can bestow upon us to make it through this week's Release Notes :muscle: You’ll understand why in just a second. It’s just that if there is anything you’ll need an abundant supply of in order to catch up with the latest IO updates, it’s energy to read through everything.

See for yourself:

### New features :rocket:

- [Hotjar first party app](https://vtex.io/docs/releases/2019-week-43-44/hotjar-first-party-app) - Forget custom HTML tags and rejoice from the services the Hotjar solution provides. A native integration of the solution with IO stores is now a reality thanks to this new 1st party app.
- [Carousel](https://vtex.io/docs/releases/2019-week-43-44/carousel) - The Carousel component block as we know it makes way for a new Carousel configuration that uses Slider Layout. The more component flexibility, the more customization options available to you!

### Deprecation :x:

- [CSS Selectors](https://vtex.io/docs/releases/2019-week-43-44/css-selectors-deprecation) - The wise Toolbelt has been warning us for the past few days, but you can also read about the deprecation of some Themes CSS selectors here. Check out the details and scenarios that are still allowed.

### Improvements :heavy_plus_sign:

- [Platform performance](https://vtex.io/docs/releases/2019-week-43-44/platform-performance) - Platform performance improvements are something we always like and want. So give this release a good read to understand what weeks 43 and 44 of 2019 bring in terms of VTEX IO improvement key points.
- [Store PWA](https://vtex.io/docs/releases/2019-week-43-44/store-pwa) - Once on the Order Placed page, users want to follow their order’s status. A notice prompting the installation of your store’s PWA seems rather strategic at this point, wouldn’t you say? If you agree, then you'll definitely like this improvement.
- [Menu](https://vtex.io/docs/releases/2019-week-43-44/menu) - If there's something that retailers like, it's code independence. And if there's something we like, it's to see happy retailers! A new configuration of the Menu block allows its content to be edited with Site Editor.
- [Image](https://vtex.io/docs/releases/2019-week-43-44/image) - Similar to the Menu, uploading Image component content can also be done using the Site Editor. Am I hearing fireworks?
- [SKU Selector](https://vtex.io/docs/releases/2019-week-43-44/sku-selector) - The SKU Selector is fully loaded this week: it can not only display exclusive images, but also be wholly displayed on the Shelf and even in the Search Results page. Check out the details here!

Are you still with us? I hope so, because there is more to come:

- [Product Specification](https://vtex.io/docs/releases/2019-week-43-44/product-specifications) - You can choose when and on which device to make the Product Specification content collapsible. So much control over a component can seem like fake news, but it's all true thanks to the new component's prop!
- [Product Summary](https://vtex.io/docs/releases/2019-week-43-44/product-summary) - These past two weeks were not special just for the SKU Selector: the Product Summary didn't just gain a blockClass prop, but also a CSS Handle.
- [Product Summary Price](https://vtex.io/docs/releases/2019-week-43-44/product-summary-price) - Who doesn't like to know how much they saved when buying a product? The Product Summary Price, knowing that the answer to that question is a resounding "everyone", now can display a product's absolute saving to users.
- [Search Results Page URL](https://vtex.io/docs/releases/2019-week-43-44/search-results-page-url) - The `preventRouteChange` prop expanded and what was valid only for custom pages is now valid for custom-less search result pages too. Apply any filters without worrying about changes to the page's path or structure.
- [Site Editor](https://vtex.io/docs/releases/2019-week-43-44/site-editor) - GIFs. Yep, that's right. GIFs. G I F S are now properly working in Site Editor.

### Notable bug fixes :bug:

- [Search Results page buttons](https://github.com/vtex-apps/search-result/pull/264) - The `Fetch previous` and `Show more` buttons were vanishing after being clicked on when the previous search results page was either the first or last page with search results. Witchcraft you say? Whatever the case, we've fixed it. In these scenarios, page loading is now rendered before new results are displayed.
- [Structured data for unavailable products](https://github.com/vtex-apps/structured-data/pull/9) - Unavailable products didn't have their price filled into the page's structured data and were therefore being displayed as free in Google searches. Talk about communication failure :cold_sweat: No unavailable product page structured data will be sent to Google anymore, avoiding erroneous descriptions in the search results and customer confusion.
- [Two tabs Product Specifications](https://github.com/vtex-apps/store-components/pull/610) - The Product Specification component was facing problems when configured to have two tabs. When expanding the first tab's content (by clicking on a `show more` button) and switching between tabs, users were confronted with a `Show less` button, as if they had already opted to expand that second tab as well. This scenario was corrected and the tabs now act independently :muscle:
