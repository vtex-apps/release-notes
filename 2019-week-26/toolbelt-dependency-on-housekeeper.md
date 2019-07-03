# Toolbelt dependency on Housekeeper 

In order to decrease inconsistencies between apps updates, [VTEX IO Toolbelt](https://github.com/vtex/toolbelt) now uses the __Housekeeper API__.  

:information_source: Housekeeper is the system responsible for automatically updating account apps.

## What has changed

Previously, our CLI (VTEX IO Toolbelt) did not take advantage of the Housekeeper apps updater service when launching the `vtex update` command. By not taking advantage of this service, Toolbelt was not able to support features such as Edition, which could have led to inconsistencies about which specific workspace apps should be updated.

:information_source: Edition is a feature that seeks for VTEX IO usage to fit a user’s specific requirements, through various VTEX IO editions such as VTEX IO Enterprise.

The Housekeeper API solves both issues: it is now used by VTEX IO Toolbelt to decide which updates are to be made to a given workspace considering the necessary changes to an account edition. 

When launching the `vtex update` command, tables separated by the app installation type (if it is an infra app, an user-installed app, an edition-installed app, etc.) are displayed containing the pending updates. For example:

![vtex-io-toolbelt-using-housekeeper-api](https://user-images.githubusercontent.com/52087100/60602163-a670c700-9d89-11e9-9667-2ddb3f2db34a.png)

## Main advantages

By depending on the Housekeeper API, VTEX IO Toolbelt has become more reliable when it comes to app updates. In addition, it is now also compatible with Editions and any other Housekeeper features.
