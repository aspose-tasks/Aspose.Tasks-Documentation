---
title: Managing Task Costs
type: docs
weight: 140
url: /net/managing-task-costs/
---

{{% alert color="primary" %}} 

To estimate the cost of a project, tasks are associated with costs. Aspose.Tasks supports this feature of Microsoft Project with a range of properties.

{{% /alert %}} 
## **Working with Task Cost**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) exposes a number of properties for working with task cost:

- [Cost](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/cost): a task's projected or scheduled cost (double).
- [BCWP](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/bcwp): the budgeted cost of the work performed to date (double).
- [BCWS](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/bcws): the budgeted cost of scheduled work (double).
- [FixedCost](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/fixedcost): the fixed cost associated with a task (single).
- [FixedCostAccrual](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/fixedcostaccrual): the fixed cost accrued for a task (CostAccrualType).
### **Viewing Task Costs in Microsoft Project**
To view task costs in Microsoft Project:

1. On the Task Entry form, go to the **Insert** menu and select **Columns**.
2. Add the cost columns.
### **Getting Task Costs**
The following examples show how to get a task's cost using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskCosts-ReadTaskCosts.cs" >}}
