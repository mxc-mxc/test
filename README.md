# test
Programming instructions
=====
I. Description of development 
----
    This program uses the latest.NET 5 development, can be deployed under Windows, Linux run (install.NET 5 runtime)
    Development tool: Visual Studio 2019 16.8.3
    Database: Install MS SQL SERVER 2016 Localdb (the default installation when Visual Studio is installed)
II. Engineering structure description
----
    ConsoleMVC: View layer, console program;
    Console VcBusiness is the business logic layer that controls the program business logic;
    ConsolMVCRepository is the data access layer. It uses EntityFrameworkCore to access the database.
    ConsoleMVCTest is a test project. This program is rarely used.
III.Description of program design
----
    This program is divided into view layer (console), business logic layer, data access layer, data layer (database).The layer invocation is built by dependency injection and the database access is implemented by EntityframeworkCore.
IV. Project description
---
ConsolMVC
-----
    View items:
    The Db directory is MS SQLSERVER Localdb database file.
    The Doc directory is the documentation for the program.
    The View directory is implemented as the Console interface
    Appsettings.json configuration file, configuring database connection string, with detailed instructions.
    Program.cs is the boot class that is described in detail.
ConsoleMVCBusiness Business logic layer
-----
    Models are view Models, and the code inside the model accessed as an interface is detailed.
    Service is a domain object, defines the domain operation interface, the code is detailed.
Console VCrepository Data access layer
-----
    Entity directory, database Entity layer, with detailed annotations in corresponding database tables.
    Repository database entity warehouse class, corresponding to the database table of additions, deletions, changes, search operations, code with detailed comments.
