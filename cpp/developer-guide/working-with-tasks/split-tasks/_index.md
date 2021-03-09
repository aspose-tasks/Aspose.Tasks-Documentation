---
title: Split Tasks
type: docs
weight: 80
url: /cpp/split-tasks/
---

{{% alert color="primary" %}} 

Sometimes it is not possible to complete a task as scheduled and it needs to be split into two or more parts. Aspose.Tasks API supports this Microsoft Project feature.

{{% /alert %}} 
## **Splitting Tasks**
The SplitParts property exposed by the [Task](http://www.aspose.com/api/net/tasks/aspose.tasks/task) class is used to determine the split parts of a task whereas SplitTask method exposed by the ResourceAssignment class is used to split a single task into multiple parts. SplitParts returns a collection of split parts whereas SplitTask method accepts start date, finish date and calendar arguments to split the task.
### **Splitting and Viewing Tasks in Microsoft Project**
To split a task in Microsoft Project:

1. Identify a long task and you want to divide.
2. On the **Task** menu, select the **Schedule** group and click **Split Task**.
3. Click at the position you want to split the task.

To see split tasks in Microsoft Project:

1. On the **View** menu, select **Gantt Chart**.
   Split tasks are linked by a dotted line.
### **Creating and Splitting Task**
To create and split a task, follow these steps:

1. Create a new project.
2. Create and assign a new calendar for the project.
3. Create and add a new task in the project.
4. Create and add a new resource assignment in the project.
5. Use the SplitTask method exposed by the ResourceAssignment class to split the task.
6. Write the new project to the disk.

The following code shows how to accomplish these tasks:

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-CreateSplitTasks-CreateSplitTasks.cpp" >}}


Viewing Split Tasks with Aspose.Tasks

The following example shows how to identify split tasks and printing their details to a console window.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ViewSplitTasks-ViewSplitTasks.cpp" >}}
### **Calculating a Split Task's Finish Date**
The following code example calculates finish date for a split task.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-CalculateSplitTaskFinishDate-CalculateSplitTaskFinishDate.cpp" >}}
