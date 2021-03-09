---
title: Split Tasks in VSTO and Aspose.Tasks
type: docs
weight: 80
url: /net/split-tasks-in-vsto-and-aspose-tasks/
---

{{% alert color="primary" %}} 

Sometimes it is not possible to complete a task as scheduled and it needs to be split into two or more parts. Aspose.Tasks supports this Microsoft Project feature.

{{% /alert %}} 
## **VSTO**
Below is the code for VSTO Project to split tasks:

{{< highlight cs >}}

  string FileName = "MyProject.mpp";

 object missingValue = System.Reflection.Missing.Value;

 Application.FileOpenEx(FileName,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

    missingValue, missingValue, missingValue, missingValue,

    missingValue);

 Project MyProject = Application.ActiveProject;

 Task MyTask = MyProject.Tasks[1];

 MyTask.Split(DateTime.Parse("01.11.13 08:00"), DateTime.Parse("09.11.13 08:00"));


{{< /highlight >}}
## **Aspose.Tasks**
The SplitParts property exposed by the [Task\]() class is used to determine the split parts of a task whereas SplitTask method exposed by the ResourceAssignment class is used to split a single task into multiple parts. SplitParts returns a collection of split parts whereas SplitTask method accepts start date, finish date and calendar arguments to split the task.
#### **Splitting and Viewing Tasks in Microsoft Project**
To split a task in Microsoft Project:

1. Identify a long task and you want to divide.
2. On the **Task** menu, select the **Schedule** group and click **Split Task**.
3. Click at the position you want to split the task.

To see split tasks in Microsoft Project:

1. On the **View** menu, select **Gantt Chart**.
   Split tasks are linked by a dotted line. 
   **Split tasks in Microsoft Project** 
#### **Creating and Splitting Task**
To create and split a task, follow these steps:

1. Create a new project.
2. Create and assign a new calendar to the project.
3. Create and add a new task in the project.
4. Create and add a new resource assignment in the project.
5. Use the SplitTask method exposed by the ResourceAssignment class to split the task.
6. Write the new project to the disk.

The following code shows how to accomplish these tasks:

{{< highlight java >}}

  string FileName = "MyProject.mpp";

 Project MyProject = new Project(FileName);

 ResourceAssignment MyResource = MyProject.ResourceAssignments[0];

 MyResource.SplitTask(DateTime.Parse("01.11.13 08:00"), DateTime.Parse("09.11.13 08:00"), MyProject.Calendar);


{{< /highlight >}}
## **Download Running Code**
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO%20Projects/Code%20Comparison%20of%20Common%20Features/Split%20Task)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01/view/SourceCode#content)
## **Download Sample Code**
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01)
