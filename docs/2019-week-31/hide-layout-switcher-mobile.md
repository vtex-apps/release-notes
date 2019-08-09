
# Control Layout Switcher on Mobile mode


Control the mobile layout's default mode on your search results and the display of the layout's controller. Current mobile layout options are grid mode and single mode

## What has changed 

By setting the prop `mobileLayout`in your [search-result component](https://github.com/vtex-apps/search-result), it is possible to choose which is the mode in which to show your search-results on mobile mode. 


Grid mode:

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62788279-f3d50800-ba9c-11e9-8176-7583235fd709.png">




Single mode:

<img width=180 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62789631-ba51cc00-ba9f-11e9-842f-d6b2e22fbaf3.png">



With this prop you are able to set four different scenarios:


* Grid mode as default and only option
* Single mode as default and only option
* Grid mode as default, and single mode as secondary option
* Single mode as default, and grid mode as secondary option


The secondary option can be activated/deactivated by the store's user through the layout switcher component placed in the upper-right corner of the search results page. When setting a scenario with only one layout option, the layout switcher doesn't show up on the user's screen.


## What you need to do


__1.__ Set the [Search Result](https://github.com/vtex-apps/search-result) to your `store.search` block.


__3.__ Configure your search result block with the following options inside the prop `mobileLayout`:


- `mode1`: __enum__ - . Layout mode of the switcher (values: 'normal' or 'small') . Default value is `normal`.
- `mode2`: __enum__ - . Layout mode of the switcher (values: 'normal' or 'small') . Default value is `small`.


The value `normal` sets the **single** mode.
The value `small` sets the **grid** mode.


Notice that the default behavior for your store will be the one defined by the mode1. If you want the user to be able to switch between two modes, you must specify the mode2 prop. 
If only the mode1 is provided, the layout switcher will not be shown and search results will always be rendered according to mode1.




An example of a simple shelf with the scenary "Grid mode as default, and single mode as secondary option" set can be shown below:
    
```
"search-result": {
    "blocks": [
      "filter-navigator.v2",
      "gallery",
      "not-found",
      "breadcrumb",
      "order-by",
      "total-products"
    ],
    "props": {
     "mobileLayout": {
        "mode1": "small",
        "mode2": "normal"
      }
```

