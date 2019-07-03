# React builder optimization 

The React builder optimization improves webpack logic by having more and smaller javascript bundles. 

## What has changed

Previously, a lot of unnecessary code was being sent to the browser due to the way React builder was implemented, directly impacting the user experience when accessing a page.  

Previously:

![react-builder-optimization-before](https://user-images.githubusercontent.com/52087100/60601542-ae7c3700-9d88-11e9-954b-d8777e049e94.png)

Presently:

![react-builder-optimization-after](https://user-images.githubusercontent.com/52087100/60601533-aa501980-9d88-11e9-87d8-f6a43e85b155.png)
 
As shown above, the React builder optimization has led to __a 53% reduction in resources!__

> Results from [http://storetheme.vtex.com](http://storetheme.vtex.com).

## Main advantages

A reduction in resources means less page loading time for users, also saving them bandwidth.

## What you need to do 

If you are using the `react 3.x` builder, you just have to release a new version.
