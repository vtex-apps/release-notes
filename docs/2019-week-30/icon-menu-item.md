---
title: "Menu-item component now supports icon"
description: "​Now it is possible to add an icon besides each menu-item text and create customized menus."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Menu-item component now supports icon
​
​
## What has changed
​Now it is possible to add an icon besides each menu-item text and create customized menus. It is not necessary to add custom CSS to each menu-item to make that happen.
​
This functionality is used to create menus with text and custom icons besides each menu item. Example:

<img width=200 alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/Mo1BRNnVtmWfw0Hq4Kzwn/82acbdadb27e1e2b6b8d84f820c8d1f9/image.png">

## How it works

Two props were created:
- `iconPosition` as `left` or `right`: sets the positioning of the icon relative to the menu-item text
- `iconProps`: group of icon's props

The `iconProps` can hold the following sub-props:


| Prop name      | Type     | Description                                          | Default value |
| -------------- | -------- | ---------------------------------------------------- | ------------- |
| `id`         | `String` | the id of the icon  | N/A           |
| `isActive`         | `boolean` | if the item is active  | `true`          |
| `size`         | `number` | the icon size | 16           |
| `viewBox`         | `String` | the viewbox of the icon  | `0 0 16 16`           |
| `activeClassName`         | `String` | the classname of the icon when `isActive` is true  | N/A           |
| `mutedClassName`         | `String` | the classname of the icon when `isActive` is false  | N/A           |


## What you need to do


1 - Make sure you have a menu implemented in your store with menu-items
2 - Add the necessary props in your menu-item block as the example below:
```
"menu-item": {
  "props": {
    "id": "menu-item-shop",
    "highlight": false,
    "iconProps": {
      "id": "bnd-logo",
      "size": 16,
      "viewBox": "0 0 16 16",
      "activeClassName": "rebel-pink",
      "mutedClassName": "c-action-primary"
    },
    "iconPosition": “right”
  }
}
```



Pr for reference - https://github.com/vtex-apps/menu/pull/59

Issue for reference - https://github.com/vtex-apps/store-discussion/issues/4
