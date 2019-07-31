---
title: Price internationalization
description: "Currency codes and decimal places can now be easily internationalized by defining their values and behavior in your admin’s Sales Policies section."
date: "24/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Price internationalization

Currency codes and decimal places can now be easily internationalized by defining their values and behavior in your admin’s Sales Policies section.

## What has changed

Previously, a store’s price currency code only took the sales policies’ `Currency Symbol` field value into account. As this field’s value was usually filled by retailers according to their local currency code parameter, stores face internationalization problems with international user’s understanding of a product’s real value.

Let’s suppose the following: a brazilian retailer sets their store’s currency code to `R$`. While `R$` might be an understandable currency code for brazilian users, understanding a product’s value may prove difficult to international users, since `R$` is not an international currency parameter.

In addition, customizing the decimal places displayed by the store’s prices was also not possible, as the default was always _two_ decimal places per price.

Aiming to put an end to misunderstandings caused by price value and overcome the hurdles of a store’s internationalization process, **this feature showcases two brand new functionalities**:

- The sales policy’s `Currency Decimal Places` field now allows you to freely set the number of decimal places that your store’s prices display.

- A store’s currency code definition will now only consider values that are filled in the sales policy’s `Currency Code` and `Culture Info` fields. The `Currency Symbol` field does not perform this function anymore, although it’s still present on the interface and can be used in stores built outside the VTEX IO platform.

### How it works

When the site’s language differs from the default set in the `Culture Info` field, the system interprets that it is dealing with an international user therefore the currency shown should follow currency code international standards (ISO standard). In these scenarios, the system will display prices with the international currency code set in the `Currency Code` field.

When the site’s language is the same as the deafult set in the `Culture Info` field, the system will interpret that it is dealing with a local user therefore the currency code doesn’t require to follow international standards. It will suffice if the commonly used currency symbol for that country is displayed.

Looking at the example stated above, we could have the following real life situation: a brazilian retailer that set the `Culture Info field` value to `Brasil(pt-BR)` and the `Currency Code` to `Real (BRL)` will have his prices displayed with the `BRL` currency code for international users and `R$` for local users.

## Main advantages

The features not only gives retailers the **freedom of choosing** how many decimal places the store’s prices are displayed with, but also encourages **internationalization** by correctly adapting the currency code according the end-user’s location. This avoids that the user is faced with misleading product price information and ensures greater store reliability.

## What you need to do

Make sure the store is running [Store Components](https://github.com/vtex-apps/store-components) app version **3.54.0** or higher.
