---
title: Site Editor
description: "They say 1 is few, 2 is good and 3 is a party. If a release for the Site Editor is already incredible, picture 3? Check out the new Topbar, complete with tooltips and new modal texts for the admin section."
date: "11/25/2019"
git: "https://github.com/vtex-apps/release-notes/blob/master/docs/2019-week-45-46/site-editor.md"
---

# Site Editor 

The admin's Site Editor section gained three key releases that improve user experience when editing blocks. These improvements are as follows:

- **Topbar redesign**
- **Topbar Tooltips**
- **Modal texts**

## What has changed 

### Topbar redesign 

The Site Editor's topbar was completely redesigned to improve user editing experience. This release's main change was transferring the **Store** and **Design** tabs, previously in the Site Editor's topbar, to the admin's sidebar. 

- Previously: 

![site-editor-topbar-redesign](https://user-images.githubusercontent.com/52087100/69550686-34885c80-0f7a-11ea-9828-dba0f8c25958.png)

- Presently: 

![site-editor-topbar-redesign-2](https://user-images.githubusercontent.com/52087100/69550748-52ee5800-0f7a-11ea-9e89-5f1a7b4177ab.png)

Notice that the Store and Design tabs are now only accessed through the admin's sidebar:

![cms-styles-store-sections](https://user-images.githubusercontent.com/52087100/69550948-a6f93c80-0f7a-11ea-833d-0260db65449b.png)

### Topbar Tooltips 

In order to help users understand the new topbar buttons, tool tips were added during the hover.

![site-editor-topbar-tooltip](https://user-images.githubusercontent.com/52087100/69551002-c09a8400-0f7a-11ea-8b9d-1b301946f7de.png)

### Modal texts 

Modal texts are shown to users when a critical action is taken during the editing of content by the Site Editor, such as cancelling already made changes and thus losing these changes.

This release improves the displayed texts, aiming to **make communication with users clearer** with regards to the consequences of their action. For example:

- Previously: 

When deciding to discard already made changes, users were faced with the following warning: `"Your unsaved changes will be lost. Are you sure you want to continue?"`

- Presently: 

In trying to make users aware of the consequences their action brings, the above mentioned message was replaced with the following: `"You have unsaved changes. Are you sure you want to continue and discard your modifications? This action cannot be undone."`. 

## What you need to do 

The **topbar's redesign** is available for your store starting with version **4.17.0** of the [Admin Pages](https://vtex.io/docs/app/vtex.admin-pages). 

**Tooltips** can be displayed in your Site Editor starting with version **4.18.0** or higher of the same app above.

However, if you want to really slick Site Editor which includes these incredible releases in addition to the **new modal texts**, the Admin Pages in your store should be at least version **4.18.1**.
