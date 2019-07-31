---
title: Server timing
description: "Aiming to improve the oversight of performance issues, this new VTEX IO release offers a server timing feature running throughout the request cycle."
date: "24/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Server Timing

Aiming to improve the **oversight of performance issues**, this new VTEX IO release offers a server timing feature running throughout the request cycle.

## What has changed

Previously, the lack of a more precise monitoring of performance issues was a blind spot in VTEX IO.

With the new Server Timing feature active in each request performed on the platform, it became easier to control and decipher issues related to the platform’s slow responsiveness.

### How it works

The Server Timing header in each request follows the following format:

`<hop>.<service>#<target>`

- `<hop>` is the quantity of commands already executed in the IO infrastructure up to the respective request.

- `<service>` is the app the firstly received a request and that performs a query, meaning that it sends another request to another app to get the necessary data.

- `<target>` is the app that is receiving the request from the `<service>`.

These terms may become clearer with following practical example: let's suppose that we have two apps, `gql-srv` and `Apps`. A request is made starting in `gql-srv` calling `Apps`.

The Server Timing results from this chain are the following:

<img width="1439" alt="server-timing" src="https://user-images.githubusercontent.com/52087100/61877084-a82f3580-aec4-11e9-8602-986c4e34f955.png">

:eyes: The Server Timing shows us that `gql-srv` app took 529ms to perform the request and receive its response. It also shows us that `Apps` took 74ms between receiving the request and answering `gql-srv`. By showing all the time taken by `Apps`, the feature allows us to know that `gql-srv` actually took 455ms to perform all its individual actions.

Here, we can notice that `<service>` is the `gql-srv` app that firstly receives the request and that sends another request to `Apps`, the `<target>`. If `Apps` needed to query another app, `` for example, the following format would ensue:

`1.Apps#test`

where `<hops>` is now equal to **1** because of the quantity of commands that were already executed on the IO infra (`gql-srv` > `Apps`) up to the given moment.

## Key advantage

The feature aims to give greater **response timing visibility**, helping to detect bugs that previously could be hidden in certain apps.

By making performance issues easier to surveil, the store’s behavior control and monitoring become undemanding and more agile.

## What you need to do

Any user browsing a VTEX IO version **2.x** page can access the Server Timing information in the browser by following the steps below:

**1.** Inspect the page

**2.** Access the Network tab

**3.** Click on the first name from the data list that will appear

**4.** Access Timing tab to check the data collected by the Server Timing feature

:warning: In cached pages, Server Timing may not show responsiveness data for certain apps since the information required by the request can already be reached through the cache, without the need to call the app.

## Side effects

You can face a small data loading time increase due to the Server Timing header being sent with every request.
