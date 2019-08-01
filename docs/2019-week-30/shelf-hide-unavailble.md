---
title: Simple shelf can now hide unavailable products
description: "Adding the new prop hideUnavailableItem to a shelf will prevent out-of-stock products from appearing on it."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Simple shelf can now hide unavailable products
​
​
## What has changed
​It is now possible to choose whether the shelf component will show unavailable items or not by setting a prop.
It is used to ensure that the shelf will only show products that are in stock - available to be purchased.

<img width=450 alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/4W7LhuQMPL0oLTKd90a8Vv/832caf785d1a2ce94cd0ca322a3a56e1/shelf-unavailable.png_h_250">

This prop doesn't work for “Related products shelf”, but only for the simple product shelf.



## What you need to do

​1 - Make sure your store had the [vtex.shelf](https://github.com/vtex-apps/shelf) app installed 

2 - Add the component shelf to your store with the prop “hideUnavailableItems” set to true as in the example below:

```
  "shelf": {
    "props": {
      "hideUnavailableItems": true //Default value is false.
    }
  }
```
Or go to the store front, click on the shelf component and enable the option “Hide unavailable item”



<img width=180 alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/71zEioPowWYxH0CU8ZfqUP/52d4d45cf1bfba149486fad8a374b5e6/shelf-unavailable-2.png">