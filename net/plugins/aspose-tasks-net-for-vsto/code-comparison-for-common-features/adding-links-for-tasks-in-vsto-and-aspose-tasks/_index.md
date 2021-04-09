---
title: Adding Links for Tasks in VSTO and Aspose.Tasks
description: "Learn how to add Microsoft Project (MPP/XML) new task links using Aspose.Tasks for .NET. in comparison with VSTO."
type: docs
weight: 20
url: /net/adding-links-for-tasks-in-vsto-and-aspose-tasks/
---

## **Code Examples**
### **VSTO**
To link a task using VSTO:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference.
3. Select the COM components tab, and select Microsoft Project 12.0 Object Library.Click OK.This imports the Microsoft.Office.Interop.MSProject namespace at the start of your code. Use the code from the following example to link tasks.

{{< highlight csharp >}}
Microsoft.Office.Interop.MSProject.Application projectApplication = new MSProject.Application();
object missingValue = System.Reflection.Missing.Value;
projectApplication.FileOpenEx("Project.mpp",
	missingValue, missingValue, missingValue, missingValue,
	missingValue, missingValue, missingValue, missingValue,
	missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
	missingValue, missingValue, missingValue, missingValue,
	missingValue);
Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;
project.Tasks.get_UniqueID(2).TaskDependencies.Add(project.Tasks.get_UniqueID(1), PjTaskLinkType.pjFinishToStart);
project.Tasks.get_UniqueID(3).TaskDependencies.Add(project.Tasks.get_UniqueID(2), PjTaskLinkType.pjFinishToStart);
project.Tasks.get_UniqueID(4).TaskDependencies.Add(project.Tasks.get_UniqueID(3), PjTaskLinkType.pjFinishToStart);
project.Tasks.get_UniqueID(5).TaskDependencies.Add(project.Tasks.get_UniqueID(4), PjTaskLinkType.pjFinishToStart);
project.Tasks.get_UniqueID(5).TaskDependencies.Add(project.Tasks.get_UniqueID(2), PjTaskLinkType.pjFinishToStart);
foreach (Task tsk in project.Tasks)
{
	foreach (TaskDependency dep in project.Tasks.get_UniqueID(tsk.ID).TaskDependencies)
	{
		Console.WriteLine("From ID = " + dep.From.ID + "=>To ID = " + dep.To.ID);
	}
	Console.WriteLine("____________________________________________________________");
}
projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);
{{< /highlight >}}

### **Aspose.Tasks**
To link tasks in a project using Aspose.Tasks for .NET:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference.
3. Select .NET tab and select Aspose.Tasks.Click OK.This imports the Aspose.Tasks namespace at the start of your code. Use the code from the following example to link tasks.

{{< highlight csharp >}}
ProjectReader reader = new ProjectReader();
FileStream St = new FileStream("Project.mpp", FileMode.Open);
Project prj = reader.Read(St);
St.Close();
TaskLink taskLink = new TaskLink(prj.RootTask.Children[0] as Aspose.Tasks.Task, prj.RootTask.Children[1] as Aspose.Tasks.Task, TaskLinkType.FinishToStart);
prj.AddTaskLink(taskLink);
taskLink = new TaskLink(prj.RootTask.Children[1] as Aspose.Tasks.Task, prj.RootTask.Children[2] as Aspose.Tasks.Task, TaskLinkType.FinishToStart);
prj.AddTaskLink(taskLink);
taskLink = new TaskLink(prj.RootTask.Children[2] as Aspose.Tasks.Task, prj.RootTask.Children[3] as Aspose.Tasks.Task, TaskLinkType.FinishToStart);
prj.AddTaskLink(taskLink);
taskLink = new TaskLink(prj.RootTask.Children[3] as Aspose.Tasks.Task, prj.RootTask.Children[4] as Aspose.Tasks.Task, TaskLinkType.FinishToStart);
prj.AddTaskLink(taskLink);
taskLink = new TaskLink(prj.RootTask.Children[1] as Aspose.Tasks.Task, prj.RootTask.Children[4] as Aspose.Tasks.Task, TaskLinkType.FinishToStart);
prj.AddTaskLink(taskLink);
ArrayList allLinks = new ArrayList(prj.TaskLinks);
foreach (TaskLink taskLink1 in allLinks)
{
	Console.WriteLine("From ID = " + taskLink1.PredTask.Id + "=>To ID = " + taskLink1.SuccTask.Id);
	Console.WriteLine("________________________________________");
}
prj.Save("Project1.mpp", Aspose.Tasks.Saving.SaveFileFormat.MPP);
{{< /highlight >}}

## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/download/AsposeTaskNETVsVSTOProjectv1.1/Adding.Links.for.Tasks.Aspose.Tasks.zip)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-vsto/downloads/Adding%20Links%20for%20Tasks%20(Aspose.Tasks).zip)
