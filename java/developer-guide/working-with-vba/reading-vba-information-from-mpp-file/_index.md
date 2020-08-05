---
title: Reading VBA Information from MPP File
type: docs
weight: 10
url: /java/reading-vba-information-from-mpp-file/
---

{{% alert color="primary" %}} 

Aspose.Tasks API provides support for reading VBA information from MPP file. This includes working with:

- Vba Information
- Modules information contained in the Project
- References Information stored in the Project

The VBaProject class is the main class for reading the VBA information from the project file. This further has Modules and References collection for reading further details of the VBA project file. This article demonstrates the usage of all these with the help of code samples.

{{% /alert %}} 
## **Reading VBA Project Information**
The following example shows how to read VBA Project Information with the help of VBaProject and Project class



**Java**

{{< highlight java >}}

 // loading project file

Project project = new Project("VbaProject1.mpp");

VbaProject vbaProject = project.getVbaProject();

System.out.println("VbaProject.Name " + vbaProject.getName());

System.out.println("VbaProject.Description " + vbaProject.getDescription());

System.out.println("VbaProject.CompilationArguments" + vbaProject.getCompilationArguments());

System.out.println("VbaProject.HelpContextId" + vbaProject.getHelpContextId());

{{< /highlight >}}
## **Reading References Information from VBA**
The following example shows how to read VBA References Information from VBA with the help of VBaProject, Project and VbaReference class

**Java**

{{< highlight java >}}

 // loading project file

Project project = new Project("VbaProject1.mpp");

VbaProject vbaProject = project.getVbaProject();

VbaReferenceCollection references = vbaProject.getReferences();

System.out.println("Reference count " +  references.getCount());

VbaReference reference = vbaProject.getReferences().toList().get(0);

System.out.println("Identifier: " + reference.getLibIdentifier());

System.out.println("Name: " + reference.getName());

reference = vbaProject.getReferences().toList().get(1);

System.out.println("Identifier: " + reference.getLibIdentifier());

System.out.println("Name: " + reference.getName());

reference = vbaProject.getReferences().toList().get(2);

System.out.println("Identifier: " + reference.getLibIdentifier());

System.out.println("Name: " + reference.getName());

{{< /highlight >}}
## **Reading Modules Information from VBA**
The following example shows how to read modules information from VBA with the help of VBaProject, Project and IVbaModule class

**Java**

{{< highlight java >}}

 Project project = new Project("VbaProject1.mpp");

VbaProject vbaProject = project.getVbaProject();

System.out.println("Total Modules Count: " + vbaProject.getModules().getCount());

IVbaModule vbaModule = vbaProject.getModules().toList().get(0);

System.out.println("Module Name: " + vbaModule.getName());

System.out.println("Source Code: " + vbaModule.getSourceCode());

{{< /highlight >}}
## **Reading Module Attributes Information from VBA**
The following example shows how to read modules attributes from VBA with the help of VBaProject, Project and IVbaModule class.

**Java**

{{< highlight java >}}

 // loading project file

Project project = new Project("VbaProject1.mpp");

VbaProject vbaProject = project.getVbaProject();

IVbaModule vbaModule = vbaProject.getModules().toList().get(0);

System.out.println("Attributes Count: " + vbaModule.getAttributes().getCount());

System.out.println("VB_Name: " + vbaModule.getAttributes().toList().get(0).getKey());

System.out.println("Module1: " + vbaModule.getAttributes().toList().get(0).getValue());

{{< /highlight >}}
