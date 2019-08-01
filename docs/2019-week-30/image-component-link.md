---
title: Image component now has href prop
description: "Our image component now supports the prop link."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Image component now has href prop

Our image component - https://github.com/vtex-apps/store-components/blob/master/react/components/Image/README.md now supports the prop link. It is now possible to make the image clickable, and to set the url to where the user will be redirected both on storefront and in the block files.

## What has changed

Our image component wasn't clickable before, it was not possible to link it.

## Main advantages

It is now possible to set a custom image url directly through store front or blocks.

## What you need to do

1 - Make sure your store had the app store-components installed -https://github.com/vtex-apps/store-components/

2 - Add the component Image to your store
https://github.com/vtex-apps/store-components/blob/master/react/components/Image/README.md 

3 - Add the prop “link” to it in blocks.json; example:

```
“props”: {
  “link” : {
    “attributeNofollow”: false, //if true, sets rel=noFollow attribute to the link. Default = false
    “attributeTitle”: "My image here", //set tooltip message on hover
    "newTab": true, //if true, will open link on new tab. Default = false
    "url": "google.com" //	sets the url that the user will follow by clicking on the image
  }
}
```

Or enter in the store front and edit the url through the interface:

<img width="417" alt="prop-link" src="https://images.ctfassets.net/alneenqid6w5/3Yi5ujGAA1R8UrGxUKxj72/8d0318fe1f1960ad1ce52746afd4803c/Captura_de_Tela_2019-07-31_a__s_16.27.39.png">