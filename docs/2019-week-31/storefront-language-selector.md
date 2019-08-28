---
title: Storefront Language selector 
description: "A language selector has been added to the admin’s Storefront."
date: "09/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Storefront Language selector

A language selector has been added to the admin’s Storefront. The selector takes a user’s location into account.

## What has changed

Previously, to edit content in different languages in Storefront, the user had to change the admin’s language selector which only supported English, Portuguese, and Spanish.

With this change, a new language selector has been added to Storefront’s top bar interface, allowing users to select the language in which they want to add or edit store content.

## Key advantage

Storefront is now able to support languages having different locales, e.g: `pt-BR`, `pt-PT`, `en-US`, `en-GB`.

## What you need to do

__1.__ Make sure your [__VTEX Admin Pages__](https://github.com/vtex-apps/admin-pages) app runs version __4.6.0__ or newer.

__2.__ Make sure the [__VTEX Messages__](https://github.com/vtex-apps/admin-messages) app is installed.

__3.__ Configure the languages that the store can support by accessing __Apps__ from your admin’s __Account Settings__ and selecting the __VTEX Messages__ box.

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62799423-255acd00-bab7-11e9-9e42-01c8bc8189db.png">

__4.__ In CMS, go to the __Storefront__ section and select the language previously configured.

<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62799362-fc3a3c80-bab6-11e9-8ef8-33177038bf03.png">
