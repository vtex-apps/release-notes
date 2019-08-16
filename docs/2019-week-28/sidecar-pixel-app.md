# Sidecar pixel app

Integrate your store with the [Sidecar solution](https://hello.getsidecar.com/) by simply using the VTEX IO Sidecar pixel app.

:information_source: The Sidecar solution is used to track and manage Google Shopping campaigns, as well as individual product performance.

## What has changed

In order to use the Sidecar solution on your website, you need to add a script in your Google Tag Manager.

However, as we [previously announced](https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-25/custom-html-tags-are-now-blocked-from-running-on-google-tag-manager-app.md), the integration between store and third-party service using custom script tags is no longer supported and should be done natively using pixel apps.

## Main advantages

This new feature allows Sidecar clients to continue implementing this solution in their store by simply installing the new pixel app and configuring their credentials.

## What you need to do

To install Sidecar pixel app in your store, follow the steps below:

**1.** Open your terminal and run:

```
vtex install vtex.sidecar-pixel@1.x

```

**2.** Open the **Apps** section in your store admin by accessing the following URL:

`https://{STORENAME}.myvtex.com/admin/apps/`

**3.** Click on the Sidecar box and fill in your **Site Domain** and **Site ID**. Then, click on **Save**.

:warning: Installing the pixel app does not automatically contract Sidecar services, but merely provides a native integration together with a solution. It is therefore only available to those that already use this solution in their store.
