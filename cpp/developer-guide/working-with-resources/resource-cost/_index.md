---
title: Working with Resource Costs
description: "Learn how to work with Microsoft Project (MPP/XML) resource works using Aspose.Tasks for C++."
type: docs
weight: 50
url: /cpp/resource-cost/
---

{{% alert color="primary" %}}

The [Resource](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.resource) class is used to manage costs related to a resource:

- Cost represents a resource's total project cost across all assignments (decimal).
- BCWP represents the budgeted cost of work performed by a resource (double).
- BCWS represents the budgeted cost of scheduled work (doubled).
- ACWP represents the actual cost of work performed by a resource to date (double).
- AccrueAt represents the cost accrual method used for a resource (CostAccrualType).

{{% /alert %}}

## **Working with Resource Costs**
To view resource costs in Microsoft Project:

1. On the Resource sheet, from the **Insert** menu, select **Column**.
2. Add the columns.

### **Getting Resource Costs in Aspose.Tasks**
The following code example demonstrates how to get task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-GetResourceCosts-GetResourceCosts.cpp" >}}
