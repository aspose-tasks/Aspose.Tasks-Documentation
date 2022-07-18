---
title: Creating Task Links
description: "Learn how to edit Microsoft Project (MPP/XML) task links using Aspose.Tasks for .NET."
type: docs
weight: 10
url: /net/creating-task-link/
---

Microsoft Project allows to link tasks based on the relationship between these. A task link is defined by a predecessor and a successor task. Task links can be of different [types](https://reference.aspose.com/tasks/net/aspose.tasks/tasklinktype) including FinishToFinish, FinishToStart, StartToFinish, and StartToStart. Aspose.Tasks for .NET API provides users with the capability to define task links in their project using the [TaskLink](https://reference.aspose.com/tasks/net/aspose.tasks/tasklink) class.

## **Creating a Task Link**
A task link is created using the default constructor (TaskLink) which accepts three parameters:

1. The first parameter defines the predecessor Task,
2. the second parameter defines the successor Task and, finally,
3. the third parameter defines the task link type from values specified by the TaskLinkType enumeration type. This is an optional parameter.

The following example creates a link between two tasks with Task1 as predecessor.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskLinks-CreateTaskLinks.cs" >}}
