# Awesome Entity Framework Core

## Official Websites
* [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/)
* [Microsoft.EntityFrameworkCore (NuGet)](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore)

## Entity Framework Core 5.0
* [Announcing Entity Framework Core 5.0 Preview 3](https://devblogs.microsoft.com/dotnet/announcing-entity-framework-core-5-0-preview-3/) - (April 2020)

## Videos
#### Entity Framework Core
* [Entity Framework Core Part 1](https://www.youtube.com/watch?v=xx5_pVsLP44) (Phil Japikse, April 2020)
* [Entity Framework Core Part 2](https://www.youtube.com/watch?v=ta46892FM6g) 
* [Entity Framework Core Part 3](https://www.youtube.com/watch?v=KtnkkEPlm44)
* [Entity Framework Core Part 4](https://www.youtube.com/watch?v=aX9EBlRM9U8)
* [Entity Framework Core Part 5](https://www.youtube.com/watch?v=iFHsQuBB6ZU)


#### Entity Framework Core In-Depth
* [Entity Framework Core In-Depth Part 1](https://www.youtube.com/watch?v=Y__n6OOt9IQ) (Phil Japikse, June 2020)

#### Others
* [Mapping DDD Domain Models with EF Core 2.1](https://www.youtube.com/watch?v=Z62cbp61Bb8) (Julie Lerman, May 2019)

## Tutorials
* [Learn Entity Framework Core](https://www.learnentityframeworkcore.com/) - learnentityframeworkcore.com
* [Entity Framework Core](https://www.entityframeworktutorial.net/efcore/entity-framework-core.aspx) - entityframeworktutorial.net
* [Entity Framework Core Tutorial](https://www.dotnetcurry.com/entityframework/1347/entity-framework-ef-core-tutorial) - dotnetcurry.com
* [Entity Framework Core Series](https://code-maze.com/entity-framework-core-series/) - code-maze.com
* Installation (PMC)
  * [Installing Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/get-started/install/)
    * Install-Package Microsoft.EntityFrameworkCore.SqlServer
    * Install-Package Microsoft.EntityFrameworkCore.Tools
    * Install-Package Microsoft.EntityFrameworkCore.Design
* Connection String
  * [Connection Strings](https://docs.microsoft.com/en-us/ef/core/miscellaneous/connection-strings) - Microsoft
  * [The Connection Strings Reference](https://www.connectionstrings.com/)
  * [UDL File](https://blogs.msdn.microsoft.com/farukcelik/2007/12/31/basics-first-udl-test/)
* Tools Commands
  * [Entity Framework Core tools reference](https://docs.microsoft.com/en-us/ef/core/miscellaneous/cli/powershell)
* Scaffolding (Database First)
  * [Entity Framework Core Database First Example (YouTube)](https://www.youtube.com/watch?v=iX-fb1ddfjM) - Programming
  * [Reverse Engineering](https://docs.microsoft.com/en-us/ef/core/managing-schemas/scaffolding)
  * [Generating a model from an existing database](https://www.learnentityframeworkcore.com/walkthroughs/existing-database) 
  * [Fluent API or Data Annotations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/scaffolding#fluent-api-or-data-annotations)
  * [Entity Framework Core tools reference](https://docs.microsoft.com/en-us/ef/core/miscellaneous/cli/powershell#scaffold-dbcontext)
    * Examples:
      * Scaffold-DbContext "Server=(local);Database=AdventureWorks;Trusted_Connection=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -t Production.Product, Production.ProductSubcategory -DataAnnotations
      * Script-Migration -To Initial
      * Script-Migration -From 0
      * Update-Database -Migration 0 (The number 0 is a special case that means before the first migration and causes all migrations to be reverted.)
* Validation
  * [Model validation in ASP.NET Core MVC and Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/mvc/models/validation) - Microsoft Docs
  * [Validation in ASP .NET Core](https://wakeupandcode.com/validation-in-asp-net-core/) - Wake Up And Code!   
* Logging
  * [Logging](https://docs.microsoft.com/en-us/ef/core/miscellaneous/logging?tabs=v3)
* Migration
  * [Custom Migrations Operations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/operations)
* [Using HierarchyID in Entity Framework](https://softwarehut.com/blog/tech/hierarchyid-entity-framework) - Paweł Kondzior

## SQLite
* [SQLite in .NET Core with Entity Framework Core](https://kontext.tech/column/dotnet_framework/275/sqlite-in-net-core-with-entity-framework-core) - kontext.tech
* [DB Browser for SQLite](https://sqlitebrowser.org/) - DB Browser for SQLite (DB4S) is a high quality, visual, open source tool to create, design, and edit database files compatible with SQLite.

## Database Providers
* [Database Providers](https://docs.microsoft.com/en-us/ef/core/providers/?tabs=dotnet-core-cli)
* [InMemory is designed to be a general purpose database for testing](https://docs.microsoft.com/en-us/ef/core/miscellaneous/testing/in-memory) - Microsoft Docs

## EF with ASP.NET MVC
* [ASP.NET Core MVC with EF Core](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/)
* [Razor Pages with Entity Framework Core in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro)


## Advanced
* Separation of Concerns (SoC)
  * Articles and Resources
    * [.NET Core — Using Entity Framework Core in a separate Project](https://medium.com/oppr/net-core-using-entity-framework-core-in-a-separate-project-e8636f9dc9e5) - Rodrigo Santos (Medium)
    * [Should you split your ASP.NET MVC project into multiple projects?](https://programmingwithmosh.com/net/should-you-split-your-asp-net-mvc-project-into-multiple-projects/) - Mosh Hamedani
  * Sample
    * Class Lib: Project.Domain (POCO)
    * Class Lib: Project.Data (Context); Reference Domain; EF SQLServer, EF Tools
    * Web Application: Project.Web (ASP.NET MVC); Reference Data; EF Design
* Patterns
  * [Repository and Unit of Work Pattern](https://www.programmingwithwolfgang.com/repository-and-unit-of-work-pattern/) - Wolfgang Ofner
  * [Implementing the Repository and Unit of Work Patterns in an ASP.NET MVC](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions/getting-started-with-ef-5-using-mvc-4/implementing-the-repository-and-unit-of-work-patterns-in-an-asp-net-mvc-application)
