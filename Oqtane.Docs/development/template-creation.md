# Template Creation

I created a proof-of-concept custom template that is used for generating custom modules. 
I began with the default template that is located at:

```
oqtane.framework/Oqtane.Server/wwwroot/Modules/Templates/External
```

I copied that folder and named the new folder External2 (I imagine that the name doesn't matter, so it should be named more appropriately).

Then I changed some files using VS Code, using the writeup at [Michael Washington's Blazor Helpsite](https://blazorhelpwebsite.com/ViewBlogPost/4) as a guide. 
The files that I changed are as follows. 

**template.json** - Changed the Title appropriately

**/Shared/Models/Module.cs** - Added fields to the module definition 

**/Server/Migrations/EntityBuilders/[Module]EntityBuilder.cs** - Add new fields in 2 places:

```
protected override [Module]EntityBuilder BuildTable(ColumnsBuilder) Table {
    ...
}

public OperationBuilder<AddColumnOperation> MyNewFieldName { get; set; }
```

**/Client/Modules/Edit.razor** - Changed 5 different places for each field. Michael's write-up can be used as a guide. 

Once these changes are made, then the template should show up in the drop down for the template to use for a custom module. 
If this template is chosen, then it should create a module with the new fields that have been added in this template. 


