# csharp-console-app-osx
Empty Console App to run with Visual Studio Code on OSX

## Setting up the Environment

1. Install [Visual Studio Code](https://www.visualstudio.com/en-us/products/code-vs.aspx)

2. Install .NET Version Manager (DNVM) by running the following:
 ```
 curl -sSL https://raw.githubusercontent.com/aspnet/Home/dev/dnvminstall.sh | DNX_BRANCH=dev sh && source ~/.dnx/dnvm/dnvm.sh
 ```

3. Use DNVM to install DNX for .NET Core:
 ```
 dnvm upgrade -r coreclr
 ```

4. Install Mono
 ```
 brew update & brew install mono
 ```

5. Use DNVM to install DNX for Mono:
 ```
 dnvm upgrade -r mono
 ```

### Starting a new app

1. Clone this repo

2. Move to the new project location and run:
 ```
 dnu restore
 dnu build
 dnx . run
 ```
