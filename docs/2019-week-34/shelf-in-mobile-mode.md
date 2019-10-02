---
title: Shelf in mobile mode
description: "Partially display products in Shelf component without breaking the page layout."
date: "29/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Shelf in mobile mode

The Shelf component in mobile mode supports partially displaying your next item to the user, without breaking the layout. 

## What has changed

Previously, the `minItemsPerPage` prop (responsible for setting how many products were displayed on the mobile page) already allowed fractional values, such as `1.5` and `2.79`. The issue was that the page layout wasn't supporting this. Therefore, the Shelf always took on a weird behavior for the mobile user when it was set to partially display a product. 

Following this improvement, the page layout now supports fractional values configured by the `minItemsPerPage` prop.

<img width="323" alt="shelf-mobile-mode" src="https://user-images.githubusercontent.com/52087100/63977586-983ddf00-ca8a-11e9-8b68-5d30e8d60c46.png">

:information_source: The shown fractional prop value will always rounded up by multiples of `0.5`. Let's suppose that you configure the prop to `"minItemsPerPage"="1.9"`, for example. The component will be rendered with a value of `2`, the closest multiple of `0.5` to the value originally configured. 

## Main advantages

The due support to the prop's fractional values, with rounding up, doesn't let the Shelf's layout in mobile mode break anymore when partially displaying products. 

## What you need to do

Ensure that your store is already running version **1.27.0** or higher of the [**Shelf**](https://github.com/vtex-apps/shelf) component. 
