# Global Messages discontinued

Seeking to ensure a greater support to multi-language stores, Web Framework will only translate and provide messages used by each component being rendered on a given page.

 __A new version of the Web Framework will be released during the next week that deprecates Global Messages__ and all VTEX apps will be migrated to respect the new format. 

## What has changed 

Currently, components using react builder 3.x can use the provided `react-intl` library to internationalize messages (e.g. using `<FormattedMessage/>`).

As the number of components in a store has grown, it became important that only strings that are actually being used in a given page are translated by Web Framework. 

## Why we are taking this action

Initially, messages were not scoped by an app, leading to the possibility of using (directly in your code) messages defined by other apps you depend on. Being able to tap into implicit dependencies is extremely dangerous since your dependency may change their messages without notice and break a working app.

By making this dependency explicit, as all others in VTEX IO, we can ensure apps continue working normally. 

## Main advantages

By translating and providing only the messages actually used by the page being rendered, we can have faster response times and smaller response payloads.

## What you need to do

Wherever you are using a `<FormattedMessage>` component in your code, check that the message is defined by your app in one of the `messages/` files. If it's not, you must check from which of your dependencies this message is exported. 

Then, add a key in the `messages/context.json` file in the format:

`"Vendor.name::message-id": ""`

Where:

•	`vendor.name` is the vendor and the name of your dependency
•	`message-id` is the ID of the message you are using

Example: [https://github.com/vtex-apps/my-account/blob/feature/lazy-messages/messages/context.json#L58](https://github.com/vtex-apps/my-account/blob/feature/lazy-messages/messages/context.json#L58)

:eyes: In order to use messages defined by a dependency, you must specify that they should be used in your `messages/context.json`.

## Side effects 

Any apps using messages from dependencies implicitly will simply show the raw message ID instead of the proper message. Fixing it is straight-forward as shown above. 
