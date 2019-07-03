# Search Bar component

The Search Bar component behavior has improved the search __results preview performance__ with more accurate product results and a more explanatory display message when no results are found.

## What has changed 

Previously, the search results preview was not as accurate. For example: when searching for _Shirt_, no results were displayed, even though there products with _Shirt_ in their name existed.

The search results now show __all__ products that contain the searched term in their names, without exception.

![search-results-preview-example](https://user-images.githubusercontent.com/52087100/60601187-0e261280-9d88-11e9-936b-6f934e44f502.png)

In addition, the message displayed when no results are found also has been improved. When searching for a term that was not found in any product name, the displayed message saying that no match was found was misleading the user since a more complete search (not just a preview by product name) would give results.

Presently, when nothing is retrieved from the search results preview, the Search Bar component displays the following message: "_Search for: {the term you’ve searched for}_", letting the user know that even though no product was shown in the preview, it is still possible to find a positive result for the searched term.

![search-results-preview-empty](https://user-images.githubusercontent.com/52087100/60601249-30b82b80-9d88-11e9-9988-1fb8d4d1ac32.png)

## Main advantages

As the Search Bar component was previously behaving, users would feel frustrated for not being able to see a proper preview of items in the search bar after typing a simple term and being subjected to a long loading time.

The Search Bar also felt buggy, since the empty results message showed no match was found even though results were uncovered when an advanced search was performed

## What you need to do

To set this improvement up in your store, just make sure that your store has at least the 3.48.0 version of the app [Store Components](https://github.com/vtex-apps/store-components) installed and that you are using the component [Search Bar](https://github.com/vtex-apps/store-components/blob/master/react/components/SearchBar/README.md).
