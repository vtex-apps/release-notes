---
title: Product Summary
description: "These past two weeks were not special just for the SKU Selector: the Product Summary didn't just gain a blockClass prop, but also a CSS Handle. Now that's rad right?"
date: "11/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-43-44/product-summary.md"
---

# Product Summary

The Product Summary component now has its own **CSS Handles** and **blockClass**. 

<div class="alert alert-info">  
CSS Handles are <strong>HTML element identifiers</strong> and can therefore be used to customize store components that use Product Summary by simply using CSS classes in the store theme's code.  
</div>

<div class="alert alert-info">  
The blockClass is a prop that functions as a block identifier within your code. When configured, it becomes possible to customize two Product Summary blocks individually
</div>

## Main advantages 

Without CSS Handles, Product Summary customization depended on CSS Selectors, which looked to a page's HTML structure when selecting an element. 

This store customization practice, in addition to being vulnerable, will soon be [deprecated](https://vtex.io/docs/releases/2019-week-43-44/css-selectors-deprecation). Therefore, launching the component's Handles is of **strategic importance**.

In addition, the blockClass allows retailers to **experiment more with different customization** for various Product Summary blocks.

## What you need to do

Handles and blockClass can already be used in your store! Simply ensure that your store uses [Product Summary](https://vtex.io/docs/app/vtex.product-summary) version **2.43.2** or higher.
