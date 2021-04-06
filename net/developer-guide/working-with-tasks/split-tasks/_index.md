---
title: Split Tasks
type: docs
weight: 160
url: /net/split-tasks/
---

Sometimes it is not possible to complete a task as scheduled and it needs to be split into two or more parts. Aspose.Tasks supports this Microsoft Project feature.

## **Splitting Tasks**
The [SplitParts](https://apireference.aspose.com/tasks/net/aspose.tasks/task/properties/splitparts) property exposed by the [Task](https://apireference.aspose.com/tasks/net/aspose.tasks/task) class is used to determine the split parts of a task whereas [SplitTask](https://apireference.aspose.com/tasks/net/aspose.tasks/resourceassignment/methods/splittask) method exposed by the [ResourceAssignment](https://apireference.aspose.com/tasks/net/aspose.tasks/resourceassignment) class is used to split a single task into multiple parts. SplitParts returns a collection of split parts whereas SplitTask method accepts start date, finish date and calendar arguments to split the task.
### **Splitting and Viewing Tasks in Microsoft Project**
To split a task in Microsoft Project:

1. Identify a long task and you want to divide.
2. On the **Task** menu, select the **Schedule** group and click **Split Task**.
3. Click at the position you want to split the task.

To see split tasks in Microsoft Project:

1. On the **View** menu, select **Gantt Chart**.
   Split tasks are linked by a dotted line.

### **Creating and Splitting Task**
To create and split a task, follow these steps:

1. Create a new project.
2. Create and assign a new calendar to the project.
3. Create and add a new task in the project.
4. Create and add a new resource assignment in the project.
5. Use the SplitTask method exposed by the ResourceAssignment class to split the task.
6. Write the new project to the disk.

The following code shows how to accomplish these tasks:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-CreateSplitTasks-CreateSplitTasks.cs" >}}

### **Viewing Split Tasks with Aspose.Tasks**

The following example shows how to identify split tasks and printing their details to a console window.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ViewSplitTasks-ViewSplitTasks.cs" >}}
