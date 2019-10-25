---
title: Infinite scroll on flexible Search Result page
description: "No one wants a bad UX, right? Therefore, this deprecation is already deployed and you'll now understand why."
date: "10/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/infinite-scroll-on-flexible-search-result-page.md"
---

# Infinite scroll on flexible Search Result page

The infinite scroll config to fetch more results on flexible search result pages was **deprecated**. From here on out, it will only work on search result pages that do not use Flex Layout. 

![search-result-pagination-als](https://user-images.githubusercontent.com/52087100/66756478-7ea4fb00-ee70-11e9-8ba3-305f8e3bac83.gif)
_Example of infinite scroll being used in the store's Search Result page._

## Why this action is being taken

**The infinite scroll configuration worsens the user experience**, since it effectively never allows users to view the store's footer. 

Since the Search Results component was recently released with the ability to be built using Flex Layout and since none of our clients uses infinite scroll in this new format, the deprecation will not be deleterious to any store. 

However, it serves to make everyone aware of the fact that **the technical team's recommendation is that every store, whether having flexible search result pages or not, opt for the use of a button such as** `Show more`.
  
## What has changed

Following this deprecation, the infinite scroll will be automatically replaced when rendered by a `Show more` button on flexible search result pages. 

Upon inspecting the Search Results page, the console tab will show a warning about the deprecated configuration:

![infinite-scroll-warning](https://user-images.githubusercontent.com/52087100/67563877-05bb6400-f6f8-11e9-9804-e3b39d23cb5f.png)

## Side effects 

This deprecation expects no side effects.
