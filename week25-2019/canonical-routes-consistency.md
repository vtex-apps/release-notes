# Canonical routes consistency
 
Seeking to achieve more consistent route mapping, a new portal API was developed to discover the system counterpart of a canonical route.

## What has changed 

Our systems have the difficult task of providing the disambiguation of departments, brands and search canonical routes. When receiving a query as `/clothes`, `vtex.store-sitemap` provides the system route of the canonical route `/clothes/d`. 

`vtex.store-sitemap` used to do this mapping using a learning method. This means that whenever a user accessed `/clothes/d`, the system learned that this was a department and generated the `/clothes` canonical route pointing to `/clothes/d`. 

As the system was suffering from inconsistencies in its responses, an API that maps correctly the canonical to the system route was developed for `vtex.store-sitemap`. 

<strong>Only VTEX stores on v2 are affected with this improvement. GoCommerce stores still uses the old learning method. </strong>

:information_source: Simultaneously, a new metric was created in order to help debugging the learning based approach error rate.  

## Key advantage

The system became more reliable since the new API has improved the routes consistency of VTEX stores. 
