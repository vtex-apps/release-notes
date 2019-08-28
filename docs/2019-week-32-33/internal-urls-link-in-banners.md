---
title: Internal URLs link in banners 
description: "With the new 'Internal URL' field, CMS’s Storefront section now allows you to easily and swiftly link internal URLs to a banner by simply copy-pasting the desired address."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Internal URLs link in banners

With the new `Internal URL` field, CMS’s Storefront section now allows you to easily and swiftly link internal URLs to a banner by simply copy-pasting the desired address.

## What has changed

Previously, in order to link an internal store URL to a banner, you had to select the desired route and insert all its parameters in the `Banner target page` and `Params` fields.

With the `Internal URL` field, the URL that will be linked to the banner can be filled in without needing to insert the route or parameters as before. Simply copy and paste the desired address.

<img width="1142" alt="internal-url-field" src="https://user-images.githubusercontent.com/52087100/63539007-77f0ac00-c4ef-11e9-8933-c5da41d7b6f4.png">

:warning: With the new feature, the `Banner target page` and `Params` fields were deprecated. Therefore, the filled in `internal URL` data will be the only data taken into account when indicating the desired internal route. 

## Main advantages

When linking a complex query internal URL to a banner, the retailer would have faced difficulties in correctly filling out all the parameters. By allowing the internal URL to be linked by simply copying and pasting it in the new field, the feature brings simplicity to a retailer’s Storefront experience.

## What you need to do

To benefit from this new feature, make sure that your store is running [__Carousel__](https://github.com/vtex-apps/carousel) version __2.11.0__ or higher.
