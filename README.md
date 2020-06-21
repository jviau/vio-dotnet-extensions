# Vio.Dotnet.Templates

Contains dotnet templates for use with `dotnet new`

## Vio.Dotnet.Templates.Class

Item template for generating a simple C# class. Does not poplate namespace or perform any smart replacements besides name.

**Usage**: `dotnet new class -n ClassName`

**Outputs**: A C# class file.

## Vio.Dotnet.Templates.Proj

Project template for generating a `src` and `test` project tuple.

**Usage**: `dotnet new proj -n ProjectName -o OutputFolder`

**Outputs**: Two projects, a classlib at `src/ProjectName.csproj` and a xunit test project at `test/ProjectName.Tests.csproj`

## Vio.Dotnet.Templates.Repo

Project (repo) template for scaffolding out a new C# repo structure.

**Usage**: `dotnet new repo -n RepoName -o OutputFolder`

**Outputs**:

- .gitignore
- .editorconfig
- Directory.Build.props/targets/rsp
- global.json
- Packages.props (contains analyzers, for use with [Microsoft.Build.CentralPackageVersions]([Microsoft.Build.CentralPackageVersions](https://github.com/microsoft/MSBuildSdks/tree/master/src/CentralPackageVersions)))
- readme.md
- releasenotes.md
- version.json (for Nerdbank.GitVersioning)
- eng:
  - Analyzers.ruleset
  - Common.props/targets
  - stylecop.json
  - Test.props/targets
- src:
  - solution
