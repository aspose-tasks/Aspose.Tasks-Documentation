---
title: Managing Assignment Cost
description: "Learn how to manage Microsoft Project (MPP/XML) resource assignment costs using Aspose.Tasks for Java."
type: docs
weight: 30
url: /java/managing-assignment-cost/
---

## **Managing Assignment Cost**
The [ResourceAssignment](https://reference.aspose.com/tasks/java/com.aspose.tasks/ResourceAssignment) class exposes several properties used to manage assignment cost:

- Cost represents an assignment's total project cost (decimal).
- BCWP represents the budgeted cost of work to date on an assignment (double).
- BCWS represents the budgeted cost of work scheduled for an assignment (double).
- ACWP represents the actual cost of the work carried out on an assignment to date (double).

To view assignment costs in Microsoft Project:

1. On the Task Usage page, select the **Insert** menu and then **Column**.
2. Add columns.

**Resource cost columns in Microsoft Project**

![modify resource costs in Microsoft Project 2010](managing-assignment-cost_1.png)

### **Getting Assignment Costs with Aspose.Tasks**
The following example shows getting task costs using Aspose.Tasks.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-ResourceAssignments-AssignmentCost-managing-assignment-cost.java" >}}
