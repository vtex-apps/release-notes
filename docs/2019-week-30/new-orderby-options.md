---
title: New ordering options on search result and shelf components
description: "Our search results and shelf components may be sorted by new criteria and their default ordering now is Relevance"
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# New ordering options on search result and shelf components
​
​
## What has changed
​Our search results and shelf products may now be sorted by:

- Name ascending
- Name descending
- Release Date
- Discount
- Relevance

Also, The default value of these two components has changed from "Sales" to “Relevance”.

The shelf component and the search results can have their default order changed (by the store owner) by all these new criteria through the store-front and directly by the blocks.

<img width="200" alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/46JqXbxOVeUa9nqEec63uA/b9067e9de60ca189531363d713c42db4/sort-by-relevance.png">

Before this improvement, it was only possible to sort the products on these components by 
- Sales
- Price: high to low
- Price: low to high

​
## What you need to do

- On the shelf component:

Add the prop `orderBy` to the block on your store with the following options:

- `OrderByTopSaleDESC` - makes shelf be sorted by Sales
- `OrderByReleaseDateDESC` - makes shelf be sorted by Release date
- `OrderByBestDiscountDESC` - makes shelf be sorted by Discount
- `OrderByPriceDESC` - makes shelf be sorted by Price (high to low)
- `OrderByPriceASC`- makes shelf be sorted by Price (low to high)
- `OrderByNameASC` - makes shelf be sorted by Name (alphabetic order)
- `OrderByNameDESC` - makes shelf be sorted by Name (non-alphabetic order)
- `‘’` - defaul value makes shelf be sorted by “relevance”

Or

On the Store front, you may choose this options as well to change the default value


- On the search-results component:

Add the prop `orderByField` to the block on your store with the following options:


- `OrderByTopSaleDESC` - makes search-results be sorted by Sales
- `OrderByReleaseDateDESC` - makes search-results be sorted by Release date
- `OrderByBestDiscountDESC` - makes search-results be sorted by Discount
- `OrderByPriceDESC` - makes search-results be sorted by Price (high to low)
- `OrderByPriceASC`- makes search-results be sorted by Price (low to high)
- `OrderByNameASC` - makes search-results be sorted by Name (alphabetic order)
- `OrderByNameDESC` - makes search-results be sorted by Name (non-alphabetic order)
- `‘’` - defaul value makes search-results be sorted by “relevance”

Or

On the Store front, you may choose this options as well to change the default value

## Side effects

The previous default ordering value was “Sales”. If you already had a shelf or a search result block in your store ordered by the default value, it will change its behaviour and show up sorted by “Relevance” instead of “Sales”.


PRs for reference: 
https://github.com/vtex-apps/search-result/pull/205 
https://github.com/vtex-apps/shelf/pull/160

