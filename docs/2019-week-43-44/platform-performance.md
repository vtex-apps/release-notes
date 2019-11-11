---
title: Platform performance
description: "Platform performance improvements are something we always like and want. So give this release a good read to understand what weeks 43 and 44 of 2019 bring in terms of VTEX IO improvement key points."
date: "11/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-43-44/platform-performance.md"
---

# Platform performance

Check out our latest releases for week 40 & 41 of 2019 on promoting an **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

:eyes: No action for the releases below is required on your side. The performance improvement is already available to all VTEX IO users!

## Rendering performance 

Previously, all submenus triggered by users or not were processed for rendering through the platform.

This lead to an **overload** when rendering the store as a whole, which resulted in a **slower loading time** for users.

This release enables a submenu to be processed only when the menu option it is within is actually opened by the user, thus **improving the store's render performance** de 1,75 seg para aprox 620 ms:

- Previously:

![submenu-performance](https://user-images.githubusercontent.com/52087100/68602913-fe30e480-0485-11ea-87f0-8362888ab86c.png)

- Presently:

![submenu-performance-2](https://user-images.githubusercontent.com/52087100/68602946-1143b480-0486-11ea-90f4-ed09f1219702.png)


