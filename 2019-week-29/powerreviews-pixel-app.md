# PowerReviews pixel app

Users are now able to use the __Checkout Beacon solution__ from PowerReviews and have all its functionalities at hand by natively integrating with the platform using the PowerReviews pixel app.

:information_source:  The Checkout Beacon solution is used to integrate consumer purchases with the PowerReviews platform.

## What has changed

Previously, our PowerReviews pixel app did not support the Checkout Beacon solution, it only allowed integrations with the platform reviews system.

## Key advantage

Once the user is able to integrate his store natively with the Checkout Beacon solution, he can review purchases experiences on the PowerReviews platform, monitoring store conversion results in a better, faster and easier way.

:warning:  __Installing the PowerReviews pixel app does not automatically contract PowerReviews services__, but merely provides a native integration together with a solution. It is therefore only available to those that already use this solution in their store.

## What you need to do

Make sure that you store is running [PowerReviews](https://github.com/vtex-apps/powerreviews) pixel app version __1.2.2__ or higher.

In order to install it, follow the steps below:

__1.__ Open your terminal and run:

`vtex install vtex.powerreviews@1.x`

__2.__ Open the __Apps__ section in your store admin by accessing the following URL:

`https://{AccountName}.myvtex.com/admin/apps/`

__3.__ Click on the __PowerReviews__ box and fill in the __App Key__, __Merchant ID__, __Merchant Group ID__ and __API Unique ID__ fields. The first three values are given by the PowerReviews platform when granting the integration. The __API Unique ID__ must be filled out using the product information that will link the product review available on the platform to the PowerReviews solution. You can choose between __Link Text__, __product ID__ or __Product reference ID__.

## Side effects

There should be none.
