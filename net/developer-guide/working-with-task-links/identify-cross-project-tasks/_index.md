---
title: Identify Cross Project Tasks
description: "Learn how to identify cross project Microsoft Project (MPP/XML) tasks using Aspose.Tasks for .NET."
type: docs
weight: 50
url: /net/identify-cross-project-tasks/
---

## **How to Identify Cross Project Tasks**
If you have linked a task from one project to a task from the other project, the IDs and UIDs of the task is different in the original and external projects as you can see in the following image:

![identifying external tasks in Microsoft Project](identify-cross-project-tasks_1.png)

The ExternalId property exposed by the [Task](https://reference.aspose.com/tasks/net/aspose.tasks/task) class is used to find an external task's original ID. The Id property returns the ID of the external task in the **external** project whereas the ExternalId property returns the ID of the external task in the **original** project.

The code below finds the original and external ID of a task.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskLinks-IdentifyCrossProjectTasks.cs" >}}
