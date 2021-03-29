---
title: Outline Properties
type: docs
weight: 100
url: /cpp/outline-properties/
---

{{% alert color="primary" %}} 

Microsoft Project has an outline structure that let users get a quick overview of a project. Aspose.Tasks API supports this functionality and lets developers control the outline number - where the task appears in a hierarchy - and the outline level - which level of the hierarchy the task is in.

{{% /alert %}} 
## **Working with Outline Properties**
The Tsk class exposes the OutlineNumber and OutlineLevel properties for managing outlines associated with a class:

1. OutlineNumber (string).
2. OutlineLevel (integer).
### **Outlines in Microsoft Project**
In Microsoft Project, outline number and outline level properties can be viewed on the Task Entry form by adding the columns:

1. On the **Insert** menu, select **columns**.
2. Add the OutlineNumber and OutlineLevel columns.
### **Getting Outline Properties in Aspose.Tasks**
The following example shows how to get the outline level and outline number information about a task using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskOutlineProperties-ReadTaskOutlineProperties.cpp" >}}
