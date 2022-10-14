# dotnet reminders

```powershell
# create a new solution file
dotnet new sln --name mysolution
```

```c#
// how to exclude a project from code coverage
<AssemblyAttribute Include="System.Diagnostics.CodeAnalysis.ExcludeFromCodeCoverageAttribute" />
```

```powershell
# how to get code coverage

# add a reference to the coverlet nuget package
<PackageReference Include="coverlet.collector" />

# go to the test project folder
dotnet test --collect:"XPlat Code Coverage"

# go to the folder TestResults/{guid}
reportgenerator -reports:"coverage.cobertura.xml" -targetdir:"coveragereport" -reporttypes:Html

```
