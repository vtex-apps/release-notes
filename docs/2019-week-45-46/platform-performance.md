---
title: Platform performance
description: "We always rejoice from performance improvements, and I promise you that this one involving data fetching is legit. Check out the VTEX IO performance improvement for week 45 and 46 of 2019."
date: "11/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/platform-performance.md"
---

# Platform performance

Check the latest releases for week 45 & 46 of 2019 on promoting an **optimal VTEX IO infra performance**, ensuring a better, faster and stabler platform experience:

## Data fetching 

One of the pain points related to platform performance is the GraphQL (responsible for data fetching) **overload**, due to an excessive number of unnecessary requests sent to it.  

Just imagine the following scenario: for a product to be available on a shelf, GraphQL would receive a request to fetch all the SKUs pertaining to that product. In most cases, such a request is unnecessary, since many products have SKUs that are not available and that should therefore not be displayed to users.

As a consequence, the `skuFilter` field was created with the aim to **optimize GraphQL**, reducing its response and thereby considerably **improve store performance**. Its possible values are as follows:

- `FIRST_AVAILABLE`: only returns the **first available SKU fetched in the query**, gaining more than 1s in search speed. This value is recommended for stores that do not use the SKU Selector component on the Shelf or on the search results page.
- `ALL_AVAILABLE`: returns **only available SKUs**. This value was set as the field's default and no further action is necessary if this is the desired scenario for your store. 
- `ALL`: returns **all SKUs for each product** regardless of availability, the same way the former GraphQL behavior did.  
