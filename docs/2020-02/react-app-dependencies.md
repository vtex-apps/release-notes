---
title: React app dependencies 
description: "The wise Toolbelt will now update an App React's dependencies (located in the app's `package.json` file) to keep them in line with Render's dependencies list."
date: "2020-03-16"
git: "https://github.com/vtex-apps/release-notes/blob/fix-link-typos/docs/2020-02/react-app-dependencies.md"
---

# React app dependencies 

App React dependencies (located in the app's `package.json` file) are now automatically updated by Toolbelt and kept up-to-date with the Render Runtime dependencies. 

## What has changed

The Render Runtime (VTEX IO service app responsible for server-side rendering apps) declares its own dependencies in order to run renderable apps in your browser.  

While React apps also declare their own dependencies to properly function, in practice, when an dependency is declared both in Render and in the React app, only the version declared into the Render was taken into account when the React app was being rendered.

At the end of the day, independent of the apps and versions declared in a React app's dependencies, VTEX IO platform only used those listed in Render, leading to a lack of transparency in the development process.

React app dependencies that are also in Render will continue to not be taken into account for the rendering process, however now **Toolbelt will update the React dependencies and keep it up-to-date with the Render fixed dependencies list**.

:warning: Bear in mind that this is regarding dependencies that are declared **both** in Render and React apps. Dependencies that are only listed in React apps will keep being used by Render and updated by Housekeeper normally.

### How it works

Whenever the React app is linked, published, deployed or undergoes any changes that require Toolbelt interaction, Toolbelt will automatically update the app's dependencies list to keep it up-to-date with the Render's dependencies. 

However, this will only occur if these updates are not breaking changes.

Toolbelt **will not** update any dependency if this implies a change in a Major, meaning a  breaking change for your app. Only changes to minor and patch versions will be applied. 

## Why we are doing this

The **homogeneity** of the dependencies lists aims to ensure the **transparency** of the React apps development process. Besides that, it aims to guarantee the **robustness** of the platform architecture and its various apps and services.

## Side effects

Your app should function without any adverse side effects.

However, statistical analysis tools may detect the updates that Toolbelt performed to your code and point out inconsistency errors based on the code used and the dependency's new version.

Whenever this happens, check the app's dependencies version and perform the necessary changes! 

## What you need to do 

Let Toolbelt perform its magic for you. Just keep an eye out for any errors that may pop up due to the changes implemented by Toolbelt.
