---
title: Parent and Child Tasks
type: docs
weight: 150
url: /cpp/parent-and-child-tasks/
---

{{% alert color="primary" %}} 

Tasks can be organized in a hierarchy. When a task has one or more tasks beneath it, they are referred to as parents. The tasks underneath are called children.

{{% /alert %}} 
## **Working with Parent Tasks and Children**
The [Task ](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.task/)class exposes classes that help you determine a:

- Parent: determines that a task is a parent task. Accepts and returns a Task object.
- Children: determines that a task is a child task. Accepts and returns an array list of Task objects.
### **Parent and Child Tasks in Microsoft Project**
To declare a task as a parent or a child task in Microsoft Project:

1. In the Task Entry form, select a task and click it.
2. Select **Outdent** to turn a task into a parent, or,
3. Select **Indent** to turn a task into a child.
### **Getting Parent and Child Tasks**
The following examples show viewing parent and child tasks in a project using Aspose.Tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadParentChildTasks-ReadParentChildTasks.cpp" >}}
