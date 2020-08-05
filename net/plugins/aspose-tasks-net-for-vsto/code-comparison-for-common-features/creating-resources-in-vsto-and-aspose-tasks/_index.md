---
title: Creating Resources in VSTO and Aspose.Tasks
type: docs
weight: 50
url: /net/creating-resources-in-vsto-and-aspose-tasks/
---

## **VSTO**
Below is code sample to create resource in project.

{{< highlight cs >}}

  string FileName = @"E:\Aspose\Aspose Vs VSTO\Aspose.Tasks VS VSTO Projects\Sample Files\MyProject.mpp";

 object missingValue = System.Reflection.Missing.Value;

 Application.FileOpenEx(FileName,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

    missingValue, missingValue, missingValue, missingValue,

    missingValue);

 Project MyProject = Application.ActiveProject;

 MyProject.Resources.Add("Material");

 MyProject.Resources.Add("Work");

{{< /highlight >}}
## **Aspose.Tasks**
The [Resource](http://www.aspose.com/docs/display/tasksnet/Aspose.Tasks.Resource+Class) class allows to add a new resource to the project.

{{< highlight cs >}}

  string FileName = "MyProject.mpp";

 Project MyProject = new Project(FileName);

 MyProject.Resources.Add(new Resource("Material"));

 MyProject.Resources.Add(new Resource("Cost"));

{{< /highlight >}}
## **Download Running Code**
- [Codeplex](https://asposevsto.codeplex.com/SourceControl/latest#Aspose.Tasks Vs VSTO Project/Creating Resources/)
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO%20Projects/Code%20Comparison%20of%20Common%20Features/Creating%20Resources)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01/view/SourceCode#content)
## **Download Sample Code**
- [Codeplex](https://asposevsto.codeplex.com/releases/view/616887)
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01)
