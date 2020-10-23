---
title: Writing Updated Task Data to MPP
type: docs
weight: 230
url: /java/writing-updated-task-data-to-mpp/
---

{{% alert color="primary" %}} 

With Aspose.Tasks, it is possible to update [tasks](/tasks/java/working-with-tasks/) and then write the updated data back to a Microsoft Project MPP file.

{{% /alert %}} 
**Updating Task Data**
The following code snippet shows how to update a project's task data and write it back to the MPP file. The step involved in this activity are:

1. Create an instance of Project Reader.
1. Read the source MPP file.
1. Create a [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task/) and add it to the root task.
1. Update the task parameters such as Deadline, NotesText, etc.
1. Add additional tasks to the root task.
1. Save the project.

The following code finds a task's original and external ID through the cross-project.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-UpdatedTaskDataToMpp-updated-tasks-to-mpp.java" >}}
