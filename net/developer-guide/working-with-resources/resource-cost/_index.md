---
title: Managing Resource Costs
description: "Learn how to get Microsoft Project (MPP/XML) resource cost fields using Aspose.Tasks for .NET."
type: docs
weight: 50
url: /net/resource-cost/
---

The [Resource](https://apireference.aspose.com/tasks/net/aspose.tasks/resource) class is used to manage costs related to a resource:

- Cost represents a resource's total project cost across all assignments (decimal).
- BCWP represents the budgeted cost of work performed by a resource (double).
- BCWS represents the budgeted cost of scheduled work (doubled).
- ACWP represents the actual cost of work performed by a resource to date (double).
- AccrueAt represents the cost accrual method used for a resource (CostAccrualType).

## **Working with Resource Costs**
To view resource costs in Microsoft Project:

1. On the Resource sheet, from the **Insert** menu, select **Column**.
2. Add the columns.

### **Getting Resource Costs in Aspose.Tasks**
The following example shows how to get task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-GetResourceCosts.cs" >}}
