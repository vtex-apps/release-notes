---
title: Events context
description: "Create a web app with more ease with help from Events' expanding functionalities."
date: "09/13/2019"
git: "https://github.com/vtex-apps/release-notes/edit/master/docs/2019-week-36/events-context.md"
---

# Events context

An app's events context now has access to the `node-vtex-api` library's Clients.  

:information_source: **Events are a way VTEX IO apps communicate** such as HTTP requests. While HTTP requests are a one-to-one mechanism, events are one-to-many. Apps that want to consume that information can subscribe to those events.

:information_source:² **Client assists one service in communicating with another**. Behind the scences, the Client knows how to make HTTP requests, without the need for the developer to know all the implementation details. 

## What has changed

Previously, all Clients provided by the `node-vtex-api` library were instantiated only in the context of the HTTP middlewares, but not event handlers. Instead of having all the Clients in the library available, it was necessary to instantiate the specific Client of the service call upon by the event request.

With this improvement, all `node-vtex-api` Clients will already instantiated in event contexts.

## Main Advantages

For the developer building an app in VTEX IO, **Client instantiation eliminates the differences between HTTP path requests and events**, allowing new functionalities to be acquired by the latter, such as logging errors and timing metrics.

## What you need to do 

Take a break and relax, because you don't have to do anything at all to add this improvement to your development process! It is freely available :tada:
