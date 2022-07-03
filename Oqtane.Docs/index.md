# MyLabBook Documentation

## Goals for MyLabBook

**We are building an open source Research Platform for the future, beginning with focusing on an Electronic Lab Notebook (ELN).** We especially have in mind 
those in the academic or startup communities who may be financially constrained but have the time and interest in using and helping to build a robust ELN 
for their own unique research and/or teaching needs.  

Our goal is to incorporate best practices that will lead to an outstanding ELN for the research community. Our [main goals](./overview/goals/index.md) include the following. 

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

In trying to meet these goals there are always trade-offs. Assessing the possibilities, we have decided to use the [Oqtane framework](https://oqtane.org) 
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

## Documentation Contents

This documentation for MyLabBook is structured as follows.

1. [Overview](./overview/index.md) contains information about the overall project, concepts, building the documentation, and article and video links
1. [Administration Manuals](./admin/index.md) has instructions for administrators
1. [Development](./development/index.md) has information about the structure of the Oqtane code and default custom modules and how to make your own modules  
1. [Examples](./examples/index.md) has various examples for how you might extend MyLabBook for your own use
1. [Code Documentation](./api/index.md) is extracted from the source code and organized for easy access 
1. To work on the docs, read up on [how the docs work](./overview/documentation/index.md)

** Note that this direction in development is a change from our use of the Drupal CMS for an ELN for the past 14 years

