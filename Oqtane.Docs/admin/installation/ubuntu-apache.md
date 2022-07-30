# Installation

![installationbanner](./assets/installation-banner.png)

## Overview

This description is for installation of MyLabBook on the Ubuntu 22.04 operation system using the Apache 2 server software and the dot Net 6.0 framework. 

The steps of installation are listed below. 

* **[InstallUbuntu]()** 
* **[Install Apache]()**  
* **[Install the .NET framework]()**  
* **[Install MyLabBook]()** 
* **[Configure Apache]()**  
* **[Run MyLabBook]()** 


## Install Ubuntu

You can get anUbuntu VM on a hosting or cloud provider. Or you can download an iso for your local computer or local VM and run Ubuntu from there. 


## Install Apache

    sudo apt-get install apache2

    sudo a2enmod proxy proxy_http proxy_html proxy_wstunnel

    sudo a2enmod rewrite


## Install the .NET Framework and ASP.Net Core

    sudo apt-get update

    sudo apt-get install apt-transport-https

    sudo apt-get update

    sudo apt-get install dotnet-sdk-6.0

    sudo apt-get install aspnetcore-runtime-6.0

    sudo apt-get install dotnet-runtime-6.0


## Install MyLabBook

For now, we are just documenting how to install Oqtane until the MyLabBook repository is fully functional. 



## Configure Apache

For a publicly facing website, we assume that you have registered the domain example.com for your instance of MyLabBook. 
If you are running on a local computer we assume that you are using localhost. 

To set up apache, you will need to create a config file for the website. This file will initially be placed in the /etc/apache2/sites-available directory. 
An example config file follows, where of course you should replace example.com with your own domain name. We call this example.conf, but you should
use a name that corresponds to your actual domain. Note that apache expects the file to end with .conf. 

    <VirtualHost *:*>
        RequestHeader set "X-Forwarded-Proto" expr=%{REQUEST_SCHEME}
    </VirtualHost>

    <VirtualHost *:80>
        ProxyPreserveHost On
        ProxyPass / http://127.0.0.1:44357/
        ProxyPassReverse / http://127.0.0.1:44357/

        RewriteEngine on
        RewriteCond %{HTTP:UPGRADE} ^WebSocket$ [NC]
        RewriteCond %{HTTP:CONNECTION} Upgrade$ [NC]
        RewriteRule /(.*) ws://127.0.0.1:44357/$1 [P]

        ServerAdmin webmaster@example.com
        ServerName example.com
        ServerAlias *.example.com

        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined
    </VirtualHost>

After this file is created, use the following command to enable it. 

    sudo a2enmod example.conf 

Restart the apache server with the following command.
cd 
    sudo 

Also, you should set the /etc/hosts file with the appropriate entry

    127.0.0.1   example.com

To setup the SSL so that you can hae your site at https://example.com, then you can use the https://letsencrypt.org service for Apache on Ubuntu. 


## Run MyLabBook

From the MyLabBook directory, first build the application.

    cd <directory of MyLabBook>/Oqtane.Server

    dotnet build

You can run the application from the command line with 'dotnet run'. However, if you want to have the application run in the background 
and be able to close your SSH session, then type the following. 

    nohup dotnet run &


    



