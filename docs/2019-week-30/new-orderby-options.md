---
title: A new way to order search results and shelf components
description: "Our search results and shelf components may be sorted according to new criteria and their default order is by Relevance now"
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# New search result and shelf components order options
​
​
## What has changed
​Our search results and shelf products may now be sorted by:

- Name, ascending
- Name, descending
- Release Date
- Discount
- Relevance

Also, the default value of these two components has changed from "Sales" to “Relevance”.

The shelf components and search results can have their default order changed (by the store owner) to any of these new criteria through the store-front and directly through blocks.

<img width="200" alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/46JqXbxOVeUa9nqEec63uA/b9067e9de60ca189531363d713c42db4/sort-by-relevance.png">

Before this improvement, product shelf components could only be sorted according to 
- Sales
- Price: high to low
- Price: low to high

​
## What you need to do

- Regarding the shelf component:

Add the  `orderBy` prop to your store's block with the following options:

- `OrderByTopSaleDESC` - shelf is sorted by Sales
- `OrderByReleaseDateDESC` - shelf is sorted by Release date
- `OrderByBestDiscountDESC` - shelf is sorted by Discount
- `OrderByPriceDESC` - shelf is sorted by Price (high to low)
- `OrderByPriceASC`- shelf is sorted by Price (low to high)
- `OrderByNameASC` - shelf is sorted by Name (alphabetic order)
- `OrderByNameDESC` - shelf is sorted by Name (non-alphabetic order)
- `‘’` - default value; shelf is sorted by “relevance”

Or

On the Store's front, you may choose these options or/and change the default value


- On the search-results component:

Add the `orderByField` prop your store's block with the following options:


- `OrderByTopSaleDESC` -  search results are sorted by Sales
- `OrderByReleaseDateDESC` - search results are sorted by Release date
- `OrderByBestDiscountDESC` - search results are sorted by Discount
- `OrderByPriceDESC` - search results are sorted by Price (high to low)
- `OrderByPriceASC`- search results are sorted by Price (low to high)
- `OrderByNameASC` - search results are sorted by by Name (alphabetic order)
- `OrderByNameDESC` - search results are sorted by Name (non-alphabetic order)
- `‘’` - default value makes search-results be sorted by “relevance”

Or

On the Store's front, you may choose these options or/and change the default value

## Side effects

The previous default ordering value was “Sales”. If you already had a shelf or a search result block in your store which was ordered by the default value, it will change its behavior and show up as sorted by “Relevance” instead of “Sales”.


PRs for reference: 
https://github.com/vtex-apps/search-result/pull/205 
https://github.com/vtex-apps/shelf/pull/160
