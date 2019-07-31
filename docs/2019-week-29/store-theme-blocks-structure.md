---
title: Store Theme blocks structure
description: "The original Store Theme `blocks.json` file now can be split into different folders and files, in addition to also accepting written comments in it."
date: "24/07/2019"
git: "https://github.com/vtex-apps/release-notes"
---

# Store Theme blocks structure

The original Store Theme `blocks.json` file now can be **split into different folders and files**, in addition to also **accepting written comments** in it.

## What has changed

Before this feature, your store’s entire component structure would be stored in a single `blocks.json` file, in your theme code `store` folder. Since the file did not allow blocks to be divided into other files and folders, some stores were facing code reliability issues in `blocks.json` files with more than 1500+ lines which didn’t have any separation or explanatory comments.

Now, developers can organize the store theme code however they seem best, declaring store blocks in different folders and files and adding comments whenever warranted.

<img width="233" alt="blocks json-structure" src="https://user-images.githubusercontent.com/52087100/61823740-c187a180-ae32-11e9-9593-1f7ba16a812b.png">

In the `blocks` folder, you can create as many folders and files as you want and declare your components in an order of your choosing.

:information_source: You can create files having `.json` and `.jsonc` extensions. We strongly recommend that you create files with the `.jsonc` extension, since it allows you to add file comments, improving the theme’s organization even more.

## Main advantages

The new feature improves theme code organization, improving its management and development through a better readability.

## What you need to do

Make sure that you store is running [Store Theme](https://github.com/vtex-apps/store-theme) app version **3.6.1** or higher.

## Side effects

There should be none since the feature allows you to keep the `blocks.json` or `blocks.jsonc` file as it previously was, attaching it to any file inside the `blocks` folder (if any exist).
