---
title: Resource Work Variances
description: "Learn how to use Aspose.Tasks for C++ to manage resource work variances in Microsoft Project (MPP/XML) files."
type: docs
weight: 120
url: /cpp/resource-work-variances/
---

Work variance is the difference between the estimated work (the baseline) and actual work performed.

## **Handling Variances**
The WorkVariance property exposed by the Resource class handles variance in work:

- WorkVariance: a project resource's difference from the baseline work (double).

### **Microsoft Project View of Resource Work Variance**
To see the resource work variance in Microsoft Project:

1. On the Resource Sheet, go to the **Insert** menu and select **Column**.
2. Add the Variance column.

### **Getting Resource Work Variance in Aspose.Tasks**
The following code example demonstrated how to get resource work variance using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-GetResourceWorkVariance-GetResourceWorkVariance.cpp" >}}
