---
title: Defining Link Type
description: "Learn how to change Microsoft Project (MPP/XML) task link types using Aspose.Tasks for C++."
type: docs
weight: 20
url: /cpp/defining-link-type/
---

{{% alert color="primary" %}} 

The LinkType property exposed by the TaskLink class is used to retrieve or define the type of link between two tasks. It reads and writes one of the values defined by the TaskLinkType enumeration type.

{{% /alert %}}

## **Defining Link Type**
To define link type in Microsoft Project:
On the **View** menu, select **More Views** and then **Task Entry Form**.

1. Double-click the desired task.
2. Select the **Predecessor** tab.

**Defining link type in Microsoft Project** 

![editing task link type in Microsoft Project](defining-link-type_1.png)

### **Setting Link Type with Aspose.Tasks**
The code sample given below set a link type as "Start-to-Start”, the default link type is "Finish-to-Start”.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTaskLinks-SetTaskLinkType-SetTaskLinkType.cpp" >}}

### **Getting Link Type with Aspose.Tasks**
The code sample given below display link types by traversing the task links in the project and printing the result to a console window.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTaskLinks-GetTaskLinkType-GetTaskLinkType.cpp" >}}
