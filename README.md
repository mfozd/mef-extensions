mef-extensions
======
This project is solving the problem of removal [Managed Extensibility Framework (MEF)](https://msdn.microsoft.com/en-us/library/dd460648(v=vs.110).aspx) project plugin.

## Problem
MEF does not allow you to remove plugins(dll files) while the process is running. The reason is that the process use dll while it is running and operating system does not allow you to remove these files. Consequently, you can not remove plugins, you can add only.

## Solution
Solution of the problem were managed [mef](https://msdn.microsoft.com/en-us/library/dd460648(v=vs.110).aspx) plugings with a yaml file. You can add remove plugins using yaml file.
Yaml file:
 * plugins-dir : directory that contains plugins
 * plugins: list of plugins (dlls)

The content of sample [yaml](http://www.yaml.org) file is as follows :
```
plugins-dir : .\plugins
plugins:
 - a.dll
 - b.dll
```

## Third part libraries
* see [LIBRARIES](https://github.com/mfozd/mef-extensions/blob/master/LIBRARIES.md) file

## Licence
* see [LICENCE](https://github.com/mfozd/mef-extensions/blob/master/LICENSE) file

## Sample Project
* see [mef-extensions-example](https://github.com/mfozd/mef-extensions-example) project

## Contact
#### Developer
  * e-mail : mehmetfatihozd@gmail.com
