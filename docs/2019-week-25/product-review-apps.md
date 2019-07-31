# Product Review apps

It is now possible to create Product Review apps using abstract interfaces in your store. Since these abstract interfaces have public extensibility, anyone is able to implement the app.   

You can check those interfaces [here](https://github.com/vtex-apps/product-review-interfaces)

## What has changed

Previously, it was not possible to customize your store with a Product Review app. 

## Key advantage

Now, integrate your store with the product review functionalities became simpler and more practical: you just have to install an app. 

## What you need to do

The Theme app must place the abstract product review interfaces in its `blocks.json` so the Review apps show up in a plug and play way. You can check how the interfaces `product-review-form`, `product-reviews`, `product-rating-summary` and `product-rating-inline` are placed in the [Store-theme](https://github.com/vtex-apps/store-theme) app.

Also, check the example app implementation [here](https://github.com/vtex-apps/product-review-interfaces/tree/master/example). 

:eyes: Two apps are ready to be installed and used. Since their code is public, they serve as an example of how it can be done for other services:
[https://github.com/vtex-apps/bazaarvoice/](https://github.com/vtex-apps/bazaarvoice/)
[https://github.com/vtex-apps/powerreviews/](https://github.com/vtex-apps/powerreviews/)
