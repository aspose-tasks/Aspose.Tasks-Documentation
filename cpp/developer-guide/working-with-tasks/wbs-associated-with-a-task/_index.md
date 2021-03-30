---
title: WBS Associated with a Task
type: docs
weight: 130
url: /cpp/wbs-associated-with-a-task/
---

{{% alert color="primary" %}} 

WBS (Work Breakdown Structure) codes, lets you assign outline numbers to tasks according to the needs of your business. It's a method for applying a customized outline scheme to a project. Aspose.Tasks API supports this feature.

{{% /alert %}} 
## **Working with Work Breakdown Structure**
The WBS and WBSLevel properties exposed by the [Tsk](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.tsk/) class are used to read and write a tasks work breakdown structure.
### **Microsoft Project View of WBS**
To view WBS information in Microsoft Project:

1. On the Task Entry Form, select the **Insert** menu and then **Column**.
2. Add the WBS column.
### **Getting WBS in Aspose.Tasks**
The following examples show how to get a task's WBS value using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskWBS-ReadTaskWBS.cpp" >}}
### **Adding WBS Code Definitions**
Aspose.Tasks API allows adding WBS code definition for tasks to a project same as Microsoft Project.WBSCodeDefinition class exposes various properties that can be used to generate desired WBS codes in a project. The following code sample demonstrates setting up WBS code definitions in a project.



{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-AddWBSCodes-AddWBSCodes.cpp" >}}
## **Renumber WBS codes**
Aspose.Tasks API is able to renumber WBS codes similar to MSP's "Renumber" function.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-RenumberTaskWBSCodes-RenumberTaskWBSCodes.cpp" >}}
