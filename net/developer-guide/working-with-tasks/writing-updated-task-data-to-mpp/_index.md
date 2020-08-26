---
title: Writing Updated Task Data to MPP
type: docs
weight: 230
url: /net/writing-updated-task-data-to-mpp/
---

{{% alert color="primary" %}} 

With Aspose.Tasks, it is possible to update [tasks](/tasks/net/working-with-tasks/) and then write the updated data back to a Microsoft Project MPP file.

{{% /alert %}} 
## **Updating Task Data**
The following code snippet shows how to update a project's task data and write it back to the MPP file. The step involved in this activity are:

1. Create an instance of the Project class.
1. Load the source MPP file.
1. Create a [Task](http://www.aspose.com/api/net/tasks/aspose.tasks/task) and add it to the root task.
1. Update the task parameters such as Deadline, NotesText, etc.
1. Add additional tasks to the root task.
1. Save the project.
### **Programming Samples**
The following code finds a task's original and external ID through the cross project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-UpdateTaskData-UpdateTaskData.cs" >}}
