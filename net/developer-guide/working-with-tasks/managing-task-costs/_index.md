---
title: Managing Task Costs
description: "Learn how to manage Microsoft Project (MPP/XML) task costs using Aspose.Tasks for .NET."
type: docs
weight: 140
url: /net/managing-task-costs/
---

To estimate the cost of a project, tasks are associated with costs. Aspose.Tasks for .NET supports this feature of Microsoft Project with a range of properties.

## **Working with Task Cost**
The [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) exposes a number of properties for working with task cost:

- [Cost](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/cost): a task's projected or scheduled cost (double).
- [BCWP](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/bcwp): the budgeted cost of the work performed to date (double).
- [BCWS](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/bcws): the budgeted cost of scheduled work (double).
- [FixedCost](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/fixedcost): the fixed cost associated with a task (single).
- [FixedCostAccrual](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/fixedcostaccrual): the fixed cost accrued for a task (CostAccrualType).

### **Viewing Task Costs in Microsoft Project**
To view task costs in Microsoft Project:

1. On the Task Entry form, go to the **Insert** menu and select **Columns**.
2. Add the cost columns.

### **Getting Task Costs**
The following examples show how to get a task's cost using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskCosts.cs" >}}
