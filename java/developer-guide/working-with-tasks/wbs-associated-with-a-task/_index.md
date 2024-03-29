---
title: WBS Associated with a Task
description: "Learn how to work with Microsoft Project (MPP/XML) task WBS values using Aspose.Tasks for Java."
type: docs
weight: 130
url: /java/wbs-associated-with-a-task/
---

{{% alert color="primary" %}}

WBS codes, work breakdown structure codes, lets you assign outline numbers to tasks according to the needs of your business. It's a method for applying a customized outline scheme to a project. Aspose.Tasks for Java supports this feature.

{{% /alert %}}

## **Working with Work Breakdown Structure**
The WBS and WBSLevel properties exposed by the [Tsk](https://reference.aspose.com/tasks/java/com.aspose.tasks/Tsk/) class is used to read and write a tasks work breakdown structure:

- WBS: sets or gets a task's WBS code (string).
- WBS_LEVEL: sets or gets a task's WBS level (string).

### **Microsoft Project View of WBS**
To view WBS information in Microsoft Project:

1. On the Task Entry Form, select the **Insert** menu and then **Column**.
2. Add the WBS column.

**Work breakdown structure in Microsoft Project**

![WBS associated with tasks](wbs-associated-with-a-task_1.png)

### **Getting WBS in Aspose.Tasks**
The following examples show how to get a task's WBS value using Aspose.Tasks.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-WbsAssociatedWithTask-wbs-association.java" >}}

## **Renumber WBS Codes**
Aspose.Tasks for Java API can renumber WBS codes similar to MSP's "Renumber" function.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-WbsAssociatedWithTask-RenumberTaskWBSCodes.java" >}}
