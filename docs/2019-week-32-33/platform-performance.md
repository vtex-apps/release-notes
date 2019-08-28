---
title: Platform performance 
description: "Overall performance improvements."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Platform performance

Check our latest releases to promote an **optimal VTEX IO infra performance**, ensuring a better, faster and more stable platform experience:

:eyes: No action for the releases below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## • render-server latency decrease

The average `render-server` latency, the service responsible for delivering pages to the browser, was reduced threefold (from around 700ms to 240ms). The impact of this decrease in page delivery time can be felt by end-users mainly on store home pages.

**Previously:**

![IMAGE 1 render server](https://user-images.githubusercontent.com/52087100/63539684-07e32580-c4f1-11e9-8ccf-359c9460e345.png)

**Presently:**

![IMAGE 2 render server](https://user-images.githubusercontent.com/52087100/63539688-09ace900-c4f1-11e9-8537-3696e07c8a6b.png)

--- 

## • Cache increase in Segments requests

Due to an increase in the Segments system requests cacheability, latency for apps that use the Catalog, such as Search and Product Page, was decreased.


![chamadas-segment-cacheadas](https://user-images.githubusercontent.com/52087100/63539856-66100880-c4f1-11e9-9420-dd925ca249d4.png)

:information_source: The Segments system saves user's current session information, influencing what should be displayed from the store.

---

## • Logs architecture improvement

The internal logs architecture was improved, reducing internal infrastructure requests load by about 20k reqs/min.


![IMAGE LOGS](https://user-images.githubusercontent.com/52087100/63539727-1df0e600-c4f1-11e9-8275-717ab49786c2.png)

---


## • render-ssr latency decrease

The average `render-ssr` latency, the VTEX IO service responsible for generating the HTML for page rendering, was decreased from 1300ms to 800ms, approximately.


![image 1 render ssr](https://user-images.githubusercontent.com/52087100/63539746-26492100-c4f1-11e9-9362-19ba571c6aa2.png)


---

## • Optimized number of requests for Messages

The number of requests for Message, the system responsible for translating VTEX IO pages, was optimized, leading to decrease in requests from 1.25M/day to 250K/day.


![otimização-chamadas-messages](https://user-images.githubusercontent.com/52087100/63539876-6dcfad00-c4f1-11e9-8b22-232f8ac3d9d0.png)

---

## • Low browser javascript request rate

With this improvement, the number of javascript requests needed by the browser for loading an IO page in production was decreased. The decrease directly impacts the loading time of VTEX IO pages in production, reducing page rendering time and improving end user browsing experience.
