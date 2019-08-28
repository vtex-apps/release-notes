---
title: Drawer component 
description: "Your store Drawer’s behavior and appearance can be customized for mobile users thanks to the component’s 3 new props and CSS handles."
date: "22/08/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Drawer component

Your store Drawer’s behavior and appearance can be customized for mobile users thanks to the component’s **3 new props and CSS handles**.

## What has changed

Before this improvement, it wasn’t possible to customize the store Drawer’s appearance or behavior, such as how it would open and what the icon that closes the Drawer when clicked would be.

The Drawer now has 3 new props that give the retailer greater control over the component’s behavior: `isFullWidth`, `slideDirection` and `maxWidth`. In addition, 3 new CSS handles were enabled in order to customize its appearance: `.openIconContainer`, `.closeIconContainer` e `closeIconButton`.

## How it works

-  `isFullWidth`  is a boolean prop. It allows the user to control whether the Drawer component should take up the full width of the screen when opened (`true`) or only 80% of it (default value `false`).

- `slideDirection` controls whether the Drawer opens from top-to-bottom (`vertical`) or left-to-right (default value `horizontal`).

- `maxWidth`  is either a number (a value in pixels) or a string. It controls the maximum open Drawer width. Since its default value is set at 450 (pixels), the prop becomes very useful for screen sizes greater than 450px if the `isFullWidth` Drawer prop is also active and set to `true`.

---

- `.openIconContainer` is the icon container that opens the Drawer when clicked on.

- `closeIconContainer` is the icon container that closes the Drawer when clicked on.

- `closeIconButton` is the button around of the icon that closes the Drawer when clicked on.

## Main advantage

With the new props, it is possible to control the Drawer component and customize its behavior according to the store’s needs, without having to abide by a default behavior that would hinder mobile user experience.

The new CSS handles also enable Drawer customization as desired, allowing for a symbiotic relationship between it and the store’s identity.

## What you need to do

To customize the [**Drawer**](https://github.com/vtex-apps/drawer), ensure that your store is already running version __0.2.0__ or higher.
