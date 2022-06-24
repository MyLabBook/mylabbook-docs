# MyLabBook Documentation

![documentationbanner](./assets/documentation-banner.png)

Here we'll explain how the documentation works, with all the magic in it. 

## The Basics

The `MyLabBook.Docs` project generates the documentation for MyLabBook using [docfx](https://dotnet.github.io/docfx/).

The generator will compile all of MyLabBook and create an output into `../docs`. 
Note that this docs project is outside of the normal `oqtane.framework` repo structure, 
because it's meant to be deployed to a separate repo https://github.com/oqtane/oqtane.docs 
and then hosted on https://docs.oqtane.org

## Important Considerations

As of now (September 2020) docfx in Visual Studio still requires the full .net framework; a port to .net core is almost complete. 
For this reason, documentation generation currently still requires a windows PC. 
We'll transition to full .net core docs when docfx is ready, probably Q1 2021.
