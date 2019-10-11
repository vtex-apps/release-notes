---
title: Platform performance
description: "Understand what the VTEX IO performance improvement key points were for week 39 and 40 of 2019."
date: "10/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/platform-performance.md"
---

# Platform performance

Check our latest releases for week 39 & 40 of 2019 about promoting an **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

:eyes: No action for the releases below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## Server side rendering 

Previously, the `render-ssr` app, responsible for the server side rendering of the first components seen by users during browsing, would assume that the entire page performed a query.

This behavior led to an overhead in the app when rendering query-less pages, thereby taking more time to load components for users.

The new `render-to-string` app has the same responsibility as `render-ssr`, but in pages that are rendered to users without the need for queries, such as the homepage. This improves **page rendering performance**, directly **impacting the loading time for end users**.

![homepage-avarage-render-time](https://user-images.githubusercontent.com/52087100/66655279-27095400-ec12-11e9-8b94-9da50388b0a6.png)

_The graph above shows a comparison between a homepage's average loading time. The blue line represents the `render-ssr` app avarage time to render all of a homepage's components, while the green line represents the average time  `render-to-string` takes to load the same page._
