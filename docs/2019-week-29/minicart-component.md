---
title: Minicart component
description: "The minicart component can now display the total cart item quantity and value."
date: "24/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Minicart component

Thanks to two new properties, the Minicart component now can display the **total cart item quantity and value**.

## What has changed

Previously, the Minicart component could only show the **quantity for different items** added to the cart. This means that if two identical shirt and one pair of pants were added to a cart, the Minicart would mislead the user by displaying only **2** items. Also, viewing the total cart value was not possible.

With the new `showTotalItemsQty` and `showPrice` properties, the Minicart can now follow a distinct behavior which will show the total quantity of items present in your cart as well as their total value. Before this feature, none of these two behaviors was available for the component.

<img width="417" alt="minicart-component" src="https://user-images.githubusercontent.com/52087100/61824296-052edb00-ae34-11e9-81d2-b2cdb6c716dc.png">

### How it works

- `showTotalItemsQty` as `true`: the total item quantity will be displayed.
- `showTotalItemsQty` as `false`: the quantity of different items will not be displayed.
- `showPrice` as `true`: the total cart value will be displayed.
- `showPrice` as `false`: the total cart value will not be displayed.

## Main advantages

With this release, the Minicart behavior is improved, providing users with a better browsing experience since they can now easily have total cart item quantity and value at hand.

## What you need to do

Make sure the store is running version **2.22.0** or higher of the [Minicart](https://github.com/vtex-apps/minicart) app.
