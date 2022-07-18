---
title: Working with Resource Properties
description: "Learn how to work with Microsoft Project (MPP/XML) resource properties using Aspose.Tasks for C++."
type: docs
weight: 20
url: /cpp/resource-properties/
---

{{% alert color="primary" %}}

The [Resource](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.resource) class has a number of properties for getting and setting resource attributes:

- Name gets and sets a resource's name (string).
- Id gets and sets a resource's ID (integer).
- Uid gets and sets a resource's UID (integer).
- Start gets and sets a resource's start date (DateTime).
- Finish gets and sets a resource's end date (DateTime).

{{% /alert %}}

## **Working with General Resource Properties**
To view a resource's general properties in Microsoft Project:

1. From the **View** menu, select **More Views** and then **Resource Sheet**.
2. From the **Insert** menu, select **Column**.
3. Add the Start, Finish, ID and unique ID columns.

### **Setting General Resource Properties using Aspose.Tasks**
The following code example demonstrates how to set general resource properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-SetGeneralResourceProperties-SetGeneralResourceProperties.cpp" >}}
