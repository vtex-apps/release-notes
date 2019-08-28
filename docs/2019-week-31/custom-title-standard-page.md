---
title: Title of contextless routes 
description: "The field title for routes without a context (such as product, brand, category, etc) weren’t editable previously. This release enables its editing."
date: "09/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Title of contextless routes

The field title for routes without a context (such as product, brand, category, etc) weren’t editable previously. This release enables its editing.

:information_source: Pages with context titles are defined by their context, i.e. product’s name.

## Key advantage

This brings SEO advantages, as users can change the Home title, for example, without impacting other pages.

## What you need to do

This feature is available in the __3.x__ and __4.x__ [__VTEX Pages__](https://github.com/vtex-apps/admin-pages) majors.

__1.__ Go to the Pages admin section. To get there, go to your store’s admin homepage, click on __CMS__ and then access the __Pages__ section.

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62791754-3221f580-baa4-11e9-91ef-7254c201c290.png">

__2.__ Choose the desired page whose titles you wish to edit, under the __Standard group__.

__3.__ Type the title you want have displayed in your store and then click on __Save__.

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62793723-9fd02080-baa8-11e9-9c44-b1126388dab8.png">

Resulting title:

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62793775-c9894780-baa8-11e9-885d-78f55fb12b9a.png">

:warning: __Be careful when editing this option in your master workspace!__ The changes will be automatically applied to your store in production. To test these changes without affecting production, access the admin from a development workspace.
