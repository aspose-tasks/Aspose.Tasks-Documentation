---
title: Managing Assignment Cost
description: "Learn how to manage Microsoft Project (MPP/XML) resource assignment costs using Aspose.Tasks for .NET."
type: docs
weight: 30
url: /net/managing-assignment-cost/
---

## **Managing Assignment Cost**
The [ResourceAssignment](https://apireference.aspose.com/tasks/net/aspose.tasks/resourceassignment) class exposes several properties used to manage assignment cost:

- Cost represents an assignment's total project cost (decimal).
- BCWP represents the budgeted cost of work to date on an assignment (double).
- BCWS represents the budgeted cost of work scheduled for an assignment (double).
- ACWP represents the actual cost of the work carried out on an assignment to date (double).

To view assignment costs in Microsoft Project:

1. On the Task Usage page, select the **Insert** menu and then **Column**.
2. Add the columns.

### **Getting Assignment Costs with Aspose.Tasks**
The following example shows getting task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-GetResourceAssignmentCosts-GetResourceAssignmentCosts.cs" >}}
