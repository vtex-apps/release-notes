---
title: Search Result OrderBy
description: "OrderBy’s new `hiddenOptions` prop does away with the component’s forced exhibitionism. Its options can now either be hidden or displayed according to the retailer’s chosen scenario."
date: "11/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/search-result-orderby.md"
---

# Search Result OrderBy

OrderBy's new `hiddenOptions` prop now allows the component's options to be **hidden** from user view. 


![orderby-gif](https://user-images.githubusercontent.com/52087100/69576047-47b32080-0faa-11ea-9436-1c9f860b34e4.gif)
_Exemple of OrderBy component displaying all order results options._

## What has changed

Prior to this release, you could not determine which options OrderBy should or should not display, due to the fact that all were **hardcoded** by the component.  

The new `hiddenOptions` prop allows you to configure the block so that options can be hidden when redering the component. 

## Main advantages

VTEX's search context necessarily supports ordering products by all options provided by OrderBy, however other search engines/systems may not support it, forcing retailers to display an option which does not return any results to users.

While most stores use VTEX's search system, OrderBy's lack of flexibility tied all stores to it, whether out of the retailers own volition or not.  

The new prop therefore offers retailers **greater freedom** and makes the **component adaptable** to the store's different business scenarios. 

## What you need to do

Make sure that your store is running [**Search Result**](https://vtex.io/docs/app/vtex.search-result) version **3.38.0** or higher.
