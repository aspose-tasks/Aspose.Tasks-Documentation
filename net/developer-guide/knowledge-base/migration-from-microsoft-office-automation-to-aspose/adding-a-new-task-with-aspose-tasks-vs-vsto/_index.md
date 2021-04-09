---
title: Adding a New Task with Aspose.Tasks vs VSTO
description: "Learn how to add new tasks to the project using Aspose.Tasks for .NET in comparison with Microsoft Office Automation Tools."
type: docs
weight: 30
url: /net/adding-a-new-task-with-aspose-tasks-vs-vsto/
---

{{% alert color="primary" %}}

While working with Microsoft Project (MPP/XML) files, you often need to add new tasks to projects. This article shows how to load MPP files in your .NET applications and add new tasks to your project using [VSTO](/tasks/net/adding-a-new-task-with-aspose-tasks-vs-vsto/) and [Aspose.Tasks for .NET](/tasks/net/adding-a-new-task-with-aspose-tasks-vs-vsto/).

{{% /alert %}}

## **Add a Task Using VSTO**
To add a task using VSTO:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**.
3. Select the COM components tab, and select **Microsoft Project 12.0 Object Library**.
4. Click **OK**.

This imports the Microsoft.Office.Interop.MSProject namespace at the start of your code. Use the code from the following example to add a new task.

### **Programming Samples - VSTO**

{{< highlight csharp >}}
Microsoft.Office.Interop.MSProject.Application projectApplication = new Application();
object missingValue = System.Reflection.Missing.Value;
projectApplication.FileOpenEx(@"C:\Project1.mpp",
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
    missingValue, missingValue, missingValue, missingValue,
    missingValue);
Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;
Microsoft.Office.Interop.MSProject.Task task;
task = project.Tasks.Add("Task1", 1);
task.Start = "8/23/2012";
task.Duration = 3 * 8 * 60;
task.Text1 = "Task1";
projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);
{{< /highlight >}}

## **Add a Task Using Aspose.Tasks for .NET**
To add tasks to project files using Aspose.Tasks for .NET:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**.
3. Select .NET tab and select **Aspose.Tasks**.
4. Click **OK**.

This imports the **Aspose.Tasks** namespace at the start of your code. Use the code from the following example to add a new task.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-KnowledgeBase-AddNewTask-AddNewTask.cs" >}}
