---
title: Create Resources and Link with Tasks
description: "Learn how to create resources and resource assignments in the project using Aspose.Tasks for .NET in comparison with Microsoft Office Automation Tools."
type: docs
weight: 50
url: /net/create-resources-and-link-with-tasks/
---

{{% alert color="primary" %}}

While working with MPP files, you might need to create resources and link them to tasks from your project. This article gives an idea about how to load MPP files in your .NET applications and create resources and link to tasks from your projects using [VSTO](/tasks/net/create-resources-and-link-with-tasks/) and [Aspose.Tasks for .NET](/tasks/net/create-resources-and-link-with-tasks/).

{{% /alert %}}

## **Create Resources and Link them to Tasks using VSTO**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **COM components** tab.
3. Select Microsoft Project 12.0 Object Library and click **OK**. 
   This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.
4. Use the code from the following example to read tasks and resources.

The sample project file used in the following code snippets, SampleProject.mpp, can be downloaded from this page attachments. Before resources are created and linked to tasks, the Project1.mpp file looks as below.

## **Input file: Gantt chart view** 

![show input Gantt chart view](create-resources-and-link-with-tasks_1.png)

## **Input file: Resource sheet view** 

![show input resource sheet view](create-resources-and-link-with-tasks_2.png)

After processing, the file is updated.

## **Output file: Gantt chart view** 

![show output Gantt chart view](create-resources-and-link-with-tasks_3.png)

## **Output file: Resource sheet view** 

![show output resource sheet chart view](create-resources-and-link-with-tasks_4.png)

{{< highlight csharp >}}
Microsoft.Office.Interop.MSProject.Application projectApplication = new Application();
object missingValue = System.Reflection.Missing.Value;
projectApplication.FileOpenEx(@"SampleProject.mpp",
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, missingValue, missingValue,
    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
    missingValue, missingValue, missingValue, missingValue,
    missingValue);
Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;
int iResourceId = 1;
foreach (Task tsk in project.Tasks)
{
    string developer = "Developer0" + iResourceId;
    project.Resources.Add(developer, iResourceId);
    tsk.Assignments.Add(tsk.ID, iResourceId, missingValue);
    iResourceId++;
}
projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);
{{< /highlight >}}

## **Create Resources and Link to Tasks using Aspose.Tasks for .NET**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **.NET** tab.
3. Select **Aspose.Tasks** and then click **OK**.
   This imports the Aspose.Tasks namespace at the start of the code.
4. Use the code from the following example to create resources and link them to tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-KnowledgeBase-CreateResourcesAndLinkToTasks.cs" >}}
