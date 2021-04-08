---
title: Working with Task Costs
description: "Learn how to work with Microsoft Project (MPP/XML) task costs using Aspose.Tasks for C++."
type: docs
weight: 140
url: /cpp/task-costs/
---

To estimate the cost of a project, tasks are associated with costs. Aspose.Tasks for C++ API supports this feature of Microsoft Project with a range of properties.

## **Working with Task Cost**
The [Tsk](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.tsk) exposes a number of properties for working with task cost:

- Cost: a task's projected or scheduled cost (double).
- BCWP: the budgeted cost of the work performed to date (double).
- BCWS: the budgeted cost of scheduled work (double).
- FixedCost: the fixed cost associated with a task (single).
- FixedCostAccrual: the fixed cost accrued for a task (CostAccrualType).

### **Viewing Task Costs in Microsoft Project**
To view task costs in Microsoft Project:

1. On the Task Entry form, go to the **Insert** menu and select **Columns**.
2. Add the cost columns.

### **Getting Task Costs**
The following code example demonstrates how to get a task's cost.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskCosts-ReadTaskCosts.cpp" >}}
