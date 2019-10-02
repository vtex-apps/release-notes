---
title: Platform performance
description: "Understand what were the VTEX IO performance improvement key points for week 37 of 2019."
date: "09/23/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-37/platform-performance.md"
---

# Platform performance

Check out our latest release on how to promote an  **optimal VTEX IO infra performance** and ensuring a better, faster and stabler platform experience:

:eyes: No action for the release below is warranted on your side. The performance improvement is already available to all VTEX IO users!

## Browser requests architecture

Previously, **navigation** requests were performed on the VTEX IO platform through `pages-graphql`. This means that the app would have received the browser request and was responsible for uncovering the route's context, in addition to structuring the requested page and delivering it onto the browser for rendering.

:information_source: Uncovering a context means finding out which content corresponds to the route sent in the browser request.

:information_source: A **navigation** request is a request sent by the browser to the VTEX IO platform based on user navigation on the site. When users click on a category, for example. A **server page** request is a request sent through the browser during the user's first store access. 

Now, any browser request find their way to the `render-server` or `rewriter` first, as was already the case with **server page** requests.

![Arquitetura request](https://user-images.githubusercontent.com/52087100/65434261-e9749080-ddf4-11e9-8e78-3fc00e34d1da.png)

With this release, the platform underwent some important improvements, such as:

- **Architecture consistency**: the flow between VTEX IO services is now the same for any request originating from the browser, be it **navigation** or **server-page**. 
- **Architecture enhancement**: with the requests flow, several services that are dependent on the context ID can work simultaneously with it, without the need to wait for the `pages-graphql` to complete the page construction to deliver such data.  
- `pages-graphql` **optimization** : because it's no longer the service responsible for uncovering the context's ID, `pages-graphql` was optimized, gaining more speed when performing its other tasks within the platform. 
- **Context ID SmartCache improvement**: since contexts were previously uncovered by `pages-graphql`, their cache was damaged, because it was grouped together with the cache of other data also uncovered by the service. Now, context IDs are easily cacheable using `rewriter` or `render-server`.
