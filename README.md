# devpc
Setup development tools and environment on a new Windows 11 PC 

``` powershell
winget install Microsoft.WindowsTerminal
winget install Microsoft.Powershell
winget install Git.Git
winget install Microsoft.AzureCLI
winget install Microsoft.VisualStudioCode
winget install Microsoft.VisualStudio.2022.Community
winget install Microsoft.DotNet.SDK.5
winget install Microsoft.DotNet.SDK.6
winget install Microsoft.Nuget
winget install GitHub.Cli
winget install Docker.DockerDesktop
winget install JanDeDobbeleer.OhMyPosh -s winget

Install-Module -Name Terminal-Icons -Repository PSGallery

exit
```

``` powershell
az login
gh auth login
oh-my-posh font install
code $PROFILE
```

``` powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\pure.omp.json" | Invoke-Expression
Import-Module -Name Terminal-Icons
```