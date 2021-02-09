---
title: Overtimes in Tasks
type: docs
weight: 170
url: /net/overtimes-in-tasks/
---

{{% alert color="primary" %}} 

Microsoft Projects lets users assign overtime to tasks. Aspose.Tasks supports this functionality through two properties in the Task class.

{{% /alert %}} 
## **Overtime**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) exposes several properties for working with overtime:

- [OvertimeCost](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/overtimecost): reads and writes the sum of a task's actual and remaining overtime cost (double).
- [OvertimeWork](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/overtimework): reads and writes the amount of overtime scheduled for a task (TimeSpan).
### **Microsoft Project view of task overtime**
To see a task's overtime work and cost properties:

1. In the Task Entry form, select the **Insert** menu and then **Column**.
1. Add the overtime columns.
### **Getting task overtimes in Aspose.Tasks**
The following examples show how to get the overtime cost and work associated with a task with Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskOvertimes-ReadTaskOvertimes.cs" >}}
