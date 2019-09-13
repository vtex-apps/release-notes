---
title: MiniCart Sandbox blocks
description: “You're now able to customize your MiniCart footer using Sandbox blocks.”
date: “09/13/2019"
git: “https://github.com/vtex-apps/release-notes/edit/master/docs/2019-week-36/events-context.md”
---

# MiniCart Sandbox blocks 

Sandbox blocks can now be declared in your store's MiniCart and be rendered in the component's lower side.

:information_source: To understand more about what Sandbox blocks are and how to use them, access our [documentation](https://vtex.io/docs/recipes/layout/using-sandbox-blocks).

## What has changed

Previously, the MiniCart didn't allow Sandbox blocks to be declared. As a result, the component could only be customized with its own props and styles. 

Now, MiniCart allows Sandbox blocks to be declared in it. 

:warning: **Notice** that Sandbox blocks rendering will take place in the MiniCart component's lower edge, meaning after the product list but before the total price. 

![sandbox-minicart-component](https://user-images.githubusercontent.com/52087100/64884333-d533d500-d637-11e9-8f29-c5c1f403d75a.png)

## Main advantages

With Sandbox blocks, MiniCart component customizations became much more **flexible**, heeding your store's needs, since new blocks allow HTML, CSS and JavaScript customizations.

## What you need to do

Make sure you've installed [**MiniCart**](https://vtex.io/docs/components/product/vtex.minicart) component version **2.26.0** or higher.
