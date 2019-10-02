---
title: Toast component redirect
description: "Greater control over user browsing is always magical. Use the `BuyButton` and `ProductSummaryBuyButton` new prop and redirect your user to any URL with a simple click on the Toast component."
date: "09/26/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/toast-component-redirect.md"
---

# Toast component redirect

Thanks to the `BuyButton` and `ProductSummaryBuyButton` new prop, retailers are now able to choose any URL to direct users to using the Toast component. 

## What has changed

Previously, the Toast component (triggered when users click on the store's `BuyButton` or `ProductSummaryBuyButton` component) led users to the checkout, without any other redirect possibilities.

With `BuyButton`'s and `ProductSummaryBuyButton`'s new prop, `customToastURL`, the Toast component can now redirect users to any desired URL.

![toast-redirect](https://user-images.githubusercontent.com/52087100/65714342-4a100180-e071-11e9-91d3-b63cbb622fb2.gif)

## Main advantages

Retailers may have wanted to redirect their users through Toast, choosing another page to where users would land besides Checkout. For example, one with special buy&win promotions or extended warranty options. 

The new prop grants **greater control over user browsing**.

## What you need to do

Have version **2.35.0** or higher of the [`product-summary`](https://vtex.io/docs/components/product/vtex.product-summary) running in your store, as well as the version **3.70.0** or higher of the `vtex.store-componentsrunning`. 
