---
title: Dealing Variances
type: docs
weight: 70
url: /net/dealing-variances/
---

## **Dealing Variances**
The [Asn]() class exposes several properties for handling variance in an assignment's baseline values and the actual cost, start date, finish data and work:

- CostVariance handles the variance in cost against an assignment's baseline (double).
- StartVariance handles the variance in start date against an assignments baseline (integer).
- FinishVariance handles the variance in end date against an assignments baseline (integer).
- WorkVariance handles the variance in work against an assignment's baseline (double).

To see resource assignment variances in Microsoft Project:

1. On the Task Usage screen, select **Insert** and ten **Columns**.
1. Add the desired columns.
### **Getting Assignment Variance in Aspose.Tasks**
The following example shows how to get the resource work variance using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-GetResourceAssignmentVariance-GetResourceAssignmentVariance.cs" >}}
