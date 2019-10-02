---
title: Platform performance
description: "Understand what were the VTEX IO performance improvement key points in week35/2019."
date: "06/09/2019"
git: "https://github.com/vtex-apps/release-notes/edit/master/docs/2019-week-35/platform-performance.md"
---

# Platform performance

Check out our latest releases on how to promote an  **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

:eyes: No action for the releases below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## Decrease in CSS bundle size

All spacing, indentation, newlines and comments were removed from CSS assets in VTEX IO production workspaces. With this release, we can reduce, on average, 18% of CSS assets, increasing the **website's speed**.

![before-cssmin](https://user-images.githubusercontent.com/52087100/64426870-25ce8f80-d086-11e9-8469-267dfb3af9df.png)

![after-cssmin](https://user-images.githubusercontent.com/52087100/64426931-48f93f00-d086-11e9-89d3-962781f94d27.png)

---

## Store Components in CSR

Some [Store Components](https://github.com/vtex-apps/store-components) are now rendered using client-side rendering instead of server-side rendering. 

These components are more frequently found in lower page corners, usually seen by users only after scrolling down. The new strategy of making the browser responsible for rendering these components results in these only being rendered **after** the priority content, which is located in the page header and rendered server-side.

The improvement reduces the time needed for rendering the entire content server-side, decreasing the SSR generated payload. This directly impacts the store's **First Contentful Paint**, since it decreases priority content loading time for users.

![storecomponents-CSR](https://user-images.githubusercontent.com/52087100/64426938-4b5b9900-d086-11e9-9a84-348163794860.png)
