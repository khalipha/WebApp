# WebApp
Restful API CRUD with EntityFramework and MVC

INSTRUCTIONS:


1) Download and extract the .zip file. (Extract All/WinRar)

2) Open the solution file in Visual Studio. (I was using Visual Studio Community Edition v17)

3) Build the solution to installs the missing NuGet packages.  (Ctrl+Shift+B)

4) Open the Package Manager Console, and run the update-database command to create the database. (Tools -> NuGet Package Manager ->  Package Manager Console)

  The *Command to run on the Package Manager Console terminal is:  "Update-Database"

   Having issues ?

   Try this command: 1) Update-Database -ConnectionString "data source=(LocalDb)\MSSQLLocalDB;initial catalog=ContosoUniversity;integrated security=True;MultipleActiveResultSets=True;App=EntityFramework" -ConnectionProviderName "System.Data.SqlClient" -Verbose
                     2) Add-Migration Version_Name -ConnectionString "data source=(LocalDb)\MSSQLLocalDB;initial catalog=ContosoUniversity;integrated security=True;MultipleActiveResultSets=True;App=EntityFramework" -ConnectionProviderName "System.Data.SqlClient" -Verbose  


   Still having issues: ?

   https://stackoverflow.com/questions/32195745/update-the-database-from-package-manager-console-in-code-first-environment
   https://www.entityframeworktutorial.net/code-first/code-based-migration-in-code-first.aspx

5)Run the application.



NB: ConnectionString on both web.config files:


  \ContosoUniversity\Views\Web.config
  \ContosoUniversity\Web.config

  <connectionStrings>
    <add name="SchoolContext" connectionString="Data Source=(LocalDb)\MSSQLLocalDB;Initial Catalog=ContosoUniversity;Integrated Security=SSPI;" providerName="System.Data.SqlClient" />
  </connectionStrings>



NB: Technologies used:


        C# </br>
        MVC </br>
        SQL SERVER (using System.Data.SqlClient;) </br>
        Restful WebAPI crud </br>
        Entity Framework 6</br>  https://www.entityframeworktutorial.net/code-first/code-based-migration-in-code-first.aspx






