---
title: VTEX IO Highlights - Week 38/2019
description: "See what is new in VTEX IO Week 38/2019"
date: "2019-09-27"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/README.md"
---

# VTEX IO Highlights - Week 38/2019

Did you ever imagine two VTEX IO Release Notes in one week? **we**. **are**. **on**. **fire** 🔥

Hope you will be able to set some time aside from your busy workweek to catch up with VTEX IO one more time.

Check out our key releases for week 38 of 2019 below:

> :bell: Keep up with VTEX IO release notes! Just click on **Releases only** in the **Watch** box in the right upper corner of this page.

### New features :rocket:

- [Fold block](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/fold-block.md) - Can you decide which store's block will be loaded and rendered after the user scroll down? Yes, you can: simply use the Fold block!
- [GraphQL types import](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/graphql-types-import.md) - Save your precious time while developing! From now on, easily import GraphQL types from one app to another.
- [Product Customizer component](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/product-customizer-component.md) - ~(finally)~ Display product attachments in your product page using the Product Customizer component.

### Improvements :heavy_plus_sign:

- [Sandbox with OrderForm](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/sandbox-with-orderform.md) - The user's cart data can now be used in Sandbox components in a fast and simple way.
- [New Toast CSS handle](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/new-toast-css-handle.md) - Customize the Toast component with a different style from the rest of the store thanks to the new CSS handle.
- [Toast component redirect](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/toast-component-redirect.md) - Greater control over user browsing is always magical. Use the `BuyButton` and `ProductSummaryBuyButton` new prop and redirect your user to any URL with a simple click on the Toast component.

### Notable bug fixes :bug:

- [Free products on Google Shopping](https://github.com/vtex-apps/store/pull/360) - Products are no longer being displayed as free on Google Shopping since the issue in our structured data that caused this bug was fixed.
- [`i18n` key props](https://github.com/vtex-apps/admin-pages/pull/279) - When editing `i18n` fields, some users were facing an issue with their key props. There were a few scenarios in which the `i18n` key itself was being rendered raw instead of having its value displayed. This PR solves this issue.
- [`__provideRuntime` cache](https://github.com/vtex-apps/admin-pages/pull/280) = The `__provideRuntime` function called the `Messages` service every time changes to a component were performed by the user, such as changing the Shelf title. To improve request responsiveness (previously at ~2s), this PR adds a local cache that returns the messages and avoids making the request whenever possible.
