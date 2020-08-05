---
title: Resource Cost
type: docs
weight: 50
url: /net/resource-cost/
---

{{% alert color="primary" %}} 

The [Resource]() class is used to manage costs related to a resource:

- Cost represents a resource's total project cost across all assignments (decimal).
- Bcwp represents the budgeted cost of work performed by a resource (double).
- Bcws represents the budgeted cost of scheduled work (doubled).
- Acwp represents the actual cost of work performed by a resource to date (double).
- AccrueAt represents the cost accrual method used for a resource (CostAccrualType).

{{% /alert %}} 
## **Working with Resource Costs**
To view resource costs in Microsoft Project:

1. On the Resource sheet, from the **Insert** menu, select **Column**.
1. Add the columns.
### **Getting Resource Costs in Aspose.Tasks**
The following example shows how to get task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-GetResourceCosts-GetResourceCosts.cs" >}}
