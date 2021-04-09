---
title: General Resource Assignment Properties
description: "Learn how to read or edit properties of Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks for Java."
type: docs
weight: 20
url: /java/general-resource-assignment-properties/
---

{{% alert color="primary" %}}

An assignment is a resource that has been assigned to a specific task. Each resource has general properties, typically a unique ID, a start and a finish time. This article explains how to set and get these properties with Aspose.Tasks.

{{% /alert %}}

## **Working with General Assignment Properties**
The [ResourceAssignment](https://apireference.aspose.com/tasks/java/com.aspose.tasks/ResourceAssignment) class exposes a number of properties used to set and get general assignment properties:

- Uid sets and gets an assignment's unique ID (integer).
- Start sets and gets an assignment's start date (java.util.Date).
- Finish sets and gets an assignment's end date (java.util.Date).

To see an assignment's general properties in Microsoft Project:
1. From the **View** menu, select **Task Usage**.
2. From the **Insert** menu, select **Column**.
3. Add the Start. Finish and Unique ID columns.

**General assignment properties viewed in Microsoft Project**

![open resource assignment properties in Microsoft Project](general-resource-assignment-properties_1.png)

### **Setting General Resource Assignment Properties using Aspose.Tasks**
The following example shows how to set these properties from scratch.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-ResourceAssignments-ResourceAssignmentProperties-setting-resource-assignment-properties.java" >}}

### **Getting General Resource Assignment Properties using Aspose.Tasks**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-ResourceAssignments-ResourceAssignmentProperties-getting-resource-assignment-properties.java" >}}
