---
title: Events context
description: “Create a web app with more ease with help from Events' expanding functionalities.”
date: “09/13/2019"
git: “https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-35/google-search-box-script.md”
---

# Events context

An app's events context now has access to the `node-vtex-api` library's instantiated clients.  

:information_source: **Events are a way VTEX IO apps communicate**. Differently from HTTP paths, events allow apps to send out requests without having specific targeting, meaning that requests can be sent without the need to have only one destination. For an event request to reach another app, it's enough for the latter to activate the reading of that request in its code. Events are a way to easily communicate when faced with apps that send the same request to multiple recipients. 

:information_source:² **Client is the sum of necessary actions needed to execute a request in a service**. Let's suppose a request is sent from app A to app B, requesting catalog information. To execute this request, app B logically needs to know where and how to look for the information required to be able to pass it onto A. It is not necessary for the developer to know all the functions required for this request to be successfully returned from the Catalog. This kind of *recipe* for performing such a request is done through a Client, instantiated in the request itself to facilitate the coding process. Each VTEX IO service Client is stored in different libraries, such as `node-vtex-api`.

## What has changed

Previously, all Clients stored in the `node-vtex-api` library were instantiated only in the context of the HTTP paths. This means that requests transmitted by events did not have this functionality. Instead of having all the Clients in the library available, it was necessary to instantiate the specific Client of the service call upon by the event request.

With this improvement, all `node-vtex-api` Clients will already instantiated in event contexts.

## Main Advantages

For the developer building an app in VTEX IO, **Client instantiation eliminates the differences between HTTP path requests and events**, allowing new functionalities to be acquired by the latter, such as logging errors.

## What you need to do 

Take a break and relax, because you don't have to do anything at all to add this improvement to your development process! It is freely available :tada:
