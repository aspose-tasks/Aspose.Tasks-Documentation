---
title: General Resource Assignment Properties
type: docs
weight: 20
url: /cpp/general-resource-assignment-properties/
---

{{% alert color="primary" %}} 

An assignment is a resource that has been assigned to a specific task. Each resource has general properties, typically a unique ID, a start and a finish time. This article explains how to set and get these properties with Aspose.Tasks.

{{% /alert %}} 
## **Working with General Assignment Properties**
The [ResourceAssignment ](https://apireference.aspose.com/cpp/tasks/class/aspose.tasks.resource_assignment/)class exposes a number of properties used to set and get general assignment properties:

- Uid sets and gets an assignment's unique ID (integer).
- Start sets and gets an assignment's start date (DateTime).
- Finish sets and gets an assignment's end date (DateTime).

To see an assignment's general properties in Microsoft Project:

1. From the **View** menu, select **Task Usage**.
2. From the **Insert** menu, select **Column**.
3. Add the Start. Finish and Unique ID columns.
### **Setting General Resource Assignment Properties using Aspose.Tasks**
The following code example demonstrates how to set these properties from scratch.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-SetGeneralResourceAssignmentProperties-SetGeneralResourceAssignmentProperties.cpp" >}}
### **Getting General Resource Assignment Properties using Aspose.Tasks**
The resource assignment properties can be accessed by traversing the project's ResourceAssignments property.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResourceAssignments-GetGeneralResourceAssignmentProperties-GetGeneralResourceAssignmentProperties.cpp" >}}
