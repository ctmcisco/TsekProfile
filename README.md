# TsekProfile

My heavily customized Powershell profile.

## Instructions

This module can be loaded as-is by importing TsekProfile.psd1. This is mainly intended for development purposes.

To speed up module load time and minimize the amount of files that needs to be signed, distributed and installed, this module contains a build script that will package up the module into three files:

- TsekProfile.psd1
- TsekProfile.psm1
- LICENSE

To build the module, make sure you have the following pre-req modules:

- Pester (Required Version 4.1.1)
- InvokeBuild (Required Version 3.2.1)
- PowerShellGet (Required Version 1.6.0)
- ModuleBuilder (Required Version 1.0.0)

Start the build by running the following command from the project root:

```powershell
Invoke-Build
```

This will package all code into files located in .\bin\TsekProfile. That folder is now ready to be installed, copy to any path listed in you PSModulePath environment variable and you are good to go!

---
Maintained by Dan Tsekhanskiy ([tseknet.com](https://tseknet.com))
