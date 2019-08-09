# Set minimum of items on Shelf


Set the minimum amount of items that can be displayied on a shelf component regardless the display mode (mobile, tablet or desktop).


## What has changed 


It was only possible to set the maximum amount of items shown in a shelf by using the prop `itemsPerPage`.  This configuration would limit the amount of items shown even in the largest of the screens.  However, in small screens, it would always show one product per row - it was not possible to set a minimum amount of items to be shown.
By setting the new prop minItemsPerPage you can also control the amount of items to be shown even in the smallest screen size.




## Key advantage
Using these two props together you can control how many items are shown in the smallest screen size  and in the biggest screen size, with the component adjusting itself when in intermediate sizes. 

For example, if you want to always display 2 items on mobile, you just need to pass minItemsPerPage: 2. and a maximum of 5 items on a big screen, you could also pass the already existing prop "itemsPerPage:5"


## What you need to do

__1.__ Make sure your store has at least the 1.23.0 version of the app [Shelf]https://github.com/vtex-apps/shelf) installed and set in your blocks files.


__2.__ Configure your shelf block with the following prop that is part of the `productList` set of props:


- `minItemsPerPage`: __number__ - .Minimum amount of slides to be on the screen, can be used to control how many itens will be displayed in the smallest screen size. Default value is 1




An example on how to set it in a valid block can be seen below:

```
"shelf": {
  "props": {
    "orderBy": "OrderByTopSaleDESC",
    "productList": {
      "maxItems": 10,
      "itemsPerPage": 4,
      "minItemsPerPage": 2,
      "scroll": "BY_PAGE",
      "arrows": true,
      "titleText": "New collection",
      "hideUnavailableItems": true,
      "summary": {
        "isOneClickBuy": false,
        "showBadge": true,
        "badgeText": "OFF",
        "buyButtonText": "Comprar",
        "displayBuyButton": "displayButtonHover",
        "showCollections": false,
        "showListPrice": true,
        "showLabels": false,
        "showInstallments": true,
        "showSavings": true,
        "name": {
          "showBrandName": false,
          "showSku": false,
          "showProductReference": false
        }
      }
    }
  }
}
```