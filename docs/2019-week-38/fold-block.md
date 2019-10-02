---
title: Fold block
description: "Can you decide which store's block will be loaded and rendered after the user scroll down? Yes, you can: simply use the Fold block!"
date: "09/26/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-38/fold-block.md"
---

# Fold block

A brand new block called **Fold** allows you to determine which store content should be loaded when the user starts scrolling.

## How it works

To use it, just add a `__fold__` block into any page's source code within your theme. For example:

```
"store.home": {  
    "blocks": [  
      "carousel#home",  
      "flex-layout.row#deals",  
      "__fold__",  
      "shelf#home",  
      "info-card#home",  
      "rich-text#question",  
      "rich-text#link",  
      "newsletter"  
    ]  
  },
```

In the example above, the content begins in `shelf#home` , meaning that the blocks below the `__fold__` block will only load for users once they start scrolling down.

You can also set different `__fold__` blocks either for mobile or desktop, by simply using `__fold__.desktop` or `__fold__.mobile` on the desired page.

:warning: It's still not possible to use the `__fold__` block on page templates built with `flex-layout`, such as product page.

## Main advantages

The new block has a direct impact on the store's **initial loading performance** (and therefore on the lighthouse score), in addition to improving user browsing experience. 

## What you need to do

In order to apply the new block in your store, make sure that `vtex.store` and `vtex.render-runtime` apps are already installed in your store on versions **2.59.0.** and **8.64.0** or higher.
