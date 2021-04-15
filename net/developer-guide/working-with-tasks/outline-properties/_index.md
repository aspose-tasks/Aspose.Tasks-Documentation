---
title: Outline Properties
description: "Learn how to work Microsoft Project (MPP/XML) outline values using Aspose.Tasks for .NET."
type: docs
weight: 100
url: /net/outline-properties/
---

Microsoft Project has an outline structure that lets users get a quick overview of a project. Aspose.Tasks for .NET supports this functionality and lets developers control the outline number - where the task appears in a hierarchy - and the outline level - which level of the hierarchy the task is in.

## **Working with Outline Properties**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes the [OutlineNumber](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/outlinenumber) and [OutlineLevel](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/outlinelevel) properties for managing outlines associated with a class:

1. OutlineNumber (string).
2. OutlineLevel (integer).

### **Outlines in Microsoft Project**
In Microsoft Project, outline number and outline level properties can be viewed on the Task Entry form by adding the columns:

1. On the **Insert** menu, select **columns**.
2. Add the OutlineNumber and OutlineLevel columns.

### **Getting Outline Properties in Aspose.Tasks**
The following example shows how to get the outline level and outline number information about a task using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskOutlineProperties.cs" >}}
