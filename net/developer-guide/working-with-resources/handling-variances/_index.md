---
title: Handling Variances
description: "Learn how to add, edit or remove Microsoft Project (MPP/XML) work variances using Aspose.Tasks for .NET."
type: docs
weight: 120
url: /net/handling-variances/
---

A work variance is the difference between the estimated work (the baseline) and actual work performed.

## **Handling Variances**
The WorkVariance property exposed by the [Resource](https://reference.aspose.com/tasks/net/aspose.tasks/resource) class handles variance in work:

- WorkVariance: a project resource's difference from the baseline work (double).

### **Microsoft Project View of Resource Work Variance**
To see the resource work variance in Microsoft Project:

1. On the Resource Sheet, go to the **Insert** menu and select **Column**.
2. Add the Variance column.

### **Getting Resource Work Variance in Aspose.Tasks**
The following examples show how to get resource work variance using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-GetResourceWorkVariance.cs" >}}
