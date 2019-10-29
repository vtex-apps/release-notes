# CSS Selectors deprecation

Starting December 10, 2019, some CSS customization scenarios implemented using the store elements' HTML hierarchy will be blocked.

## What has changed

Previously, many VTEX IO store components didn't have their own **CSS Handles**. 

<div class="alert alert-info">
Through the store theme's root code, Handles allow you to identify and then customize a specific store component using CSS classes. 
</div>

Without Handles, a component's CSS customization was necessarily done through store page HTML hierarchy using CSS Selectors, meaning element selectors for CSS customization according to the page's HTML hierarchy. 

![css-selector-usage](https://user-images.githubusercontent.com/52087100/67809498-8de29600-fa77-11e9-8a9e-ca309458f060.png)

![css-selector-usage-code](https://user-images.githubusercontent.com/52087100/67809526-9d61df00-fa77-11e9-923d-9ed796c77dde.png)

**Since most components now have their own CSS handles, some store customization scenarios using CSS Selectors will be discontinued.** 

Below, find the full CSS Selectors list that will continue to be allowed for your store's customization:

- `:hover`   
- Link selectors, such as `:visited`, `:active` and `:focus`.   
- All pseudo-elements, such as  `::before`, `::after` and `::placeholder`. 
- `:nth-child(even)` and `:nth-child(odd)` 
- `:first-child` and `:last-child`
- Descendant combination element through space, such as `.{Element1} .{Element2}` 
- `[data-*]` 
- `:global(vtex-{AppName}-{AppVersion}-{ComponentName})`

<div class="alert alert-info">
This CSS Selector whitelist can be flexible because this deprecation aims to encourage CSS customization best practices without risking breakdowns in store layout. If the deprecation of CSS Selectors not on this list causes any unintended harm to your store, let us know immediately through <a href="https://github.com/vtex-apps/store-discussion">Store Discussion</a>.
</div>

##  Why this action is being taken

CSS customization performed using CSS Selectors, meaning based on the hierarchical position of a HTML element is detrimental to a **store's stability**.

This is because any change to the HTML, such as adding a new native component on the homepage, can break the hierarchy shown in the theme's code, thereby breaking the retailer's desired customization. 

This deprecation aims to encourage the use of CSS Handles to make CSS customization default and avoid potential breakdowns in store layouts. 

## Side effects

### Published Apps 

If your store's theme was previously published, meaning that your store is **already live**, you don't need to worry about your theme's CSS customization for now, since **Toolbelt will still take all the CSS Selectors (including the one not listed above) into account when [linking](https://vtex.io/docs/recipes/store/linking-an-app)**.  

This avoids that mature stores which have already been customized without CSS Handles do not suddenly get broken layouts because of this deprecation. 

However, bear in mind that the store will continue to be susceptible to the above-mentioned problems arising from CSS Handles-less customization.

### Apps that are not yet published

If your store's project was never published, **any CSS customization performed using CSS Selectors not on the above-mentioned whitelist (such as **`:nth-child`**,** `foo > bar` **and** `[alt="bar"]`**) will be blocked by Toolbelt** during the [linking](https://vtex.io/docs/recipes/store/linking-an-app) from December 10, 2019 onward.

Although each project scenario can be evaluated individually, it is expected that stores that haven't gone live yet manage to adapt better and faster to the correct customization format.

## What you need to do

Regardless of whether your app is published or not, **it's essential to review every CSS customization for store elements** to ensure that CSS Selectors are replaced by the new CSS Handles.

For more on this topic, access our recipe [Using CSS Handles for store customization](https://vtex.io/docs/recipes/layout/using-css-handles-for-store-customization)
