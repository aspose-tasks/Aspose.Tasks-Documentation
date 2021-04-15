---
title: Creating a Task Link
description: "Learn how to create task links in Microsoft Project (MPP/XML) files using Aspose.Tasks for Java."
type: docs
weight: 10
url: /java/creating-a-task-link/
---

## **Create New Task Links**
A task link is created using the default constructor of [TaskLink](https://apireference.aspose.com/tasks/java/com.aspose.tasks/TaskLink) class which accepts three parameters:

1. The first parameter defines the predecessor Task,
2. the second parameter defines the successor Task and, finally,
3. the third parameter defines the task link type from values specified by the TaskLinkType enumeration type.

The following example creates a link between two tasks with Task1 as predecessor.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-TaskLinks-CreateTaskLink-create-task-line.java" >}}
