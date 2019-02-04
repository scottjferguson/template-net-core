<img src="{{logo-img-url}}" alt="{{application-name-lower}}">

[![Build status](https://ci.appveyor.com/api/projects/status/q261l3sbokafmx1o/branch/master?svg=true)](https://ci.appveyor.com/project/relay/{{application-name-lower}}/branch/master)
[![NuGet Release](http://img.shields.io/nuget/v/{{application-name-lower}}.svg)](https://www.nuget.org/packages/{{application-name-lower}}/)
[![NuGet Downloads](https://img.shields.io/nuget/dt/{{application-name-lower}}.svg)](https://www.nuget.org/packages/{{application-name-lower}})
[![License](https://img.shields.io/github/license/relay-dev/{{application-name-lower}}.svg)](https://github.com/relay-dev/core/{{application-name-lower}}/master/LICENSE)

# {{application-name-lower}}}

{{application-description}}}

## Folder structure
<sup>(https://gist.github.com/davidfowl/ed7564297c61fe9ab814)</sup>

```
$/
  artifacts/
  build/
  docs/
  lib/
  packages/
  samples/
  src/
  tests/
  .editorconfig
  .gitignore
  .gitattributes
  build.cmd
  build.sh
  LICENSE
  NuGet.Config
  README.md
  {solution}.sln
```


- `src` - Main projects (the product code)
- `tests` - Test projects
- `docs` - Documentation stuff, markdown files, help files etc.
- `samples` (optional) - Sample projects
- `lib` - Libraries that your application depends on, which you cannot obtian by way of NuGet
- `artifacts` - Build outputs go here. Doing a build.cmd/build.sh generates artifacts here (nupkgs, dlls, pdbs, etc.)
- `packages` - NuGet packages
- `build` - Build customizations (custom msbuild files/psake/fake/albacore/etc) scripts
- `build.cmd` - Bootstrap the build for windows
- `build.sh` - Bootstrap the build for *nix
- `global.json` - ASP.NET vNext only

## .gitignore
```
[Oo]bj/
[Bb]in/
.nuget/
_ReSharper.*
packages/
artifacts/
*.user
*.suo
*.userprefs
*DS_Store
*.sln.ide
```

