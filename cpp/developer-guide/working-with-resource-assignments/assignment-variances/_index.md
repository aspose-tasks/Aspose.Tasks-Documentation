---
title: Working With Assignment Variances
description: "Learn how to work with Microsoft Project (MPP/XML) resource assignment variances using Aspose.Tasks for C++."
type: docs
weight: 60
url: /cpp/assignment-variances/
---

## **Dealing Variances**
The [Asn](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.asn) class exposes several properties for handling variance in an assignment's baseline values and the actual cost, start date, finish date and work:

- CostVariance handles the variance in cost against an assignment's baseline (double).
- StartVariance handles the variance in start date against an assignments baseline (integer).
- FinishVariance handles the variance in end date against an assignments baseline (integer).
- WorkVariance handles the variance in work against an assignment's baseline (double).

To see resource assignment variances in Microsoft Project:

1. On the Task Usage screen, select **Insert** and ten **Columns**.
2. Add the desired columns.

### **Getting Assignment Variance in Aspose.Tasks**
The following code example demonstrates how to get the resource work variance using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-GetResourceAssignmentVariance-GetResourceAssignmentVariance.cpp" >}}
