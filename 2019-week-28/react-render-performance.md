# React render performance

The number of rendered components by React can be reduced using hooks, which allows for a better React render performance.

:eyes: This improvement is more noticeable in pages that have lots of extensions.

## What has changed

Previously, all components necessary for rendering each page were added to the React tree among a `ContextConsumer`, increasing rendering time.

At present, by using the hooks React feature in VTEX IO `render-runtime`, you can reuse a `ContextConsumer` component data by directly using the `context` object in the component itself, without adding it to the React tree. This ensures a faster loading time for the end user.

### Practical effects

- __Using React in a dev environment__

Before:

[![react_dev_before](https://user-images.githubusercontent.com/10400340/61074512-4663cb80-a3ee-11e9-9748-666307469b31.png)](https://user-images.githubusercontent.com/10400340/61074512-4663cb80-a3ee-11e9-9748-666307469b31.png)

After:

[![react_dev_after](https://user-images.githubusercontent.com/10400340/61074520-4b287f80-a3ee-11e9-978d-c79584563d99.png)](https://user-images.githubusercontent.com/10400340/61074520-4b287f80-a3ee-11e9-978d-c79584563d99.png)

- __Using react in a production environment__

Before:

[![timeline_before](https://user-images.githubusercontent.com/10400340/61074541-58456e80-a3ee-11e9-9657-8f128ba8997c.png)](https://user-images.githubusercontent.com/10400340/61074541-58456e80-a3ee-11e9-9657-8f128ba8997c.png)

After:

[![timeline_after](https://user-images.githubusercontent.com/10400340/61074558-5e3b4f80-a3ee-11e9-8407-9442cc6161aa.png)](https://user-images.githubusercontent.com/10400340/61074558-5e3b4f80-a3ee-11e9-8407-9442cc6161aa.png)

-----

This improvement can lead to improvements in responsiveness of up to 30%!

##  Main advantages

By adopting the new hooks React functionality, React will spend less time rendering components onto the interface, thereby ensuring a faster and better end user response time in both stores and admin.

## What do you need to do

This improvement is available to any user that has [Store](https://github.com/vtex-apps/store) app version 2.x installed,   since any such store automatically uses render-runtime version 8.x (in which this improvement was implemented). 

## Side effects

There should be none.
