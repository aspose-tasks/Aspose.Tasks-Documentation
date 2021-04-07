---
title: Handling Priorities
description: "Learn how to handle Microsoft Project (MPP/XML) priorities using Aspose.Tasks for Java."
type: docs
weight: 110
url: /java/handling-priorities/
---

{{% alert color="primary" %}} 

A task's priority helps Microsoft Project with automatic resource leveling (a process of fixing conflicts when a resource is over-allocated). In Microsoft Project, it is possible to assign priority values between 0 and 1000 (where 0 is the lowest priority). By default, tasks are assigned the value 500.

{{% /alert %}}

## **Working with Priorities**
The priorities associated with a class are handled through the PRIORITY property exposed by the [Tsk](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Tsk) class.

- Priority: a task's priority (integer between 1 and 1000).

#### **Priorities in Microsoft Project**
To check a task's priority in Microsoft Project one can double-click a task in the Task Entry form:

**Task priority in Microsoft Project** 

![checking task priorities in Microsoft Project](handling-priorities_1.png)

#### **Getting a Task's Priority**
The following examples show how to get a task's priority and write it to a console window using Aspose.Tasks.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandlePriorities-handle-priorities.java" >}}
