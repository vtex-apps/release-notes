---
title: Search Results Page URL
description: "The `preventRouteChange` prop expanded and what was valid only for custom pages is now valid for custom-less Search Results pages. Apply any filters without worrying about changes to the page's path."
date: "11/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-43-44/search-results-page-url.md"
---

# Search Results Page URL 

All Search Results pages, whether custom or not, can now **keep their path unaltered** even when users apply filters.

## What has changed

The Filter Navigator's `preventRouteChange` prop makes it possible to keep page customizations even when new filters are applied on the page, merely changing the URL’s query string instead of the entire URL.

The problem was that until this release, [only custom pages](https://vtex.io/docs/releases/2019-week-32-33/custom-pages-url) paths were exempt from undergoing additional changes when filtered by a user. 

Now, in addition to working on custom pages, this prop can also be applied on non-customized search result pages. 

![search-results-preventroutechange](https://user-images.githubusercontent.com/52087100/68618045-41e81600-04a7-11ea-8310-beb796e202c3.gif)
_Notice that only the search results were reloaded, the page structure remained intact_.

## Main Advantages 

Theis release **prevents a full page reload** for every time that filters are applied, thereby **improving loading time and rendering** for users.

## What you need to do

This improvement is available starting with the [**Search Result**](https://vtex.io/docs/app/vtex.search-result) app version **3.35.5** . Make sure that your store is already running this version or a higher one.
