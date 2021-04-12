---
title: Cross Project Predecessors
description: "Learn how to work with Microsoft Project (MPP/XML) cross project predecessors using Aspose.Tasks for C++."
type: docs
weight: 40
url: /cpp/cross-project-predecessors/
---

Microsoft Project lets users link tasks within the current project, or to external projects. Cross project predecessors are predecessors from another project. Aspose.Tasks for C++ API supports these too.

## **Working with Cross Project Predecessor Tasks**
In Aspose.Tasks for C++ the CrossProjectName and IsCrossProject properties exposed by the TaskLink class are used to handle cross project predecessors.

- CrossProjectName represents the external predecessor project (string).
- IsCrossProject determines whether a predecessor is part of another project (Boolean).

To manage cross project predecessor tasks in Microsoft Project one can select **Links between Projects** from the **Tools** menu.

### **Getting cross project predecessor tasks using Aspose.Tasks**
The code example given below demonstrates the predecessor/ successor task traversing the task links in the project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTaskLinks-GetCrossProjectTaskLinks-GetCrossProjectTaskLinks.cpp" >}}
