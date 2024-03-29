---
title: Overtimes in Tasks
description: "Learn how to assign overtime values for Microsoft Project (MPP/XML) tasks using Aspose.Tasks for .NET."
type: docs
weight: 170
url: /net/overtimes-in-tasks/
---

Microsoft Project lets users assign overtime to tasks. Aspose.Tasks for .NET supports this functionality through two properties in the Task class.

## **Overtime**
The [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) exposes several properties for working with overtime:

- [OvertimeCost](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/overtimecost): reads and writes the sum of a task's actual and remaining overtime cost (double).
- [OvertimeWork](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/overtimework): reads and writes the amount of overtime scheduled for a task (TimeSpan).

### **Microsoft Project view of task overtime**
To see a task's overtime work and cost properties:

1. In the Task Entry form, select the **Insert** menu and then **Column**.
2. Add the overtime columns.

### **Getting task overtimes in Aspose.Tasks**
The following examples show how to get the overtime cost and work associated with a task with Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskOvertimes.cs" >}}
