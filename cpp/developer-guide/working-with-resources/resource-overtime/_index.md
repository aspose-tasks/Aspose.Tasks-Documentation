---
title: Working with Resource Overtimes
description: "Learn how to work with Microsoft Project (MPP/XML) resource overtimes using Aspose.Tasks for C++."
type: docs
weight: 40
url: /cpp/resource-overtime/
---

{{% alert color="primary" %}}

The [Resource](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.resource) class exposes a number of properties for managing resource overtime:

- Overtime represents the overtime rate (decimal).
- OvertimeRate represents the overtime rate from the current date, if a rate table exists for the resource (decimal).
- OvertimeRateFormat represents the units used for the overtime rate (RateFormatType).
- OvertimeCost represents the sum of an actual and remaining overtime cost (decimal).
- OvertimeWork represents the amount of overtime work scheduled for tasks (TimeSpan).

{{% /alert %}}

## **Working with Resource Overtimes**
To see overtime cost, overtime rate and overtime work in Microsoft Project:

1. On the Resource sheet, select the **Insert** menu, and then select **Column**.
2. Add the columns.

### **Getting Resource Overtimes in Aspose.Tasks**
The following code example demonstrates how to get resource overtimes using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-GetResourceOvertime-GetResourceOvertime.cpp" >}}
