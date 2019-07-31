---
title: PowerReviews pixel app
description: "Users are now able to use the Checkout Beacon solution from PowerReviews and have all its functionalities at hand by natively integrating with the platform using the PowerReviews pixel app."
date: "24/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# PowerReviews pixel app

Users are now able to use the **Checkout Beacon solution** from PowerReviews and have all its functionalities at hand by natively integrating with the platform using the PowerReviews pixel app.

:information_source: The Checkout Beacon solution is used to integrate consumer purchases with the PowerReviews platform.

## What has changed

Previously, our PowerReviews pixel app did not support the Checkout Beacon solution, it only allowed integrations with the platform reviews system.

## Key advantage

Once the user is able to integrate his store natively with the Checkout Beacon solution, he can review purchases experiences on the PowerReviews platform, monitoring store conversion results in a better, faster and easier way.

:warning: **Installing the PowerReviews pixel app does not automatically contract PowerReviews services**, but merely provides a native integration together with a solution. It is therefore only available to those that already use this solution in their store.

## What you need to do

Make sure that you store is running [PowerReviews](https://github.com/vtex-apps/powerreviews) pixel app version **1.2.2** or higher.

In order to install it, follow the steps below:

**1.** Open your terminal and run:

`vtex install vtex.powerreviews@1.x`

**2.** Open the **Apps** section in your store admin by accessing the following URL:

`https://{AccountName}.myvtex.com/admin/apps/`

**3.** Click on the **PowerReviews** box and fill in the **App Key**, **Merchant ID**, **Merchant Group ID** and **API Unique ID** fields. The first three values are given by the PowerReviews platform when granting the integration. The **API Unique ID** must be filled out using the product information that will link the product review available on the platform to the PowerReviews solution. You can choose between **Link Text**, **product ID** or **Product reference ID**.

## Side effects

There should be none.
