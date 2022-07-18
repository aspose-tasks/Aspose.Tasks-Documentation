---
title: Assignment Overtime and Remaining Costs
description: "The page describes how to work with Microsoft Project (MPP/XML) resource assignment overtimes and remaining costs using Aspose.Tasks for C++."
type: docs
weight: 50
url: /cpp/assignment-overtime-and-remaining-costs/
---

## **Handling Overtime, Remaining Costs and Work**
The [Asn](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.asn) class exposes a number of properties for handling an assignment's overtime, remaining costs and work:

- OvertimeCost represents the sum of the actual and remaining overtime costs of an assignment (decimal).
- OvertimeWork represents the scheduled overtime work for an assignment (TimeSpan).
- RemainingCost represents the remaining projected cost for completing an assignment (decimal).
- RemainingOvertimeCost represents the remaining projected overtime cost for completing an assignment (decimal).
- RemainingWork represents the scheduled remaining work for an assignment (TimeSpan).
- RemainingOvertimeWork represents the scheduled remaining overtime work for an assignment (TimeSpan).

To see assignment overtime, remaining cost and work in Microsoft Project:

1. On the Task Usage screen, select the **Insert** menu, then **Column**.
2. Add the desired columns.

### **Getting Assignment Overtimes in Aspose.Tasks**
The following code example demonstrates how to get assignment overtimes, remaining costs and work using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-GetResourceAssignmentOvertimes-GetResourceAssignmentOvertimes.cpp" >}}

## **Work Completion Percentage**
The PercentWorkComplete property exposed by the [Asn](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.asn) class is used to manage the percentage of work completed on an assignment.

- PercentWorkComplete represents the percentage of the completed work on an assignment (integer).

The following example shows how to get the percentage of work completed on an assignment using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-GetResourceAssignmentPercentWorkComplete-GetResourceAssignmentPercentWorkComplete.cpp" >}}
