# Best Restaurants

#### An application that allows the user to log resturaunt details and search based on cuisine

#### Created By: Brandon Eads, Chynna Lew

## Technologies Used

* C#
* .NET 5
* NuGet
* ASP.NET Core
* Entity Framework Core
* MySql
* MySql Workbench

## Description

This application allows the user to create and store a list of restaurants, logging the name, cuisine type, proce range, etc. The user can view their list, view the types of cuisines, and search for restaurants by cuisine type.
This application was created for Epicodus to demonstrate an understanding of ASP.NET Core MVC, SQL databases, and one to many relationships in C#. 

* Project objectives:
  - Create cuisine and resturant classes
  - Build out all CRUD functionality
  - Create a SQL database with tables for each class
  - Properly connect the cuisine and resturant classes
  - Allow the user to search for all of a cuisine's restaurants

## Setup and Usage Instructions

### Technology Requirements

* Download and install [.NET 5](https://dotnet.microsoft.com/download/dotnet/5.0)
* Download and install a code text editor. Ex: [VS Code](https://code.visualstudio.com/)
* Download, install, and complete setup for [MySql Community Server](https://dev.mysql.com/downloads/file/?id=484914) and [MySql Workbench](https://dev.mysql.com/downloads/file/?id=484391).

### Installation

* Clone [this](github.com/beads89/BestRestaurants) repository, or download and open the Zip on your local machine
* Open the BestRestaurants.Solutions folder in your preferred text editor
* To install required packages, navigate to the terminal and type the following commands:
  - dotnet add package Microsoft.EntityFrameworkCore -v 5.0.0
  - dotnet add package Pomelo.EntityFrameworkCore.MySql -v 5.0.0-alpha.2
  - dotnet add package Microsoft.EntityFrameworkCore.Proxies -v 5.0.0
* Create a file named "appsettings.json" in the BestRestaurants directory
  - add the following code to the appsettings.json file:
  ```
  {
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=best_restaurants;uid=root;pwd=[YOUR-PASSWORD-HERE];"
    }
  }
  ```
  - replace [YOUR-PASSWORD-HERE] with your unique MySql password
* Launch the MySql server:
  - In the terminal, run the command "$ mySql -uroot -p[YOUR-PASSWORD-HERE]", replacing [YOUR-PASSWORD-HERE] with your unique MySql password
* To Import the required database:
  - Open MySql Workbench
  - Select your preferred server(default is root)
  - In the "Navigator > Administration" window, select "Data Import/ Restore"
  - In "Import Options", select "Import From Self-Contained File"
  - Navigate to "BestRestaurants.Solutions/best_restaurants.sql" in the search input
  - Under "Default Schema to be Imported to" select the "New" button
  - Enter "best_restaurants" and click "OK"
  - Navigate to the "Import Progress" tab and click "Start Import" in the bottom right corner of the window
  - Reopen the "Navigator>Schemas" tab, Right click and select "refresh all" to see the imported database
* To Restore, build, and run the project:
  - Navigate to the BestRestaurants.Solutions/BestRestaurants folder in the command line or terminal
    - Run the command "$ dotnet restore" to restore the project dependencies
    - Run the command "$ dotnet build" to build and compile the project
    - Run the command "$ dotnet run" to build and compile the project

## Known Bugs

* no known bugs

### License

[MIT License](https://opensource.org/licenses/MIT)
Copyright 2021 Brandon Eads, Chynna Lew

## Support and contact details

* [Brandon Eads](github.com/beads89)
* [Chynna Lew](github.com/chynnalew) <ChynnaLew@yahoo.com>