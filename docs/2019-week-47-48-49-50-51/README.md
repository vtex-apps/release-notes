---
title: VTEX IO Release Notes - December 2019
description: "See what is new in VTEX IO December 2019"
date: "2019-12-19"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-47-48-49-50-51/README.md"
---

# VTEX IO Release Notes - December 2019

You better watch out, you better not cry, you better not pout and I'm telling you why: **Release Notes** (once again) **is coming to town**!

Given the holiday's never ending glee (and the 117 Fahrenheit if you're in Brazil :sun_with_face:) that December bestows upon us all, the **Christmasy Release Notes** comes in an exclusive format this last month of the year, bringing the best and latest of the past few weeks.

You can call me Santa Claus 'cause once you've read everything you'll feel like you've just found a Christmas tree loaded with **goodies** :christmas_tree: There are so many amazing releases bundled together that I bet you'll go through them as fast as **2019** went by...

### New features :rocket:

- [Reviews and Ratings](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/reviews-and-ratings) - Finally! A product review and rating solution to call our own!!! Say goodbye to the old third-party solution you were using and cast your eyes on this new release.
- [Publish command](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/publish-command) - If you take a deep breath, you can catch a whiff the A/B tests in the air. That’s because the Publish command from 01/02/2020 on will change its functionality and more steps will be added to the process of publishing an app on the platform. Everything to say goodbye to potential instabilities and to foster a culture of tests among our beloved devs.
- [Challenge Trade Policy Condition](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/challenge-trade-policy-condition) - This release was so necessary that you don't even have to be into B2B to rejoice with us: now, you can establish conditional rules to determine whether a user can or cannot access the content of a given trade policy.
- [Blocks on Site Editor](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/blocks-on-site-editor) - We won't deny it... we love it when the Site Editor has a new release. This one's amazing: three more of your store's components can be edited using the Site Editor's admin: Search Bar placeholder, Minicart Icon Label and Product Description title.

### Deprecation :x:

- [Declaring blocks stemming from indirect dependencies](https://vtex.io/docs/releases/2019-12-12/declaring-blocks-stemming-from-indirect-dependencies) - This one was already released and announced, but it's worth letting the crew know once more: Store Builder now requires all blocks that are used in the construction of a store's theme to be defined by the app's direct dependencies, meaning that declaring blocks stemming from indirect dependencies is no longer allowed.

### Improvements :heavy_plus_sign:

- [SKU Selector](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/sku-selector) - Retailers always want power and control over their blocks. Not that I'm judging them, since they're more than right to want as much flexibility as possible for their stores. Therefore, meeting demand, new SKU Selector props (`initialSelection` and `displayMode`) are now here to get rid of block rigidity.
- [Minicart](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/minicart) - If there is one thing that a store can always improve upon, it's user experience. The new Minicart `openOnHover` prop is here to make that point.
- [CSS Handles](https://vtex.io/docs/releases/2019-week-47-48-49-50-51/css-handles) - We get a fuzzy feeling inside whenever a CSS Handles release is nearby! Have a look at our blocks that gained new Handles and are ready to be fully customized: Menu, Flexible Search Result and Product Price.

### Notable bug fixes :bug:

- [Brands on Product Related Shelf](https://github.com/vtex-apps/shelf/pull/199) - The Product Related Shelf product brands were not rendered in the same way as the classic Shelf products. This fix removed this Brand ID preference. Product brand now appear on Product Related Shelves as well, without being discriminated against.
- [Active thumbnail on Product Image](https://github.com/vtex-apps/store-components/pull/641) - The CSS Handle `active`, responsible for customizing thumbnails of images that were selected in the Product Details Page, was ignoring the thumbnail selection. Oh my dear `active`, you had but one job to do! The Handle was only keeping the configured customization for the first image on the list, even if users had selected another image. This has come to an end and the customization now respects the user's power of choice. Hoo-rah!
- [Filter clearing on Mobile](https://github.com/vtex-apps/search-result/pull/283) - What purpose does the `Clear` button serve on a Filter? Clearing all the applied filters, right? But it seemed that `Clear` was the only one not understanding that. The button didn't clear anything, leaving users with the same active filters as before. With this bug fix, the `Clear` button now does what it was meant to do.
- [Filter Sidebar on Mobile](https://github.com/vtex-apps/search-result/pull/282) - When choosing the desired filters for mobile and clicking on `Apply`, the sidebar remained open without serving any purpose to users. If there was bug to be fixed there, it seems it had to do with the mobile Filter. It's now perfect for use: the sidebar's behavior was remedied and it's now closing as expected after clicking on `apply`.
- [Bazaar Voice](https://github.com/vtex-apps/bazaarvoice/pull/24) - Previously, the Bazaar Voice was failing to properly function for the `trackTransaction` event. This led to prices not being sent correctly and to lack of visibility for retailers. How very sad! Everything's back to blossoming for the Bazaar Voice review and sent prices.

---

Words cannot express how glad we are to have you with us on this journey!
Here's to next year and to the incredible releases that awaity :beers:

**Happy Holidays!**
