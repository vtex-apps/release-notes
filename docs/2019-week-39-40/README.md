---
title: VTEX IO Highlights - Week 39&40/2019
description: "See what is new in VTEX IO Week 39&40/2019"
date: "2019-10-11"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/README.md"
---

# VTEX IO Highlights - Week 39&40/2019

Welcome to the one and only VTEX IO Release Notes!

I bet that you've missed us these past couple weeks, but weep no more 🤗

Not only are we back, but we also have a proper explanation for turning off the lights for all this time: **the VTEX IO Release Notes will have a new format from now on, being published every two weeks**.

No need for the long face, team... a more extended publication time equals more time to bring together relevant content for you 🎉

Without further ado and with the given explanations, have a quick look at our key releases for weeks 39 and 40 of 2019:

> :bell: Keep up with VTEX IO release notes! Just click on **Releases only** in the **Watch** box in the right upper corner of this page.

### New features :rocket:

- Store v2 Edition - No more headaches with manually installing `store` v2 compatible apps thanks to Store v2 Edition.
- [Pickup Availability](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/pickup-availability.md) - New feature for strengthening Omnichannel experience? Oh yeah! Check out the new Pickup Availability component.
- [Paging the Search Results](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/paging-the-search-results.md) - If agility is what you are searching for then this feature is for you. Now, the Search Results component provides a URL for each loaded search results page!
- [Stack Layout](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/stack-layout.md) - Components overlapping other components. If this seems like something difficult, that's because you're unfamiliar with Stack Layout.
- [Tab Layout](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/tab-layout.md) - What's better than one layout release? Two of them. The Tab Layout allow the construction of different layouts for your store's tabs.
- [Product Specification Badges](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/product-specification-badges.md) - Specifications can define whether a user will or will not buy a certain SKU. Don't waste time and display them in badges with this new component!

### Improvements :heavy_plus_sign:

- [Platform performance](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/platform-performance.md) - Understand what the VTEX IO performance improvement key points were for week 39 and 40 of 2019.
- [URL field auto-fill](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/url-field-autofill.md) - When creating a new page in the admin's Page section, the URL field will automatically propose a path according to the page's chosen title. Isn't it just magical?

### Notable bug fixes :bug:

- [Negative discount badges](https://github.com/vtex-apps/store-components/pull/591) - The `DiscountBadge` component was displaying negative discount badges, such as -0%, when the product was being sold at a higher price than its original one. This strange behavior is now fixed and the `DiscountBadge` is not displayed if the product's discount is less than 1%.
- [Attachment default values sent to Checkout](https://github.com/vtex-apps/product-customizer/pull/46) - Product attachment default values were being sent to checkout as if users had chosen them, even though they had not. This scenario no longer occurs.
- [`tel:` Rich Text links attribute](https://github.com/vtex-apps/rich-text/pull/24) - Rich Texts can now interpret the HTML attribute `tel:` to create links for phone calls. Prior to this bug being fixed, this attribute was not interpreted (Rich Texts could only interpret the `mailto` attribute, used for sending e-mails).
