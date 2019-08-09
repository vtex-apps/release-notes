# Storefront Language selector

Added a language selector to storefront that supports selection of language with locale for storefront's store visualization.

## What has changed


To edit content for different languages in storefront the user had to change the of the admin. Also admin's language selector only supports English, Portuguese, and Spanish.
Now there is a new language selector at the top bar of storefront's interface that allows users to select the target language that they want to add/edit content.


## Key advantage
With this feature we're now ready to support languages with different locales, e.g: pt-BR, pt-PT, en-US, en-GB


## What you need to do


__1.__ Make sure your vtex.admin-pages has at least the 4.6.0 version.

__2.__ Make sure you have the vtex.messages app installed.

__3.__ Configure the languages your store supports at: https://<account>.myvtex.com/admin/apps/vtex.messages@<messages-version>/setup/ 
<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62799423-255acd00-bab7-11e9-9e42-01c8bc8189db.png">

__4.__ Go to storefront and select the language added. 
<img width=500 alt="shop-by-category" src="https://user-images.githubusercontent.com/12139385/62799362-fc3a3c80-bab6-11e9-8ef8-33177038bf03.png">


