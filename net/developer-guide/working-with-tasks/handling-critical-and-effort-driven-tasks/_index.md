---
title: Handling Critical and Effort-Driven Tasks
description: "Learn how to handle with Microsoft Project (MPP/XML) critical and effort-driven tasks using Aspose.Tasks for .NET."
type: docs
weight: 90
url: /net/handling-critical-and-effort-driven-tasks/
---

{{% alert color="primary" %}} 

Microsoft Project recognized a number of different types of tasks. Tasks with no duration, for example, are considered milestones by default. Critical tasks make up the critical path, one or a series of tasks that, ultimately, determines how long a project will take.

{{% /alert %}}

## **Working with Critical and Effort-Driven Tasks**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes the [IsCritical](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/iscritical) and [IsEffortDriven](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/iseffortdriven) properties to handle critical and effort driven tasks:

- IsCritical sets or gets whether a task is critical (boolean).
- IsEffortDriven: sets or gets whether a task is effort-driven (boolean).

### **Critical and Effort-driven Tasks Microsoft Project**
To check whether a task is critical or effort-driven in Microsoft Project one need to double-click a task in the Task Entry form:

![is the task critical or effort-driven](handling-critical-and-effort-driven-tasks_1.png)

### **Getting Critical and Effort-Driven Tasks**
The following code examples show how to get information about whether a task is critical or effort-driven.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-FindCriticalEffortDrivenTasks-FindCriticalEffortDrivenTasks.cs" >}}
