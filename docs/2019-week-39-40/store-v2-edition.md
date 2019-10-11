---
title: Store v2 Edition 
description: "No more headaches with complex compatibility issues between `store` v1 and v2 thanks to Store v2 Edition."
date: "10/11/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-39-40/platform-performance.md"
---

# Store v2 Edition

Having the new VTEX IO Store v2 Edition installed, stores are now able to run version `2.x.x.` of the app [`store`](https://github.com/vtex-apps/store) with compatibility error-free.

:information_source: Edition is a feature whose aim is to fit a user’s specific requirements with VTEX IO apps usage, through various VTEX IO editions such as VTEX IO Enterprise.

## What has changed

Many stores face compatibility problems with the `store` app, responsible for defining their basic component structure. This happens because of lot of these stores are still running the `store` app on version `1.x.x.`, while new platform components are only compatible with version `2.x.x`.

Due to this version divergence, stores are at risk of forcing an update to `store` v2 and thereby breaking their components still depending on v1 to function properly. Bearing this in mind, each specific component had to be manually updated to the desired version.

Now, stores with the new Edition app installed can automatically start running `store` v2, without having to worry about compatibility. **The Store v2 Edition will handle updates for all components compatible with the old version, in addition to showing installation options for v2 relevant components**.

## Main advantages

By simplifying the entire transaction process between v1 and v2, **Store v2 Edition solves compatibility issues in a easy and quick way**, allowing retailers to enjoy compatibility error-free components in their stores.

## What you need to do 

:warning: **Store v2 Edition can only be installed by someone at VTEX**, by running the command `vtex edition set vtex.edition-store-v2@0.x`. 

You can reach out to our support team to understand if this new feature fits to your store's scenario and request its installation.
