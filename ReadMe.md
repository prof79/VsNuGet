## VsNuGet ##

This folder contains helper stuff/snippets for using Visual Studio and [NuGet](https://nuget.org).


### Files ###

* `NuGetNetStandard.targets`:
  `MSBuild` target for inclusion in a Visual Studio .NET Standard
  project/class library. Cleans old `.nupkg` files and deploys the current
  package to the OneDrive folder in the user profile.

* `NuGetNetFrameworkPcl.targets`:
  `MSBuild` target for inclusion in a Visual Studio regular
  project/class library (.NET Framework, PCL, UWP, ...).
  Cleans old `.nupkg` files and deploys the current package to the OneDrive
  folder in the user profile.

**Note:** Requires `nuget\nuget.exe` in your project root and a matching OneDrive path; destination could also be a file share or other path, adjust accordingly in the `.targets` file.


### Syntax ###

Add this line to your `.csproj` file:

`<Import Project="NuGetNetStandard.targets" />`

or

`<Import Project="NuGetNetFrameworkPcl.targets" />`


### Version ###

v1.0.1 2017-09-12T11:36:00+02


### License ###

Copyright (C) 2017 Markus M. Egger (prof79), [https://markusegger.at](https://markusegger.at)

v1.0.1 is public domain - use/modify at your own risk and leisure. See `LICENSE.md`.
