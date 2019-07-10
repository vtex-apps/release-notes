# Warning disclaimer when in master

With the warning disclaimer present when in a master workspace, Storefront users benefit from greater security when editing their stores.

<img width="1430" alt="warning-disclaimer-master" src="https://user-images.githubusercontent.com/52087100/60997234-be69bd00-a32c-11e9-976a-91d8a21501cf.png">

:information_source: A master workspace corresponds to the version available to the end user.

## What has changed

Previously, no disclaimer was shown to users when editing their store in master. This lack of notice could lead to an increase in the number of errors and retries in the store editing process, since a lot of users may run tests without being aware that any modifications have an immediate effect for the store’s end users.

:warning: __Testing new configurations in master immediately affects your store’s operation.__ We recommend using a development workspace to run tests for any desired change. Only after running all the tests and making sure that everything works correctly should you promote your workspace to master.

## Main advantage

This improvement significantly minimizes storefront creation errors, decreasing the probability of a negative user browsing experience on the site of the store that is being edited.

## What you need to do

To benefit from this improvement, make sure your store’s admin has Pages app version __4.2.0__ installed.
