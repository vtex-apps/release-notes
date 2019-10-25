---
title: CSS Handles component development
description: "Devs, celebrate with me: this release is about a more advantageous, easy and brand new way to create CSS Handles for store components."
date: "10/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-41-42/css-handles-component-development.md"
---

# CSS Handles component development

Create CSS Handles for a store's component in a **faster**, **simpler** and **more resilient** way. 

## What has changed

CSS Handles pertaining to components can now be created in the same internal file of your app, instead of through an external `styles.css`, as was previously the case. 

In addition, you won't need to manually create Block Classes anymore. Using this new method, creating a Handle for an element automatically generates that Handles Block Class in the app's code.

This wasn't previously possible.

## Main advantages

If you've gone through the functionalities of this way to create CSS Handles, you probably already understood the feature's main advantage: **facilitating the developer's coding process**.

In addition, this new CSS Handles creation method has another big advantage: it is, as we like to say, **future-proof**. This means that it's **resistant to platform changes**, such as component migration among apps.

Let's suppose that you want to migrate a component that's defined in app `A` to app `B`. According to the previous method, you would also have to create the component Handle in App `B` in order to use it. With the new method, the component's Handle will always automatically adapt to the current app in which it's defined, thus making the component migration process between apps easier.

## What you need to do 

You can already start using this new way to create CSS Handles at will!

For more insight on this feature's usability, access its related [documentation](https://vtex.io/docs/app/vtex.css-handles).
