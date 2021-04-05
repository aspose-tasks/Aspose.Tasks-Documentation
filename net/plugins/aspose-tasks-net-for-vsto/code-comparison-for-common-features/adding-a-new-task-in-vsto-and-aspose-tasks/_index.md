---
title: Adding a New Task in VSTO and Aspose.Tasks
type: docs
weight: 10
url: /net/adding-a-new-task-in-vsto-and-aspose-tasks/
---

## **Code Examples**
### **VSTO**
To add a task using VSTO:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference.
3. Select the COM components tab, and select Microsoft Project 12.0 Object Library.
   Click OK.
4. This imports the Microsoft.Office.Interop.MSProject namespace at the start of your code. Use the code from the following example to add a new task. 

{{< highlight csharp >}}

 //Create an Application object

Microsoft.Office.Interop.MSProject.Application projectApplication = new MSProject.Application();

object missingValue = System.Reflection.Missing.Value;

//Open an MPP file

projectApplication.FileOpenEx("Project2.mpp",

	missingValue, missingValue, missingValue, missingValue,

	missingValue, missingValue, missingValue, missingValue,

	missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

	missingValue, missingValue, missingValue, missingValue,

	missingValue);

//Create a Project object by assigning active project

Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;

//Create and add new task

Microsoft.Office.Interop.MSProject.Task task;

task = project.Tasks.Add("Task1", 1);

task.Start = "8/23/2012";

task.Duration = 3 * 8 * 60;

task.Text1 = "Task1";

//Save project and close application

projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);

{{< /highlight >}}
### **Aspose.Tasks**
To add tasks to project files using Aspose.Tasks for .NET:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference.
3. Select .NET tab and select Aspose.Tasks.Click OK.This imports the Aspose.Tasks namespace at the start of your code. Use the code from the following example to add a new task. 

{{< highlight csharp >}}

 ProjectReader reader = new ProjectReader();

Project project = reader.Read("Project.mpp");

Aspose.Tasks.Task task = new Aspose.Tasks.Task("Task1");

task.ActualStart = DateTime.Parse("23-Aug-2012");

//Set duration in hours

task.Duration = new TimeSpan(24, 0, 0);

task.DurationFormat = TimeUnitType.Day;

project.RootTask.Children.Add(task);

//Recalculate task IDs

project.CalcTaskIds();

project.CalcTaskUids();

//Save the Project as XML

project.Save("OutputProject.xml", Aspose.Tasks.Saving.SaveFileFormat.XML);

{{< /highlight >}}
## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/download/AsposeTaskNETVsVSTOProjectv1.1/Adding.a.New.Task.Aspose.Tasks.zip)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-vsto/downloads/Adding%20a%20New%20Task%20(Aspose.Tasks).zip)
