---
title: Adding a New Task with Aspose.Tasks vs VSTO
type: docs
weight: 30
url: /net/adding-a-new-task-with-aspose-tasks-vs-vsto/
---

{{% alert color="primary" %}} 

While working with Microsoft Project files, you often need to add new tasks to projects. This article shows how to load MPP files in your .NET applications and add new tasks to your project using [VSTO](/tasks/net/adding-a-new-task-with-aspose-tasks-vs-vsto-html/) and [Aspose.Tasks for .NET](/tasks/net/adding-a-new-task-with-aspose-tasks-vs-vsto-html/).

{{% /alert %}} 
## **Add a Task Using VSTO**
To add a task using VSTO:

1. Create a new project in Visual Studio.
1. In the Solution Explorer, right-click and select **Add Reference**.
1. Select the COM components tab, and select **Microsoft Project 12.0 Object Library**.
1. Click **OK**.

This imports the Microsoft.Office.Interop.MSProject namespace at the start of your code. Use the code from the following example to add a new task.
### **Programming Samples - VSTO**


{{< highlight java >}}



// Create an Application object

Microsoft.Office.Interop.MSProject.Application projectApplication = new Application();

object missingValue = System.Reflection.Missing.Value;

// Open an MPP file

projectApplication.FileOpenEx(@"C:\Project1.mpp",

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

    missingValue, missingValue, missingValue, missingValue,

    missingValue);

// Create a Project object by assigning active project

Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;

// Create and add new task

Microsoft.Office.Interop.MSProject.Task task;

task = project.Tasks.Add("Task1", 1);

task.Start = "8/23/2012";

task.Duration = 3 * 8 * 60;

task.Text1 = "Task1";

// Save project and close application

projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);

{{< /highlight >}}
## **Add a Task Using Aspose.Tasks for .NET**
To add tasks to project files using Aspose.Tasks for .NET:

1. Create a new project in Visual Studio.
1. In the Solution Explorer, right-click and select **Add Reference**.
1. Select .NET tab and select **Aspose.Tasks**.
1. Click **OK**.

This imports the [Aspose.Tasks]() namespace at the start of your code. Use the code from the following example to add a new task.
### **Programming Sample - Aspose.Tasks**


{{< gist "aspose-tasks" "0655812ac3db2536958f" "Examples-CSharp-KnowledgeBase-AddNewTask-AddNewTask.cs" >}}
