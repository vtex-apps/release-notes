---
title: Menu
description: "A new configuration of the Menu block allows its content to be edited with Site Editor! If there's something that retailers like, it's code independence. And if there's something we like, it's to see happy retailers!"
date: "11/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-43-44/menu.md"
---

# Menu 

Edit Menu items using the **admin's Site Editor** with the help of a new and simple Menu component configuration. 

## What has changed

Prior to this release, there was only one way to configure your store's menu items: declaring them as the `menu` block's children.

For example: 

```
"vtex.menu@2.x:menu#websites": {
    "children": [
      "menu-item#shop",
      "menu-item#about-us"
    ]
  },
  "menu-item#shop": {
    "props": {
      "id": "menu-item-shop",
      "type": "custom",
      "iconId": null,
      "highlight": false,
      "itemProps": {
        "type": "internal",
        "href": "#",
        "noFollow": false,
        "tagTitle": "Shop",
        "text": "Shop"
      }
    }
  },
  "menu-item#about-us": {
    "props": {
      "id": "menu-item-about-us",
      "type": "custom",
      "iconId": null,
      "highlight": false,
      "itemProps": {
        "type": "internal",
        "href": "/about-us",
        "noFollow": false,
        "tagTitle": "about-us",
        "text": "About Us"
      }
    }
  }

```

This old configuration made Menu items only editable in code. Now, however, you can declare Menu items directly as `menu` block props, making them editable using Site Editor.

Following the example above, we'll have the following as base of the block's new configuration:

```
"vtex.menu@2.x:menu#websites": {
    "props": {
      "items": [
        {
          "id": "menu-item-shop",
          "type": "custom",
          "iconId": null,
          "highlight": false,
          "itemProps": {
            "type": "internal",
            "href": "#",
            "noFollow": false,
            "tagTitle": "Shop",
            "text": "Shop"
          }
        },
        {
          "id": "menu-item-about-us",
          "type": "custom",
          "iconId": null,
          "highlight": false,
          "itemProps": {
            "type": "internal",
            "href": "/about-us",
            "noFollow": false,
            "tagTitle": "about-us",
            "text": "About Us"
          }
        }
    ]
    }
}

```

## Main advantages 

Configuring menu-items in lists grants **retailers technical independence** with regards to the source code, allowing them to implement desired Menu changes using the Site Editor.

## What you need to do 

Your store is already prepared to configure menu-items as props! For more on how the Menu component works, access its related [documentation](https://vtex.io/docs/app/vtex.menu).
