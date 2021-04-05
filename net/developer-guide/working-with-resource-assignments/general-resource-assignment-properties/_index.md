---
title: General Resource Assignment Properties
type: docs
weight: 20
url: /net/general-resource-assignment-properties/
---

{{% alert color="primary" %}} 

An assignment is a resource that has been assigned to a specific task. Each resource has general properties, typically a unique ID, a start and a finish time. This article explains how to set and get these properties with Aspose.Tasks.

{{% /alert %}} 
## **Working with General Assignment Properties**
The [ResourceAssignment](https://apireference.aspose.com/tasks/net/aspose.tasks/resourceassignment) class exposes a number of properties used to set and get general assignment properties:

- Uid sets and gets an assignment's unique ID (integer).
- Start sets and gets an assignment's start date (DateTime).
- Finish sets and gets an assignment's end date (DateTime).

To see an assignment's general properties in Microsoft Project:

1. From the **View** menu, select **Task Usage**.
2. From the **Insert** menu, select **Column**.
3. Add the Start. Finish and Unique ID columns.
### **Setting General Resource Assignment Properties using Aspose.Tasks**
The following example shows how to set these properties from scratch.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-SetGeneralResourceAssignmentProperties-SetGeneralResourceAssignmentProperties.cs" >}}
### **Getting General Resource Assignment Properties using Aspose.Tasks**
The resource assignment properties can be accessed by traversing the project's ResourceAssignments property.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-GetGeneralResourceAssignmentProperties-GetGeneralResourceAssignmentProperties.cs" >}}
