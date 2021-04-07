---
title: Overtimes in Tasks
description: "Learn how to assign overtime values for Microsoft Project (MPP/XML) tasks using Aspose.Tasks for C++."
type: docs
weight: 160
url: /cpp/overtimes-in-tasks/
---

Microsoft Project lets users assign overtime to tasks. Aspose.Tasks for C++ API supports this functionality through two properties in the Task class.

## **Overtime**
The [Tsk] (https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.tsk) exposes several properties for working with overtime:

- OvertimeCost: reads and writes the sum of a task's actual and remaining overtime cost (double).
- OvertimeWork: reads and writes the amount of overtime scheduled for a task (TimeSpan).

### **Microsoft Project view of task overtime**
To see a task's overtime work and cost properties:

1. In the Task Entry form, select the **Insert** menu and then **Column**.
2. Add the overtime columns.

### **Getting task overtimes in Aspose.Tasks**
The following code example demonstrates how to get the overtime cost and work associated with a task.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskOvertimes-ReadTaskOvertimes.cpp" >}}
