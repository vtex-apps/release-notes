# Shelf component 

The group of products shown up in a shelf can now be defined by a subcategory and specification. 

## What has changed

Before this improvement, shelf products could only be defined by:

- Departments (first level of category)
- Collections

Now, the shelf can also be customized to show products from the same:

- Subcategories
- Specifications

## Key advantage 

Each store has a different category tree and a different catalog structure. This improvement aimed to make our component as flexible as possible in order to attend different shelf scenarios. 

 ## What you need to do

 Make sure that you have the [shelf component](https://github.com/vtex-apps/shelf) installed, at least on v1.19.0. Then, follow the steps below:

__1.__ In the admin v2, access __CMS__ and click on the __Storefront__ section

__2.__ Click on the __Shelf component__ that you'd like to customize

__3.__ Select the __content scope__ that you want to change

__4.__ Fill out the field __Category__ with the desired subcategory ID 


![image](https://user-images.githubusercontent.com/52087100/60180793-31384b80-97f7-11e9-951a-93cfd80db6ff.png)


__5.__ If you want to customize your shelf by specification, add a __Specification Filters item__ and fill out the fields that will show up with the specification ID and the specification value respectively.  Notice that this specification should be registered in the category/subcategory defined in step 3.


![image](https://user-images.githubusercontent.com/52087100/60180873-60e75380-97f7-11e9-9b24-c54f3fd0c6be.png)
