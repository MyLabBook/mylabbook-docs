# MyLabBook Documentation

## Goals for MyLabBook

**We are building an Electronic Lab Notebook (ELN) for the future.** We especially have in mind those in the academic or startup communities who may be constrained by 
monetary budgets but have the time and interest in using and helping us to build a robust ELN for your own unique research.  

Our goal is to learn from other successful projects and then to incorporate best practices that will lead to an outstanding ELN for the research community.
We would love to have you join us. 

Some of our main goals include the following. 

* Be free and open source with a liberal license
* Be fast and easy to install
* Be cross platform (Linux, Windows, Mac)
* Minimize the learning curve for immediate productivity 
* Maximize the speed and productivity of development 
* Be easily customizable for any research project
* Have excellent documentation for installation, customization, and for the internal architecture  
* Be built on widely supported technical foundations 
* Have accuracy in scientific and technical computations 
* Scale from Raspberry Pi up through sophisticated cloud computing
* Integrate with widely used research software packages as simply as possible 
* Build on a strong open source community
* Have an efficient runtime 

### Our Solution

In trying to meet these goals there are always trade-offs. Looking at the possibilities in 2022 and assessing the possibilities for the future, we have decided
on the use of the [Oqtane framework](https://oqtane.org) for MyLabBook going forward**. It is still a relatively young framework, but it has some fairly unique
characteristics compared to other possibilities. 

* [Blazor](https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor) provides the following advantages. 
  * Allows sophisticated front end development (i.e., the browser interface) using C#, the same language as is used for the server code.
  * Utilizes WASM in the browser, opening up many previously unavaiable computational possibilities
  * Productive environment through simplification of component building 
  * Long term support from Microsoft
  * Liberal Apache license
  * Excellent free and paid development environments (Visual Studio, VS Code, JetBrains Rider)
  * Cross platform (Linux, Window, Mac)
* The [Oqtane framework](https://oqtane.org) provides the additional advantages.
  * Micro-frontend allowing separate backend feed-through. This will be useful for utilizing different scientific packages on the backend 
    with a common interface in the browser.
  * Developed by a team with experience building DNN, the previously most successful open source .NET content management system
  * Themeable
  * Supports multiple databases (MySQL, PostgreSQL, SQL Server, SQLite)
  * Supports extension through independent modules
  * Liberal MIT license

## Our Status

How far are we towards meeting our goals? Again, this is a relative judgment, but the choice of Blazor and Oqtane already provide significant strengths. 

MyLabBook already has the following features. 

* Free and open source with an MIT license
* Fast and easy to install for the standard installation
* Built on widely supported technical foundations of .NET and Blazor 
* Accuracy in scientific and technical computations with C# and .NET
* Strong .NET and Blazor open source communities and a growing Oqtane community
* Have an efficient runtime with .NET CLR
* Free and productive development environments (Visual Studio Community edition, VS Code)

While some of the following capabilities are available to varying degrees, there is also a need for improvement in these areas. Your participation can make a difference!

Click the link to find out the current status of this goal and visions and plans for how these goals might be achieved more fully. 

* [More fully cross platform]() (Linux, Windows, Mac)
* [Minimization of the learning curve]()
* [Maximization of the speed of development]()
* [Customizability for any research project]()
* [Excellent documentation]() for installation, customization, and for the internal architecture  
* [Scalability from a Raspberry Pi up through sophisticated cloud computing]()
* [Integration with widely used research software packages]() as simply as possible 
* [Development of a strong open source community for MyLabBook]()



## Documentation Contents

This website focuses on documentation concerning this approach of using Oqtane as the basis for an outstanding ELN. 

1. In the [Overview](./overview/index.md) you'll find information about the project, concepts, building the documentation, and article and video links
1. The [Administration Manuals](./admin/index.md) you'll find instructions for administrators
1. The [Blogs](./blogs/index.md) has blogs for the legacy MyLabBook as well as our new approach with Oqtane  
1. In the [API Documentation](./api/index.md) you'll find all the APIs
1. To work on the docs, read up on [how the docs work](./overview/documentation/index.md)

** Note that this direction in development is a change from our use of the Drupal CMS for an ELN for the past 14 years

