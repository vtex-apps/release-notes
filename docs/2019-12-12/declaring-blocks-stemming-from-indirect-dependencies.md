---
title: Declaring blocks stemming from indirect dependencies
description: "A few releases require more urgency and demand more focus from our users, as we'll see today. Have a look good long look at the following breaking change regarding blocks stemming from indirect dependencies to avoid future headaches!"
date: "12/12/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-12-12/declaring-blocks-stemming-from-indirect-dependencies.md"
---

# Declaring blocks stemming from indirect dependencies

The Store Builder now requires **all blocks** that are used in the construction of a store theme to be defined by the **direct dependencies** of the app in which you are working, without exception. 

## What has changed

Prior to this release, an app could use blocks stemming from apps not declared as its dependency in the `manifest.json`.  

To further understand this scenario, we'll consider the existence of three apps: `A`, `B` and `C`. 

![tree dependencies](https://user-images.githubusercontent.com/52087100/70732501-4cd0d900-1ce7-11ea-9e8e-f70415b91921.png)

According to the old scenario, app `A` could use blocks that were defined by app `C` once the latter is a direct dependent of app `B` and `B` a direct dependent of `A`.  

Now, the Store Builder **only** looks at how a block is defined in the app's direct dependents list. This means that an app can only use blocks defined by apps that are declared as dependencies in its `manifest.json`. 

Therefore, in our example above, app `A` can no longer import blocks from app `C`, because it can only use blocks that are defined by app `B`. 

## Why is this action being taken

Using blocks that were defined in direct and indirect dependencies freely led to app **consistency problems**.

As the Store Builder was searching throughout the entire dependencies tree (meaning indirect and direct dependencies) for the definition of the blocks that were used, it was possible for an app from this long list to define the same block as other apps. This in turn confused the Store Builder as to which version you wanted to export the desired block from.  

In addition to conflicts that could, within the realm of possibility, be reversed, using a defined block in an app that wasn't declared in the `manifest.json` also meant increased **fragility** for the main app.

Following the same example with apps `A`, `B` and `C` above: it was possible for a developer working on app `C` to decide to remove a block used by app `A`, thereby breaking the template construction of the latter. According to the Store Builder's old behavior, the developer would not be aware of what other apps were exporting blocks due to an indirect relationship with `C`.

This release therefore allows for an app's behavior to **become more predictable** and **resilient to errors**, as all block that are used have their origin clearly stated and are controlled by the designated developer through the app's `manifest.json`.

## Side effects

If you're still using indirect dependency blocks, you won't be able to [link](https://vtex.io/docs/recipes/store/linking-an-app) and [publish](https://vtex.io/docs/recipes/store/publishing-an-app) the app in which you are working. Instead, the following error will be displayed:

```
error: App build failed with message: Error resolving block "store.product":
I couldn't find a block "product-reviews". 
You need to declare it or depend on an app that declares it.
```

## What you need to do 

Starting from this release, it is **mandatory** to declare in the in `manifest.json` all apps that define the blocks used in your theme.
