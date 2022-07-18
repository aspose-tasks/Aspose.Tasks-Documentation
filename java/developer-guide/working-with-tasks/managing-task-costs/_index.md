---
title: Managing Task Costs
description: "Learn how to manage Microsoft Project (MPP/XML) task costs using Aspose.Tasks for Java."
type: docs
weight: 140
url: /java/managing-task-costs/
---

To estimate the cost of a project, tasks are associated with costs. Aspose.Tasks for Java supports this feature of Microsoft Project with a range of properties.

## **Working with Task Cost**
The [Task](https://reference.aspose.com/tasks/java/com.aspose.tasks/Task/) class exposes several properties for working with task cost:

- COST: a task's projected or scheduled cost (double).
- BCWP: the budgeted cost of the work performed to date (double).
- BCWS: the budgeted cost of scheduled work (double).
- FIXED_COST: the fixed cost associated with a task (single).
- FIXED_COST_ACCRUAL: the fixed cost accrued for a task (CostAccrualType).

### **Viewing Task Costs in Microsoft Project**
To view task costs in Microsoft Project:

1. On the Task Entry form, go to the **Insert** menu and select **Columns**.
2. Add the cost columns.

**Task cost in Microsoft Project**

![edit task costs in Microsoft Project](managing-task-costs_1.png)

### **Getting Task Costs**
The following examples show how to get a task's cost using Aspose.Tasks.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-ManageTaskCost-manage-task-cost.java" >}}
