---
title: Platform performance
description: "Understand what were the VTEX IO performance improvement key points for week 41 and 42 of 2019."
date: "10/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/platform-performance.md"
---

# Platform performance

Check our latest releases for week 41 & 42 of 2019 on promoting an **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

>:eyes: No action for the releases below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## Router authorization performance tweak

Every request on IO must firstly be authorized to proceed through the platform workflow. This ensures that only the accurate apps and the people behind them can access the intended resources they are requesting.  

The infrastructure service responsible for fetching what each user/app can do is called **Sphinx**. With this improvement deploy, **we radically improved the way Sphinx's requests are cached in our router**. 

Since authorization is a great part of the router overhead, we've decreased it by about **40%**, as you can see below:

![router-auth-overhead](https://user-images.githubusercontent.com/52087100/67564592-a9f1da80-f6f9-11e9-9f85-322fc6427875.png)
_The route overhead for all types of requests fell from aprox. 10ms to around 6ms. Bear in mind that this time may vary according to the type of request that was made, for example: if it's an inbound request, if it's a request that required data external to the VTEX IO platform, etc._

Since Sphinx requests can now be cached more in a shorter time-span, and for longer, its request flow drastically decreased: 

![sphinx-request-flow](https://user-images.githubusercontent.com/52087100/67564643-c857d600-f6f9-11e9-98b3-8282ae25483b.png)
_Looking at the graph above, can you guess when we deployed the change? Requests went from around a 150k/min range to about 10k requests/min for the worst scenario._  

From store admins to building and publishing an app: now **everything is faster**! :tada:
