# Dotnet_Scaffolding_Command_demo
# Dotnet command scaffolding tool controller and view

Dotnet Command Scaffolding Tool

```c#
Step 1. Modify *.csproj

 <ItemGroup>
    <PackageReference Include="microsoft.entityframeworkcore" Version="2.2.2" />
    <PackageReference Include="microsoft.entityframeworkcore.design" Version="2.2.2" />
    <PackageReference Include="Microsoft.VisualStudio.Web.CodeGeneration.Design" Version="2.2.2" />
  </ItemGroup>

  <ItemGroup>
    <DotNetCliToolReference Include="Microsoft.VisualStudio.Web.CodeGeneration.Tools" Version="2.0.4" />
  </ItemGroup>

Step 2. Open Cmd - dotnet restore
Step 3. test cmd - dotnet aspnet-codegenerator -h
Step 4. Make sure DbContext full path, You can check dbcontex using Cmd - dotnet ef dbcontext list
Step 5. dotnet aspnet-codegenerator controller -name EmployeeController -m Employee -outDir Controllers -dc Dotnet_Scaffolding_Command_demo.Data.ApplicationDbContext
