---
title: Minicart
description: "If there is one thing that a store can always improve upon, it's user experience. The new Minicart `openOnHover` prop is here to make that point."
date: "12/19/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-47-48-49-50-51/minicart.md"
---

# Minicart 

The Minicart just gained the `openOnHover` **prop** that controls whether the block may be opened or not, having the cart information displayed solely, according to the user's hover. 

:warning: **This prop only works properly on desktop mode**. For mobile devices, the behavior continues to be the default one (that is, the Minicart information is only displayed when clicking on it).

## What has changed

Previously, the Minicart **only** displayed cart information when users would clicked on it.

The new prop, when set to `true`, allows users to view the same information with a simple hover:

![minicart-hover](https://user-images.githubusercontent.com/52087100/71182017-097cea00-2254-11ea-86f0-2a43693d36bb.gif)

## Key advantages 

Although this is a release dealing with simple configurations, the Minicart as a block is an important user browsing reference point in stores.

Therefore, the new hover functionality allows users to **access information** contained in blocks **more easily**, improving their **browsing experience**. 

## What you need to do 

Make sure that your [**Minicart**](https://vtex.io/docs/components/all/vtex.minicart/) block is updated to version **2.30.0** or higher.
