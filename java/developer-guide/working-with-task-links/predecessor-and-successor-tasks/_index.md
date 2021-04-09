---
title: Predecessor and Successor Tasks
description: "Learn how to work with Microsoft Project (MPP/XML) predecessor and successor tasks using Aspose.Tasks for Java."
type: docs
weight: 30
url: /java/predecessor-and-successor-tasks/
---

{{% alert color="primary" %}}

The PredTask and SuccTask properties exposed by the [TaskLink](https://apireference.aspose.com/tasks/java/com.aspose.tasks/TaskLink) class are used to define the predecessor and successor tasks for a TaskLink. Both of these properties read and write [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task) object.

{{% /alert %}}

## **Working with Predecessor and Successor Tasks**
To manage predecessor tasks in Microsoft Project:

1. From the **View** menu, select **More Views** and then **Task Entry Form**.
2. Double-click the desired task.# Select the Predecessor tab.

**Viewing predecessor tasks in Microsoft Project** 

![checking predecessor/successors tasks in Microsoft Project 2019](predecessor-and-successor-tasks_1.png)

### **Getting Predecessor Tasks with Aspose.Tasks**
The code sample below displays the predecessor and successor task after traversing the task links in the project and writing the results to a console window.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-TaskLinks-PredecessorSuccessorTasks-predecessor-successor-tasks.java" >}}
