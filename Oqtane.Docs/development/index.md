# MyLabBook Development

The main approach to customizing Oqtane is to create or import custom modules. The easiest way to create a custom module is to use the custom 
module builder that is included by default in Oqtane. This will provide a basic framework for a working custom module. But that working
custom module is limited. The default module provides the ability for the user to create one or more items. Each item has a Name 
string. The created items can be edited or deleted by the user. The created items are listed also in the module, along with Edit and
Delete buttons for each item. However, to extend this default module requires custom programming. 

A very helpful guide to customizing this default module is provided by Michael Washington on his [Blazor Help Website](https://blazorhelpwebsite.com/ViewBlogPost/4). 
He describes how to extend the module with additional fields by adding more database migrations and then modifying the code appropriately. 

Based on this approach, I have developed a couple of additional possibilities for creating custom modules. 

* **[Template Creation](template-creation.md)** - How to create a custom template that then can be used in the custom module dropdown to create modules with the given field structure

* **[Module Modification](module-modification.md)** - How to modify a custom external module that is generated to have the appropriate fields

Either of these approaches should work and the differences are minor. Probably in most cases the Module Modification is preferable since you will end up with an external module that can be copied and used by others. The Template Creation approach also creates an external module, but it requires some extra steps. 

