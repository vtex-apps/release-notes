---
title: Simple shelf now can hide unavailable products
description: "Adding a the new prop hideUnavailableItem to a shelf will prevent that products out of stock show up on it."
date: "31/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---


# Simple shelf now can hide unavailable products
​
​
## What has changed
​Now it is possible to choose whether the shelf component will show unavailable items or not by setting a prop.
It is used to ensure that the shelf will only show products in stock - available to be purchased.

<img width="450" alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/4W7LhuQMPL0oLTKd90a8Vv/832caf785d1a2ce94cd0ca322a3a56e1/shelf-unavailable.png_h_250
">

This prop doesn't work for “Related products shelf”, only for simple product shelf.



## What you need to do

​1 - Make sure you have the app [vtex.shelf](https://github.com/vtex-apps/shelf) installed in your store 

2 - Add the component shelf to your store with the prop “hideUnavailableItems” set to true as the example below:

```
  "shelf": {
    "props": {
      "hideUnavailableItems": true //Default value is false.
    }
  }
```
Or go to the store front, click on the shelf component and activate the option “Hide unavailable item”



<img width="180" alt="shop-by-category" src="https://images.ctfassets.net/alneenqid6w5/71zEioPowWYxH0CU8ZfqUP/52d4d45cf1bfba149486fad8a374b5e6/shelf-unavailable-2.png
">
