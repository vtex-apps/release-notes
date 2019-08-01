---
title: "Menu-item component now supports icon"
description: "​It is now possible to add an icon next to each menu-item text and create customized menus."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Menu-item component now supports icon
​
​
## What has changed
​It is now possible to add an icon next to each menu-item text and create customized menus. It is not necessary to add custom CSS to each menu-item to make that happen.
​
This functionality is used to create menus with text and custom icons next to each menu item. Example:

<img width=200 alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/6gWK5iM9VPlQ9fqpyyijtd/925bf668276c714c65a794d9791fb44e/categories-shop-en.png">

## How it works

Two props were created:
- `iconPosition` as `left` or `right`: sets the position of the icon relative to the menu-item text
- `iconProps`: group of icon's props

The `iconProps` can hold the following sub-props:


| Prop name      | Type     | Description                                          | Default value |
| -------------- | -------- | ---------------------------------------------------- | ------------- |
| `id`         | `String` | the icon id   | N/A           |
| `isActive`         | `boolean` | if the item is active  | `true`          |
| `size`         | `number` | the icon size | 16           |
| `viewBox`         | `String` | the icon viewbox  | `0 0 16 16`           |
| `activeClassName`         | `String` | the icon classname when `isActive` is true  | N/A           |
| `mutedClassName`         | `String` | the icon classname when `isActive` is false  | N/A           |


## What you need to do


1 - Make sure your store has an implemented menu with menu-items
2 - Add the necessary props in your menu-item block as in the example below:
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



PR reference - https://github.com/vtex-apps/menu/pull/59

Issue reference - https://github.com/vtex-apps/store-discussion/issues/4