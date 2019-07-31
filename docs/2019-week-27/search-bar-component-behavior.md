# Search Bar component behavior

With its new prop `attemptPageTypeSearch` set as `true`, the [Search Bar component](https://github.com/vtex-apps/store-components/blob/master/react/components/SearchBar/README.md) now allows category name, brand and collection searches to be performed by users.


## What has changed

Previously, the only possible Search component behavior was to show the user all __products__ related to the search term using a Full Text type search. This in turn meant that if users tried to search for a category, brand or collection name using the Search component, they would be taken to the usual search result page for that specific term.

The only way for a store to have a __custom search result page for a category, brand or collection__ was through a link placed on an infocard or accessing it from the menu. The search could not lead users to those pages directly.

With this new prop set as `true`, the Search component is now able to take the user to a customized search result page for a category, brand or collection if any match to the search term is found.

:warning: The component search order flows as follows:  Department > Category > Brand > Collection.

:information_source: If the prop is set as `true` and no match is found between the search term and the existing store categories, brands and collections, the Search component will return to its traditional behavior and the search will be performed for products related to the search term.

## Main advantage

Users are now able to use the Search component to specifically search for a category, brand or collection.

## What you need to do

To enable this behavior in your search, follow the steps below:

__1.__ Make sure that your `"vtex.store-components"` dependency on the `manifest.json` is at least at version __3.48.0__

__2.__ Make sure that the [Search Bar component](https://github.com/vtex-apps/store-components/blob/master/react/components/SearchBar/README.md) is placed in your `blocks.json` file

__3.__ Add the prop `"attemptPageTypeSearch": true` to the block
