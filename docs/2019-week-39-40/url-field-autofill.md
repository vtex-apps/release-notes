---
title: URL field autofill 
description: "When creating a new page in the admin's Page section, the URL field will automatically propose a path according to the page's chosen title. Isn't it just magical?"
date: "10/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/url-field-autofill.md"
---

# URL field autofill 

The admin's Pages section now allows the `URL` field to autofill when creating a new page for your store. 

![gif-url-field-autofill](https://user-images.githubusercontent.com/52087100/66668807-72c8f700-ec2c-11e9-983b-b2d59998e1cc.gif)

## What has changed

Previously, the system could not allow the text written in the `Title` field to be autofilled in the `URL` field, so the user had to manually type the desired path when creating a new page. 

## Main advantages 

With the autofill feature, the `URL` field becomes more practical and useful for non-technical users mainly because **it applies best SEO practices** to the path's structure, such as eliminating capital letters from titles and the use of hyphens instead of spaces to separate words. 

## What you need to do 

Make sure you store has the [<code>admin-pages</code>](https://vtex.io/docs/app/vtex.admin-pages) app [installed](https://vtex.io/docs/recipes/store/installing-an-app) on version **4.12.6** or higher.
