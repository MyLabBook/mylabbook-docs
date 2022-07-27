# Installation

![installationbanner](./assets/installation-banner.png)


## Install an Official Release on IIS

The [Official Oqtane Relases are found on Github](https://github.com/oqtane/oqtane.framework/releases)

Read the [detailed instructions for installing Oqtane on IIS](https://www.oqtane.org/Resources/Blog/PostId/542/installing-oqtane-on-iis)

## Upgrade an Existing Oqtane

Read the [instructions for upgrading Oqtane](https://www.oqtane.org/Resources/Blog/PostId/543/upgrading-oqtane)

## Reset an Existing Oqtane

If you have already installed a previous version of Oqtane and you wish to do a clean database install, simply reset the `DefaultConnection` value in the `Oqtane.Server\appsettings.json` file to "". 
This will trigger a re-install when you run the application which will execute the database installation scripts.

## Install Oqtane for Development

### Oqtane Version 3 (.NET 6)

1. Install **[.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)**
   
1. Install the latest edition of [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) with the **ASP.NET and web development** workload enabled.
Oqtane works with ALL editions of Visual Studio from Community to Enterprise.

1. If you wish to use _LocalDB_ for development (not a requirement as Oqtane supports _SQLite_, _mySQL_ and _PostgreSQL_) you must also install the **Data storage and processing**.

1. Clone the Oqtane dev branch source code to your local system. Open the **Oqtane.sln** solution file and Build the solution.

1. Make sure you specify **Oqtane.Server** as the Startup Project and then Run the application.

