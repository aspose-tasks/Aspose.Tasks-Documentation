---
title: Managing Assignment Cost
description: "Learn how to manage Microsoft Project (MPP/XML) resource assignment costs using Aspose.Tasks for C++."
type: docs
weight: 30
url: /cpp/managing-assignment-cost/
---

## **Managing Assignment Cost**
The [ResourceAssignment](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.resource_assignment) class exposes several properties used to manage assignment cost:

- Cost represents an assignment's total project cost (decimal).
- BCWP represents the budgeted cost of work to date on an assignment (double).
- BCWS represents the budgeted cost of work scheduled for an assignment (double).
- ACWP represents the actual cost of the work carried out on an assignment to date (double).

To view assignment costs in Microsoft Project:

1. On the Task Usage page, select the **Insert** menu and then **Column**.
2. Add columns.

### **Getting Assignment Costs with Aspose.Tasks**
The following code example demonstrates how to get task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-GetResourceAssignmentCosts-GetResourceAssignmentCosts.cpp" >}}
