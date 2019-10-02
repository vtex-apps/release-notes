---
title: Platform performance
description: "Create a web app with more ease with help from Events' expanding functionalities."
date: "09/13/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-36/platform-performance.md"
---

# Platform performance

Check our latest releases aimed at promoting an  **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

:eyes: No action for the releases below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## Request processing performance

The `kube-router`, service responsible for deploying, processing and routing all requests on the VTEX IO platform, was using the `Kubernetes` API to check if a certain app service was actually running before routing a request to it. 

However, the architecture was deeply flawed, as it put the `Kubernetes` API on the requests flow's critical path, even though it should only be used to assess or mutate a cluster state.

With this improvement, `kube-router` now uses DNS resolution to perform this task instead. The DNS is not only much more reliable but also more efficient overall since we have improved the caching logic of those DNS resolutions, resulting in an improvement of around 20% in the `kube-router` routing and request performance.


![dns-router-performance](https://user-images.githubusercontent.com/52087100/64883388-a1f04680-d635-11e9-863d-dde265608c8e.png)
*This graph represents the accumulated time `kube-router` spends calling the `Kubernetes` API, in seconds. As can be seen, we reached a load reduction of more than 4x with this improvement. Notice that the router still calls `Koubernetes` API for other tasks such as service deploys, however the API isn't burdened with the critical path of most requests anymore.*
