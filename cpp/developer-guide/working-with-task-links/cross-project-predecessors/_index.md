---
title: Cross Project Predecessors
type: docs
weight: 40
url: /cpp/cross-project-predecessors/
---

{{% alert color="primary" %}} 

Microsoft Project lets users link tasks within the current project, or to external projects. Cross project predecessors are predecessors from another project. Aspose.Tasks API supports these too.

{{% /alert %}} 
## **Working with Cross Project Predecessor Tasks**
In Aspose.Tasks, the CrossProjectName and IsCrossProject properties exposed by the TaskLink class are used to handle cross project predecessors.

- CrossProjectName represents the external predecessor project (string).
- IsCrossProject determines whether a predecessor is part of another project (Boolean).

To manage cross project predecessor tasks in Microsoft Project:

1. From the **Tools** menu, select **Links between Projects**.
### **Getting cross project predecessor tasks using Aspose.Tasks**
The code example given below demonstrates the predecessor/ successor task traversing the task links in the project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTaskLinks-GetCrossProjectTaskLinks-GetCrossProjectTaskLinks.cpp" >}}
