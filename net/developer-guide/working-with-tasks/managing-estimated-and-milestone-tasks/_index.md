---
title: Managing Estimated and Milestone Tasks
type: docs
weight: 80
url: /net/managing-estimated-and-milestone-tasks/
---

{{% alert color="primary" %}} 

In Microsoft Project, milestones are used to monitor a project's progress. Milestones are crucial points in the project. Typically, a milestone's a task with no duration but any task can be marked as a milestone. Aspose.Tasks helps you manage milestones.

{{% /alert %}} 
## **Working with Milestones**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes the [IsEstimated](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/isestimated) and [IsMilestone](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/ismilestone) properties to manage estimated and milestone tasks:

- IsEstimated: set and get whether a task is estimated (boolean).
- IsMilestone: set and get whether a task is a milestone (boolean).
### **Viewing Estimated and Milestone Tasks in Microsoft Project**
To check whether a task is estimates of marked as a milestone in Microsoft Project one need to double-click on a task in the Task Entry form:

![is the task a milestone or estimated](managing-estimated-and-milestone-tasks_1.png)
### **Finding out Whether a Task is Estimated or a Milestone**
The following code examples show how to find out whether a task is estimated or a milestone using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-FindEstimatedMilestoneTasks-FindEstimatedMilestoneTasks.cs" >}}
