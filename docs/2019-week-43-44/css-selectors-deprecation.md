# CSS Selectors deprecation

Starting December 18, 2019, **CSS customization will be done exclusively via CSS Handles** (e.g. `.foo`). Selectors based on HTML structure (e.g. `div > div > span[foo="bar"]`) will be blocked for new stores.

## What has changed

Previously, many VTEX IO store components didn't have their own **CSS Handles**. 

<div class="alert alert-info">
Handles allow you to select and customize a specific store component using CSS classes. 
</div>

Without Handles, a component's CSS customization was necessarily done based on the HTML structure.

**Since most components now have their own CSS Handles, the usage of some CSS selectors will be discontinued.** 

Below, find the full CSS Selectors list that will **continue to be allowed** for your store's customization:

- Class selectors (e.g. `.foo`)
- Pseudo-selectors `:hover`, `:visited`, `:active`, `:disabled`, `:focus`, `:local`, `:not`, `:target`, `:first-child` and `:last-child`
- All pseudo-elements, such as  `::before`, `::after` and `::placeholder`
- `:nth-child(even)` and `:nth-child(odd)`
- Space combinator (e.g. `.foo .bar`)
- `[data-...]` 
- `:global(vtex-{AppName}-{AppVersion}-{ComponentName})` for selection of elements that come from different apps. 

We are deprecating all selectors and combinators not mentioned on the list above, such as:

- Type/tag selectors (e.g. `div`, `span`)
- Combinators such as `>`, `+` and `~`
- `:nth-child` with numbers
- Attribute selectors excepting `[data-...]` (e.g. `[class~="mb8 b--red"]`
- `:global` selector for classes that are not CSS Handles from other apps (i.e., that do not begin with, for example, `vtex-...`);

<div class="alert alert-info">
  This CSS Selector whitelist is flexible because this deprecation aims to encourage robust CSS customization without risking breakdowns in store layout. If the deprecation of CSS Selectors not on this list causes any unintended harm to your store, let us know immediately through <a href="https://github.com/vtex-apps/store-discussion/issues">Store Discussion</a>.
</div>

##  Why this action is being taken

CSS customization that depends on the structure of the HTML can be fragile and detrimental to the **store's stability**.

This is because any change to the HTML, such as changing an attribute, changing the order of an element or wrapping an element into a new tag, can prevent a CSS selector from targeting the correct elements, thereby breaking the retailer's desired customization.

CSS Handles, on the other hand, are guaranteed to be kept working throughout the major version, thus making the **customization much more robust**. This deprecation aims to encourage CSS Handles default use, avoiding potential breakdowns in store layouts. 

## Side effects

### Published Apps 

If your store's theme was previously published, meaning that your store is **already live**, you will **still be able to [link](https://vtex.io/docs/recipes/store/linking-an-app) and [publish](https://vtex.io/docs/recipes/store/publishing-an-app) new versions of your theme, even when using CSS selectors not listed above**.  

This prevents that mature stores which have already been customized without CSS Handles from suddenly not being able to update their theme because of this deprecation.

However, bear in mind that the store **will continue to be susceptible to the above-mentioned problems arising from customization based on the HTML structure**. It is **strongly recommended** then for the CSS to be updated to use only CSS Handles.

### Apps that are not yet published

If your store's project was never published, **any CSS customization performed using CSS Selectors not on the above-mentioned whitelist (such as **`:nth-child`**,** `foo > bar` **and** `[alt="bar"]`**) will be blocked by Toolbelt** during the linking from December 18, 2019 onward.

Although each project scenario can be evaluated individually, it is expected that stores that haven't gone live yet manage to adapt better and faster to the correct customization format.

## What you need to do

Regardless of whether your app is published or not, **it's essential to review every CSS customization for store elements** to ensure that all deprecated selectors are replaced by CSS Handles.

For more on this topic, access our recipe [Using CSS Handles for store customization](https://vtex.io/docs/recipes/layout/using-css-handles-for-store-customization)
