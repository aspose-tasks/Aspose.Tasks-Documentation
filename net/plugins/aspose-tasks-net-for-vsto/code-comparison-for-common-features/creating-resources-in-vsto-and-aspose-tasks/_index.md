---
title: Creating Resources in VSTO and Aspose.Tasks
description: "Learn how to create resources in Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET in comparison with VSTO."
type: docs
weight: 50
url: /net/creating-resources-in-vsto-and-aspose-tasks/
---

## **Code Examples**

### **VSTO**
Below is code sample to create resource in project.

{{< highlight csharp >}}
string filename = @"E:\Aspose\Aspose Vs VSTO\Aspose.Tasks VS VSTO Projects\Sample Files\MyProject.mpp";
object missingValue = System.Reflection.Missing.Value;
Application.FileOpenEx(filename,
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
    missingValue, missingValue, missingValue, missingValue,
    missingValue);
Project project = Application.ActiveProject;
project.Resources.Add("Material");
project.Resources.Add("Work");
{{< /highlight >}}

### **Aspose.Tasks**
The [Resource](https://apireference.aspose.com/tasks/net/aspose.tasks/resource) class allows to add a new resource to the project.

{{< highlight csharp >}}
Project project = new Project("MyProject.mpp");
project.Resources.Add(new Resource("Material"));
project.Resources.Add(new Resource("Cost"));
{{< /highlight >}}

## **Download Running Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO/Code%20Comparison/Creating%20Resources)

## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
