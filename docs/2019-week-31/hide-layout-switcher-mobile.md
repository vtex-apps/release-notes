---
title: Search Result layout on mobile mode 
description: "It is now possible to choose which layout mode you want your Search Result to be displayed in."
date: "09/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Search Result layout on mobile mode

By setting the prop `mobileLayout` in the Search Result component, it is now possible to choose which layout mode you want your Search Result to be displayed in.

## How it works

The Search Result component can be displayed in two different layout options:

- __Grid mode__

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62788279-f3d50800-ba9c-11e9-8176-7583235fd709.png">

- __Single mode__

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62789631-ba51cc00-ba9f-11e9-842f-d6b2e22fbaf3.png">

The `mobileLayout` prop allows you to set four different scenarios in your store:

- Grid mode as the default layout and only option for users.
- Single mode as the default layout and only option for users.
- Grid mode as the default layout and Single Mode as the secondary option for users.
- Single mode as the default layout and Grid Mode as the secondary option for users.

:eyes: The secondary option can be activated/deactivated by the store’s user through the layout switcher component placed in the upper-right corner of the Search Results page. When setting a scenario with only one layout option, the layout switcher doesn’t show up on the user’s screen.

## What you need to do

__1.__ Set the [Search Result](https://github.com/vtex-apps/search-result) component within the `store.search` block.

__2.__ Configure the Search Result with the following options inside the `mobileLayout` prop:

- `mode1`: prop that defines the default Search Result layout. Its value can be set as `normal` or `small`. :information_source: Default value is `normal`.

- `mode2`: prop that defines the secondary layout option for users. Its value can be set as `normal` or `small`. :information_source: Default value is `small`.

Notice that the default behavior for your store will be the one defined by `mode1`. If you want the user to be able to switch between two modes, you must specify the `mode2` prop. If only `mode1` is provided, the layout switcher will not be shown, and search results will always be rendered following the `mode1` value. 

:warning: __The value__ `normal` __sets the Single mode and the__ `small` __sets the Grid mode.__

Below, you can find an example of a simple shelf with the Grid mode set to default and Single mode as secondary option:

```
"search-result": {
    "blocks": [
      "filter-navigator.v2",
      "gallery",
      "not-found",
      "breadcrumb",
      "order-by",
      "total-products"
    ],
    "props": {
     "mobileLayout": {
        "mode1": "small",
        "mode2": "normal"
      }
      
      ```
