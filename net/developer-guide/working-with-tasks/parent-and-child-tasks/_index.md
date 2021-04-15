---
title: Parent and Child Tasks
description: "Learn how to work with Microsoft Project (MPP/XML) parent-child relations using Aspose.Tasks for .NET."
type: docs
weight: 150
url: /net/parent-and-child-tasks/
---

Tasks can be organized in a hierarchy. When a task has one or more tasks beneath it, they are referred to as parents. The tasks underneath are called children.

## **Working with Parent Tasks and Children**
The [Task](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes classes that help you determine a

- Parent: determines that a task is a parent task. Accepts and returns a Task object.
- Children: determines that a task is a child task. Accepts and returns an array list of Task objects.

### **Parent and Child Tasks in Microsoft Project**
To declare a task as a parent or a child task in Microsoft Project:

1. In the Task Entry form, select a task and click it.
2. Select **Outdent** to turn a task into a parent, or,
3. Select **Indent** to turn a task into a child.

### **Getting Parent and Child Tasks**
The following examples show viewing parent and child tasks in a project using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadParentChildTasks.cs" >}}
