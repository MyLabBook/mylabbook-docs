# Site Administration

![siteadminbanner](./assets/site-admin-banner.png)

Site administration involves managing a given website in the Oqtane instance. Icons for the tasks of a [Site Administrator](./role-management.html) are displayed in the [Admin Dashboard](../admin-navigation/admin-dashboard.html). These tasks are described more fully in the following sections. 

* **[File Management](./file-management.md)** - Offers folder add and edit capabilities. Offers file upload, delete and edit capabilities. 
* **[Language Management](./language-management.md)** - Manages language translations used on pages of the site.
* **[Page Management](./page-management.md)** - Lists all the website pages and offers add, edit, and delete capabilities.  
* **[Profile Management](./profile-management.md)** - Specifies custom fields for the user profiles.
* **[Recycle Bin](./recycle-bin.md)** - Offers features similar to the recycle bin on a desktop operating system. Used for deleted pages and modules. 
* **[Role Management](./role-management.md)** - Specifies custom roles and role permissions for creating and editing pages and modules. 
* **[Site Settings](./site-settings.md)** - Sets the website name, logo, favicon, theme, SMTP host, progressive web app settings, and more.
* **[Url Mappings](./url-mappings.md)** - Displays a list of mapped URLs or broken URLs.
* **[User Management](./user-management.md)** - Lists all the website users and offers add, edit, delete, and role setting capabilities, a global search function, and editable user profiles. 
* **[Visitor Management](./visitor-management.md)** - Displays records of login metadata for all website visitors.


### Administration Flexibility

A [Site Administrator](./role-management.html) has access to all of the features linked above when they are given the *Administrators* role. However it is also possible to create 

Site administration can take on many forms, but there are two use cases that you should be familiar with. First, there's site administration as defined by Oqtane.You enable this by adding the Administrators security role as one of the assigned roles for the account. That way, all “admin” features will be available for that user across that specific site.

Site administration can take on a hybrid of another sort as well, where you as the site administrator can define a different kind of administration for your site. This would be a kind of administration where you define a subset of administration capabilities and assign them to more privileged users to avoid having to make them an actual administrator.

As an example, there may be times when you want to create a security role in the [role manager](/admin/admin-dashboard/role-management.md) that might be named something like Site Admin. You would then create a page or pages on the site that contain some of the Admin modules, assigning permission to the newly created Site Admin security role so that only participants of that security role can see them. In these areas, you can also add references or links to features that normally require Administrator permissions, provided you set up your permissions properly in those other areas and that the chosen feature(s) allows this.

In summary, you can perform all of the configuration and content management tasks that you need to in order to run your own site.