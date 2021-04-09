---
title: Estimated and Milestone Tasks
description: "Learn how to work with Microsoft Project (MPP/XML) estimated and milestone tasks using Aspose.Tasks for C++."
type: docs
weight: 60
url: /cpp/estimated-and-milestone-tasks/
---

{{% alert color="primary" %}}

In Microsoft Project, milestones are used to monitor a project's progress. Milestones are crucial points in the project. Typically, a milestone's a task with no duration but any task can be marked as a milestone. Aspose.Tasks for C++ API helps you manage milestones.

{{% /alert %}}

## **Working with Milestones**
The Tsk class exposes the IsEstimated and IsMilestone properties to manage estimated and milestone tasks:

- IsEstimated: set and get whether a task is estimated (bool value).
- IsMilestone: set and get whether a task is a milestone (bool value).

### **Viewing Estimated and Milestone Tasks in Microsoft Project**
To see whether a task is estimates of marked as a milestone in Microsoft Project one can double-click a task in the Task Entry form: 

![marking an estimated task as a milestone in Microsoft Project](managing-estimated-milestone-tasks_1.png)

### **Finding out Whether a Task is Estimated or a Milestone**
The following code example demonstrates how to find out whether a task is estimated or a milestone using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-FindEstimatedMilestoneTasks-FindEstimatedMilestoneTasks.cpp" >}}
