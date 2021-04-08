---
title: WBS Associated with a Task
description: "Learn how to work with Microsoft Project (MPP/XML) task WBS values using Aspose.Tasks for .NET."
type: docs
weight: 130
url: /net/wbs-associated-with-a-task/
---

WBS (Work Breakdown Structure) codes, lets you assign outline numbers to tasks according to the needs of your business. It's a method for applying a customized outline scheme to a project. Aspose.Tasks for .NET supports this feature.

## **Working with Work Breakdown Structure**
The [WBS](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/wbs) and [WBSLevel](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/wbslevel) properties exposed by the [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class are used to read and write a tasks work breakdown structure.

### **Microsoft Project View of WBS**
To view WBS information in Microsoft Project:

1. On the Task Entry Form, select the **Insert** menu and then **Column**.
2. Add the WBS column.

### **Getting WBS in Aspose.Tasks**
The following examples show how to get a task's WBS value using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskWBS-ReadTaskWBS.cs" >}}

### **Adding WBS Code Definitions in Aspose.Tasks**
Aspose.Tasks for .NET allows adding WBS code definition for tasks to a project same as Microsoft Project.WBSCodeDefinition class exposes various properties that can be used to generate desired WBS codes in a project. The following code sample demonstrates setting up WBS code definitions in a project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-AddWBSCodes-AddWBSCodes.cs" >}}

## **Renumber WBS Codes**
Aspose.Tasks for .NET API is able to renumber WBS codes similar to MSP's "Renumber" function.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-RenumberTaskWBSCodes-RenumberTaskWBSCodes.cs" >}}
