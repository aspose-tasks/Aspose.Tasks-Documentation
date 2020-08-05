---
title: Writing Updated Task Data to MPP
type: docs
weight: 200
url: /cpp/writing-updated-task-data-to-mpp/
---

{{% alert color="primary" %}} 

With Aspose.Tasks, it is possible to update tasks and then write the updated data back to a Microsoft Project MPP file.

{{% /alert %}} 
## **Updating Task Data**
The following code snippet shows how to update a project's task data and write it back to the MPP file. The step involved in this activity are:

1. Create an instance of the Project class.
1. Load the source MPP file.
1. Create a [Task](https://apireference.aspose.com/cpp/tasks/class/aspose.tasks.task/) and add it to the root task.
1. Update the task parameters such as Deadline, NotesText, etc.
1. Add additional tasks to the root task.
1. Save the project.
### **Programming Samples**
The following code finds a task's original and external ID in the project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-UpdateTaskData-UpdateTaskData.cpp" >}}
