# VTEX IO Highlights - Week 28/2019

Welcome to the VTEX IO weekly release notes!

Here’s a sneak peek at the key changes made in the last week:

>:bell: Keep up with VTEX IO release notes! Just click on  **Releases only**  in the  **Watch**  box in the right upper corner of this page.

### New features  :rocket:

- [Sidecar pixel app](https://github.com/vtex-apps/release-notes/blob/master/2019-week-28/sidecar-pixel-app.md)  - Get your hands on a first-party integrations with the Sidecar solution.
- [Native A/B Testing](https://github.com/vtex-apps/release-notes/blob/master/2019-week-28/native-ab-testing.md) – Increase your store’s conversion rate by performing native VTEX IO A/B testing, now available to clients platform-wide.
- [Typography customization](https://github.com/vtex-apps/release-notes/blob/master/2019-week-28/typography-customization.md) - Easily customize your store’s typography through Storefront.

### Improvements  :heavy_plus_sign:

- [Submenu behaviour](https://github.com/vtex-apps/release-notes/blob/master/2019-week-28/submenu-behavior.md)  - The Menu component now has a better behavior when it is triggered to expand.
- [React render performance](https://github.com/vtex-apps/release-notes/blob/master/2019-week-28/react-render-performance.md) - VTEX IO now implements the new React feature that allows component data reuse using hooks.

### Notable bug fixes  :bug:

- [RichText content](https://github.com/vtex-apps/admin-pages/pull/241) - RichText fields edited through storefront no longer display a hash id.
- [Block title](https://github.com/vtex-apps/render-runtime/pull/345) - The block `title` prop was used to edit the block name displayed in the Storefront section, in the new CMS version. This Pull Request aims to fix it since it was broken during the latest releases.
- __“Socket Hang Up” errors__ - Recurring problems with server-side rendering, asset fetching and graphql queries were solved, ensuring that the end user no longer faces page loading errors. :information_source: This bug fix pull Request was done is a VTEX private repository.
