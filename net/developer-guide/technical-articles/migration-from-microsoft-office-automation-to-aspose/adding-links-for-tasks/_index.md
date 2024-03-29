---
title: Adding Links for Tasks
description: "Learn how to add new task links to the project using Aspose.Tasks for .NET in comparison with Microsoft Office Automation Tools."
type: docs
weight: 40
url: /net/adding-links-for-tasks/
---

{{% alert color="primary" %}}

Tasks linking is often required while working with Microsoft Project (MPP/XML) files. In VSTO, TaskDependencies.Add() is used for adding task links; Aspose.Tasks uses Project.TaskLinks.Add() to link tasks.

VSTO provides access to these links using MSProject.Project.Tasks.get_UniqueID(taskID).TaskDependencies. It provides a collection of dependencies that can be used to display and otherwise process requirements like access to detailed properties.

In Aspose.Tasks for .NET Project.TaskLinks provides a collection of links which can be used for display and accessing detailed properties of these links like LinkType, PredTask, SuccTask etc.

This article shows how to load MPP files in your .NET application and add/display link tasks using [VSTO](/tasks/net/adding-links-for-tasks/) and [Aspose.Tasks for .NET](/tasks/net/adding-links-for-tasks/).

{{% /alert %}}

## **Link Tasks Using VSTO**
To link a task using VSTO:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**.
3. Select the COM components tab, and select **Microsoft Project 12.0 Object Library**.
4. Click **OK**.

This imports the Microsoft.Office.Interop.MSProject namespace at the start of your code. Use the code from the following example to link tasks.

{{< highlight csharp >}}
Microsoft.Office.Interop.MSProject.Application projectApplication = new Application();
object missingValue = System.Reflection.Missing.Value;
projectApplication.FileOpenEx(@"D:\Aspose\Migration\SampleProject.mpp",
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
// Display the dependencies
foreach (Task tsk in project.Tasks)
{
    foreach (TaskDependency dep in project.Tasks.get_UniqueID(tsk.ID).TaskDependencies)
    {
        Console.WriteLine("From ID = " + dep.From.ID  + "=>To ID = " + dep.To.ID);
    }
    Console.WriteLine("____________________________________________________________");
}
// Save the project
projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);
{{< /highlight >}}

## **Link Tasks Using Aspose.Tasks for .NET**
To link tasks in a project using Aspose.Tasks for .NET:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**.
3. Select .NET tab and select **Aspose.Tasks**.
4. Click **OK**.

This imports the **Aspose.Tasks** namespace at the start of your code. Use the code from the following example to link tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-KnowledgeBase-LinkTasks.cs" >}}
