# asp.net-react-template

# Setting up Asp.net project with React Frontend.  Using "Clean Architecture"

Requirements
-
 - NET CORE, VS CODE, Node.JS, React, PostMan, Swagger

Extensions
-
- Bracket Pair Colorizer, C#, C# Extensions, Material Theme Icon, NuGet Gallery, SQLite

Walking Skeleton - API
-
What is a Walking Skeleton?
- A Walking Skeleton is a tiny implementation of the system that performs a small end-to-end function.  It need not use the final architecture but it hsould link together the main architectural components.  The achitecture and the functionality can then evolve in parallel.

Creating Project Files Using .net CLI
-
- See Info: 
<code>dotnet --info</code>
- See available templates
<code>dotnet new -l
- Create a new directory.  Cd into directory and make a solution file
<code>mkdir aspNetReact-Template</code>
<code>cd aspNetReact-Template</code>
<code>dotnet new sln</code>
- Create projects
<code>dotnet new webapi -n API</code>
<code>dotnet new classlib -n Application</code>
<code>dotnet new classlib -n Domain</code>
<code>dotnet new classlib -n Persistence</code>
- Add project to solution file
<code>dotnet sln add API/<code>
<code>dotnet sln add Application/</code>
<code>dotnet sln add Persistence/</code>
<code>dotnet sln add Domain</code>
- Check to see projects in solution
<code> dotnet sln list</code>

Add dependencies	
- 
-  cd into API, add dependency
<code>dotnet add reference ../Application </code>
- cd into Application/, add reference to Persistence and Domain
<code>dotnet add reference ../Persistence
<code>dotnet add reference ../Domain
- cd into Persistence/, add reference to Domain
<code>dotnet add reference ../Domain


Run API
-
- cd into the API/ directory and run with watch
<code>cd */API/</code>
<code>dotnet watch run </code>








