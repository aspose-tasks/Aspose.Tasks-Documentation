---
title: Cross Project Predecessors
description: "Learn how to work with Microsoft Project (MPP/XML) cross project predecessors using Aspose.Tasks for .NET."
type: docs
weight: 40
url: /net/cross-project-predecessors/
---

Microsoft Project lets users link tasks within the current project, or to external projects. Cross project predecessors are predecessors from another project. Aspose.Tasks for .NET supports these too.

## **Working with Cross Project Predecessor Tasks**
In Aspose.Tasks for .NET the [CrossProjectName](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink/properties/crossprojectname) and [IsCrossProject](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink/properties/iscrossproject) properties exposed by the [TaskLink](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink) class are used to handle cross project predecessors.

- CrossProjectName represents the external predecessor project (string).
- IsCrossProject determines whether a predecessor is part of another project (Boolean).

To manage cross project predecessor tasks in Microsoft Project one can select **Links between Projects** from the **Tools** menu.

### **Getting cross project predecessor tasks using Aspose.Tasks**
Here, we shall display predecessor / successor task traversing the task links in the project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskLinks-GetCrossProjectTaskLinks-GetCrossProjectTaskLinks.cs" >}}
