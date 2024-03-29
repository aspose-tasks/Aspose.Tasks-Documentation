---
title: System Requirements
description: "Before you start working with Aspose.Tasks for .NET, ensure that your environment fits the operating system, platform, frameworks, and environment requirements."
type: docs
keywords: "Aspose.Tasks for .NET System Requirements .NET 6.0 Linux Support"
weight: 50
url: /net/system-requirements/
---

Aspose.Tasks for .NET can be used to build any type of 32-bit or 64-bit .NET application including ASP.NET, WCF, WinForms, WPF etc. It is possible to use Aspose.Tasks for .NET via COM Interop from ASP, Perl, PHP and Python. Aspose.Tasks for .NET can also be used to build applications with Mono.

## **Supported Operating Systems**
Aspose.Tasks for .NET supports any 32-bit or 64-bit operating system where .NET or Mono framework is installed including, but not limited to:

### **Windows**
- Microsoft Windows Server 2003 (x64, x86)
- Microsoft Windows Server 2008 (x64, x86)
- Microsoft Windows Server 2012 (x64, x86)
- Microsoft Windows Server 2016 (x64, x86)
- Microsoft Windows Server 2019 (x64, x86)
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows Vista (x64, x86)
- Microsoft Windows XP (x64, x86)
- Microsoft Windows 7 (x64, x86)
- Microsoft Windows 8, 8.1 (x64, x86)
- Microsoft Windows 10 (x64, x86)

### **Linux**
- Linux (Ubuntu, OpenSUSE, CentOS and others)

### **Mac**
- Mac OS X

## **Supported Frameworks**
Aspose.Tasks for .NET supports .NET and Mono frameworks as follows:

### **.NET Frameworks**
- .NET Framework 3.5
- .NET Framework 4.0
- .NET Framework 4.0 Client Profile
- .NET Framework 4.5
- .NET Framework 4.5.1
- .NET Framework 4.5.2
- .NET Framework 4.6
- .NET Framework 4.6.2
- .NET Framework 4.5
- .NET Framework 4.5.1
- .NET Framework 4.5.2
- .NET Framework 4.6
- .NET Framework 4.6.1
- .NET Framework 4.6.2
- .NET Framework 4.7
- .NET Framework 4.7.1
- .NET Framework 4.7.2
- .NET Framework 4.8
- .NET Standard 2.0
- .NET Core 2.0
- .NET Core 2.1
- .NET Core 2.2
- .NET Core 3.1
- .NET 5
- .NET 6

### **Mono Framework**
- Mono 2.6.7 or later

## **Development Environments**
Aspose.Tasks for .NET can be used to develop applications in any development environment that targets the .NET platform, but the following environments are explicitly supported:

- Microsoft Visual Studio 2010
- Microsoft Visual Studio 2011
- Microsoft Visual Studio 2012
- Microsoft Visual Studio 2013
- Microsoft Visual Studio 2015
- Microsoft Visual Studio 2017
- Microsoft Visual Studio 2019
- Microsoft Visual Studio 2022
- MonoDevelop 2.4 and later

## **Limitations of .NET Core/Mono support**
There are some features of Aspose.Tasks that does not implement in .NET Core/Mono for Linux/MacOS and supported for .NET Framework/.NET Core/Mono for Windows only:
- On Linux/MasOS Aspose.Tasks does not support MPD files because there is no OLE DB driver implementation for these OSes. Check, for instance, the Mono [documentation](https://www.mono-project.com/docs/database-access/).
- Aspose.Tasks does not support the export/import of EMF/WMF images on Linux/MacOS. These formats are usually being used in RTF header/footer of page info. In this case Aspose.Tasks is exporting the text information of headers and/or footers.

## **Limitations of version targeting .NET 6**

Print-related methods are not supported, even for Windows platform.
Thus the following methods are not present in version for .NET 6.0:

```
Project.Print(PrintOptions)
Project.Print(string)
Project.Print(PrinterSettings)
Project.Print(PrinterSettings,string)
Project.Print(PrinterSettings,PrintOptions)
Print(PrinterSettings,PrintOptions,string)
```

Also the following type is excluded: Aspose.Tasks.Saving.PrintOptions.


