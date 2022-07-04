---
title: Reading the Critical Path
description: "Learn how to read critical path from the Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET. in comparison with Microsoft Office Automation Tools."
type: docs
weight: 20
url: /net/reading-the-critical-path/
---

{{% alert color="primary" %}}

The critical path is the series of tasks (or even a single task) that dictates the calculated finish date of the project. That is, when the last task in the critical path is completed, the project is completed.

By knowing and tracking the critical path for your project, as well as the resources assigned to critical tasks, you can determine which tasks can affect your project's finish date and whether your project will finish on time.

If it's important for your project to finish on schedule, pay close attention to the tasks on the critical path and the resources assigned to them. These elements determine whether your project will finish on time.

This article gives a small idea of how to load MPP files in your .NET applications and read the critical path or the tasks on the critical path from your projects using [VSTO](/tasks/net/reading-the-critical-path/) and [Aspose.Tasks for .NET](/tasks/net/reading-the-critical-path/).

{{% /alert %}}

## **Read Critical Path Using VSTO**
Following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **COM components** tab.
3. Select the Microsoft Project 12.0 Object Library and then click **OK**.
   This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.
4. Use the code from the following example to read critical tasks.

{{< highlight csharp >}}
// Create Application object
Application projectApplication = new ApplicationClass();
object missingValue = System.Reflection.Missing.Value;
projectApplication.FileOpenEx(@"C:\Project1.mpp",
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
    missingValue, missingValue, missingValue, missingValue,
    missingValue);
Project project = projectApplication.ActiveProject;
foreach (Task task in project.Tasks)
{
    // Get critical tasks
    if (task != null)
    {
        if ((bool)task.Critical)
        {
            Console.WriteLine(task.ID + "  " + task.Name);
            Console.WriteLine(task.Start);
            Console.WriteLine(task.Finish + "\n");
        }
    }
}
// Make sure to clean up and close the file
projectApplication.FileCloseAll(PjSaveType.pjDoNotSave);
{{< /highlight >}}

## **Read Critical Path Using Aspose.Tasks for .NET**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **.NET** tab.
3. Select Aspose.Tasks and click **OK**.
   This imports the Aspose.Tasks namespace at the start of the code.
4. Use the code from the following example to read tasks and resources.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-KnowledgeBase-ReadCriticalPath.cs" >}}
