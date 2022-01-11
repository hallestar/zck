# powershell

## snippets

### 命令行启用emacs模式

```powershell
# Install-Module -Name PSReadLine -Allow Prerelease -Scope CurrentUser -Force -SkipPublisherCheck
Install-Module -Name PSReadLine -RequiredVersion 2.1.0 -AllowPrerelease
Set-PSReadLineOption -EditMode Emacs
```