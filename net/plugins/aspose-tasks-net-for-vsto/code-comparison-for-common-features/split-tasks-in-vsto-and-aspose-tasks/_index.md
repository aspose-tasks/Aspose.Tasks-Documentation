---
title: Split Tasks in VSTO and Aspose.Tasks
description: "Learn how to split Microsoft Project (MPP/XML) tasks using Aspose.Tasks for .NET in comparison with VSTO."
type: docs
weight: 80
url: /net/split-tasks-in-vsto-and-aspose-tasks/
---

Sometimes it is not possible to complete a task as scheduled and it needs to be split into two or more parts. Aspose.Tasks for .NET supports this Microsoft Project feature.

## **Code Examples**

### **VSTO**
Below is the code for VSTO Project to split tasks:

{{< highlight csharp >}}
object missingValue = System.Reflection.Missing.Value;
Application.FileOpenEx("MyProject.mpp",
   missingValue, missingValue, missingValue, missingValue,
   missingValue, missingValue, missingValue, missingValue,
   missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
   missingValue, missingValue, missingValue, missingValue,
   missingValue);
Project project = Application.ActiveProject;
Task MyTask = project.Tasks[1];
MyTask.Split(DateTime.Parse("01.11.13 08:00"), DateTime.Parse("09.11.13 08:00"));
{{< /highlight >}}

### **Aspose.Tasks**
The SplitParts property exposed by the [Task](https://reference.aspose.com/tasks/net/aspose.tasks/task) class is used to determine the split parts of a task whereas SplitTask method exposed by the ResourceAssignment class is used to split a single task into multiple parts. SplitParts returns a collection of split parts whereas SplitTask method accepts start date, finish date and calendar arguments to split the task.

#### **Splitting and Viewing Tasks in Microsoft Project**
To split a task in Microsoft Project:

1. Identify a long task and you want to divide.
2. On the **Task** menu, select the **Schedule** group and click **Split Task**.
3. Click at the position you want to split the task.

To see split tasks in Microsoft Project one can select **Gantt Chart** on the **View** menu.  Split tasks are linked by a dotted line.

#### **Creating and Splitting Task**
To create and split a task, follow these steps:

1. Create a new project.
2. Create and assign a new calendar to the project.
3. Create and add a new task in the project.
4. Create and add a new resource assignment in the project.
5. Use the SplitTask method exposed by the ResourceAssignment class to split the task.
6. Write the new project to the disk.

The following code shows how to accomplish these tasks:

{{< highlight csharp >}}
Project project = new Project("MyProject.mpp");
ResourceAssignment MyResource = project.ResourceAssignments[0];
MyResource.SplitTask(DateTime.Parse("01.11.13 08:00"), DateTime.Parse("09.11.13 08:00"), project.Calendar);
{{< /highlight >}}

## **Download Running Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO/Code%20Comparison/Split%20Task)

## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
