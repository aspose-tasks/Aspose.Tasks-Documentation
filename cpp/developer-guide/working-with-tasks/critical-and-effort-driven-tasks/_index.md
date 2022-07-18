---
title: Critical and Effort-Driven Tasks
description: "Learn how to work with Microsoft Project (MPP/XML) critical and effort-driven tasks using Aspose.Tasks for C++."
type: docs
weight: 90
url: /cpp/critical-and-effort-driven-tasks/
---

{{% alert color="primary" %}}

Microsoft Project recognized a number of different types of tasks. Tasks with no duration, for example, are considered milestones by default. Critical tasks make up the critical path, one or a series of tasks that, ultimately, determines how long a project will take.

{{% /alert %}}

## **Working with Critical and Effort-Driven Tasks**
The [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes the IsCritical and IsEffortDriven properties to handle critical and effort driven tasks:

- IsCritical sets or gets whether a task is critical (bool value).
- IsEffortDriven: sets or gets whether a task is effort-driven (bool value).

### **Critical and Effort-driven Tasks in Microsoft Project**
To check whether a task is critical or effort-driven in Microsoft Project double-click a task in the Task Entry form:

![check is task effort driven in Microsoft Project](handling-critical-and-effort-driven-tasks_1.png)

### **Getting Critical and Effort-Driven Tasks**
The following code examples demonstrate how to get information about whether a task is critical or effort-driven.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-FindCriticalEffortDrivenTasks-FindCriticalEffortDrivenTasks.cpp" >}}
