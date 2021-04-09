---
title: Creating Tasks
description: "Learn how to create Microsoft Project (MPP/XML) tasks using Aspose.Tasks for C++."
type: docs
weight: 10
url: /cpp/creating-tasks/
---

{{% alert color="primary" %}}

A project is, essentially, made up by a number of tasks, each of which has to be completed for the project to be completed. When working with project files, adding tasks is an important activity. Tasks are often linked to other tasks, to indicate dependency, and typically have a set duration. Aspose.Tasks for C++ API allows developers to create tasks and define name, children and duration at the time of creation.

{{% /alert %}}

## **Creating Tasks**
The Task class exposes the Add method for adding a task to a project's root or other tasks. The following code example demonstrates how to create a task.

The default constructor creates a Task instance without any parameter being passed.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-CreateTasks-CreateTasks.cpp" >}}
