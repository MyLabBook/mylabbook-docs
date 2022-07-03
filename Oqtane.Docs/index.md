# MyLabBook Documentation

## Goals for MyLabBook

**We are building an Electronic Lab Notebook (ELN) for the future.** We especially have in mind those in the academic or startup communities who may be financially 
constrained but have the time and interest in using and helping to build a robust ELN for your own unique research and/or teaching needs.  

Our goal is to incorporate best practices that will lead to an outstanding ELN for the research community. Our main goals include the following. 

* Free and open source with a liberal license
* Fast and easy to install
* Cross platform (Linux, Windows, Mac)
* Minimize the learning curve for immediate productivity 
* Maximize the speed and productivity of development 
* Easily customizable for any research project
* Excellent documentation for installation, customization, and for the internal architecture  
* Built on widely supported technical foundations 
* Accuracy in scientific and technical computations 
* Scale from Raspberry Pi up through sophisticated cloud computing
* Integrate with widely used research software packages as simply as possible 
* Build on a strong open source community
* Have an efficient runtime 

## Our Solution

In trying to meet these goals there are always trade-offs. Assessing the possibilities, we have decided to use of the [Oqtane framework](https://oqtane.org) 
for MyLabBook going forward**. Oqtane is a relatively young framework, but it has some fairly unique characteristics. 

* [Blazor](https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor) provides the following advantages. 
  * The front end (i.e., the browser interface) is developed with C#, the same language used for the server side code.
  * Utilizes [WASM](https://webassembly.org/) in the browser, opening up many previously unavailable computational possibilities
  * Productive environment through simplified component building 
  * Long term support from Microsoft
  * Liberal Apache license
  * Excellent free and paid development environments (Visual Studio, VS Code, JetBrains Rider)
  * Cross platform (Linux, Window, Mac)
* The [Oqtane framework](https://oqtane.org) provides the additional advantages.
  * Micro-frontend allowing multiple backend sources. This will be useful for utilizing different scientific packages on the backend 
    with a common interface in the browser.
  * Developed by a team with experience building [DNN](https://www.dnnsoftware.com/), the most successful open source .NET content management system to date
  * Themeable
  * Supports multiple databases (MySQL, PostgreSQL, SQL Server, SQLite)
  * Highly extensible through independent modules
  * Liberal MIT license

## The Status of MyLabBook Development

How far are we towards meeting our goals? This is a relative judgment, but the choice of Blazor and Oqtane provide significant strengths. 

MyLabBook already fully supports the following goals. 

* Free and open source with an MIT license
* Fast and easy to install for the standard installation
* Built on widely supported technical foundations of .NET and Blazor 
* Accuracy in scientific and technical computations with C# and .NET
* Strong .NET and Blazor open source communities and a growing Oqtane community
* Have an efficient runtime with .NET CLR
* Free and productive development environments (Visual Studio Community edition, VS Code)

The remaining goals are available to varying degrees, with room for improvement. 
Click a link to find out the current status of the goal and plans for how these goals might be achieved more fully. 

* [More fully cross platform (Linux, Windows, Mac)]()
* [Minimization of the learning curve]()
* [Maximization of the speed of development]()
* [Customizability for any research project]()
* [Excellent documentation for installation, customization, and for the internal architecture]()  
* [Scalability from a Raspberry Pi up through sophisticated cloud computing]()
* [Integration with widely used research software packages as simply as possible]() 
* [Development of a strong open source community for MyLabBook]()


## Documentation Contents

This documentation for MyLabBook is structured as follows.

1. [Overview](./overview/index.md) contains information about the overall project, concepts, building the documentation, and article and video links
1. [Administration Manuals](./admin/index.md) has instructions for administrators
1. [Development](./development/index.md) has information about the structure of the Oqtane code and default custom modules and how to make your own modules  
1. [Examples](./examples/index.md) has various examples for how you might extend MyLabBook for your own use
1. [Code Documentation](./api/index.md) is extracted from the source code and organized for easy access 
1. To work on the docs, read up on [how the docs work](./overview/documentation/index.md)

** Note that this direction in development is a change from our use of the Drupal CMS for an ELN for the past 14 years

