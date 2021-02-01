### Command Prompt basics

- Pipeline output is string(not real object)
  ```sh
  dir | sort 
  ```
- CMD has some builtin commands and can call executables
- It can perform fixed set of tasks

### Powershell basics

- Initially called Monad
- Provides an environment for executing live commands and creating powerful scripts
- Built on .NET framework
- It will output objects unlike cmd which outputs strings
  ```sh
  dir | sort-object -Descending -Property lastwritetime
  ```
- Uses common syntax(verb-noun pair command)
  ```sh
  get-process
  ```
- Powershell can work on non-windows
- Check PowerShell version
  ```sh
  Get-Host | Select-Object Version
  $psversiontable
  ```
- PowerShell 5 is the latest
- Future is moving to Powershell Core [6] but only shipped with Nano servers(which can't run .NET framework but on .NET core). It is most sutiable for container which need to be light weight.
- Most PowerShell works on PowerShell core but not all