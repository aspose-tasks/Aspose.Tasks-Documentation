---
title: Identify Cross-Project Tasks
type: docs
weight: 50
url: /java/identify-cross-project-tasks/
---

**Linking tasks between projects**
If you have linked a task from one project to a task from the other project, the IDs and UIDs of the task is different in the original and external projects as you can see in the following image.


## **Internal and external IDs in Microsoft Project** 

![viewing cross project links](identify-cross-project-tasks_1.png)

The ExternalId property exposed by the [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/task/) class is used to find an external task's original ID. The Id property returns the ID of the external task in the **external** project whereas the ExternalId property returns the ID of the external task in the **original** project.

The code below finds the original and external ID of a task.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-TaskLinks-IdentifyCrossProjectTasks-identify-cross-project-tasks.java" >}}
