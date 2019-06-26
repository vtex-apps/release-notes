# Custom HTML tags are now blocked from running on Google Tag Manager app

Scripts placed in a page might interfere with other apps, eventually breaking the store. In order to avoid that, Google Tag Manager app now blocks Custom HTML (also called Custom Scripts) tags from running. 

## Why we are taking this action

Usually, Custom HTML tags are used to integrate a store with a third party service.  As we believe this integration should be done natively using apps instead of using Google Tag Manager, from now on a third party service or any interested stakeholder must create an app in order to integrate with a store. 

## What you need to do

Instead of using Custom HTML, you can create a pixel app. A pixel app is basically any third party service that needs to collect data from the user or the store using the pixel builder and the react builder.

You can check some implementations [here](https://github.com/search?q=topic%3Avtex-pixel+org%3Avtex-apps&type=Repositories).
