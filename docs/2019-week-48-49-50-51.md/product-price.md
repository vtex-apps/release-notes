---
title: Product Price
description: "Shall we celebrate search query's independence from the facets query? Even when the latter doesn't return any results, the former renders data fetched by the `productSearch` query, providing users with search results regardless."
date: "12/19/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/search-query.md"
---

# Product Price

The product Price block just gained a special **new prop**: `blockClass`!

## What has changed

Previously, the Product Price did not accept the `blockClass` prop.  Since blockClass is a prop that functions as a block identifier within your code, all Product Price blocks had to be, before anything else, customized in the same way. 

## Main advantages

With this release, you can **apply specific customizations** for each one of the Product Prices blocks that are part of your theme! 

## What you need to do

It's quick and easy: make sure that the [**Store Components**](https://vtex.io/docs/components/all/vtex.store-components/) app is running version 3.77.0 or higher!
