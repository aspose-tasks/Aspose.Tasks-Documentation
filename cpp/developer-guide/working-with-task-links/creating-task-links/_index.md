---
title: Creating Task Links
type: docs
weight: 10
url: /cpp/creating-task-links/
---

## **Overview**
Microsoft Project allows to link tasks based on the relationship between these. A task link is defined by a predecessor and a successor task. Task links can be of different types including FinishToFinish, FinishToStart, StartToFinish, and StartToStart. Aspose.Tasks API provides users with the capability to define task links in their project using the [TaskLink](https://apireference.aspose.com/cpp/tasks/class/aspose.tasks.task_link/) class.
## **Creating a Task Link**
A task link is created using the default constructor (TaskLink) which accepts three parameters:

1. The first parameter defines the predecessor Task,
1. the second parameter defines the successor Task and, finally,
1. the third parameter defines the task link type from values specified by the TaskLinkType enumeration type. This is an optional parameter.

The following example creates a link between two tasks with Task1 as predecessor.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTaskLinks-CreateTaskLinks-CreateTaskLinks.cpp" >}}
