---
title: Custom pages URL 
description: "The new Filter Navigator's 'preventRouteChange' prop enables custom pages paths to not undergo any more changes when filtered by a user."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Custom pages URL

The new Filter Navigator's `preventRouteChange` prop enables custom pages paths to not undergo any more changes when filtered by a user.

## What has changed

Previously, custom static route pages were undergoing changes in their URLs and consequently in their content due to filters applied on them.

The new Filter Navigator's  `preventRouteChange` prop makes it possible to avoid this behavior and to keep page customizations even when new filters are being applied on the page, changing merely the URL’s query string instead of the entire URL.

:eyes: The prop’s default value is `false`. To avoid changes to the page’s path, it should be set to `true`.

## Main advantages

With this new prop, the user’s store experience is improved since browsing a custom page becomes more coherent and seamless, without being subjected to sudden changes because of filters.

## What you need to do

It’s available starting with [**Search Result**](https://github.com/vtex-apps/search-result) app version **3.23.0** . Make sure that your store is already running this version or higher.

:eyes: This prop is only available in `filter-navigator.v1`! Soon on `filter-navigator.v2`.
