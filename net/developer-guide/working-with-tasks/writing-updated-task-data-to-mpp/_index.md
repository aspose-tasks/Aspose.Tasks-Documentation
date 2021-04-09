---
title: Writing Updated Task Data to MPP
description: "Learn how to write Microsoft Project (MPP/XML) task properties using Aspose.Tasks for .NET."
type: docs
weight: 230
url: /net/writing-updated-task-data-to-mpp/
---

With Aspose.Tasks for .NET it is possible to update [tasks](/tasks/net/working-with-tasks/) and then write the updated data back to a Microsoft Project MPP file.

## **Updating Task Data**
The following code snippet shows how to update a project's task data and write it back to the MPP file. The step involved in this activity are:

1. Create an instance of the Project class.
2. Load the source MPP file.
3. Create a [Task](https://apireference.aspose.com/tasks/net/aspose.tasks/task) and add it to the root task.
4. Update the task parameters such as Deadline, NotesText, etc.
5. Add additional tasks to the root task.
6. Save the project.

The following code finds a task's original and external ID through the cross project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-UpdateTaskData-UpdateTaskData.cs" >}}
