---
title: Pages Settings Tab 
description: "The Pages Settings tab, which served as a shortcut to a basic settings page in VTEX stores, was deprecated."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Pages Settings Tab

The Pages Settings tab, which served as a shortcut to a basic settings page in VTEX stores, was deprecated.

## What has changed

Previously, a Settings tab located in Pages, within CMS, served as shortcut to an App Store admin page that dealt with basic store settings, such as name, favicon and meta description tag.

<img width="1055" alt="settings-tab-setup-fields" src="https://user-images.githubusercontent.com/52087100/63537366-f0556e00-c4eb-11e9-81fb-060d2e168d1b.png">

Now, the Settings tab within Pages has been deprecated. The user can still find and use the page’s functionalities using the admin, by accessing the VTEX Store setup in __Apps__.

## Why are we taking this action

The Pages Settings tab was merely a shortcut to a store’s basic configurations admin page. Since CMS is a novel section aimed at __content__ editing in VTEX stores and not their basic configurations, the shortcut’s deprecation strives for a more cohesive organization of available admin functionalities, improving its findability levels.

## What you need to do

For your admin to reflect this deprecation, ensure that your store is running [**Pages Admin**](https://github.com/vtex-apps/admin-pages) version __4.7.0__ or higher.
