---
title: Minicart Sandbox blocks
description: "You're now able to customize your Minicart footer using Sandbox blocks."
date: "09/13/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-36/minicart-sandbox-blocks.md"
---

# Minicart Sandbox blocks 

Sandbox blocks can now be declared in your store's Minicart and be rendered in the component's lower side.

:information_source: To understand more about what Sandbox blocks are and how to use them, access our [documentation](https://vtex.io/docs/recipes/layout/using-sandbox-blocks).

## What has changed

Previously, the Minicart didn't allow Sandbox blocks to be declared. As a result, the component could only be customized with its own props and styles. 

Now, Minicart allows Sandbox blocks to be declared in it. 

:warning: **Notice** that Sandbox blocks rendering will take place in the Minicart component's lower edge, meaning after the product list but before the total price. 

![sandbox-minicart-component](https://user-images.githubusercontent.com/52087100/64884333-d533d500-d637-11e9-8f29-c5c1f403d75a.png)

## Main advantages

Minicart component now became much more **flexible**, heeding your store's style needs, since Sandbox blocks allow HTML, CSS and JavaScript customizations.

## What you need to do

Make sure you've installed [**Minicart**](https://vtex.io/docs/components/product/vtex.minicart) component version **2.26.0** or higher.
