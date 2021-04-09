---
title: Default Project Properties
description: "Learn how to work with default project properties of Microsoft Project (MPP/XML) projects using Aspose.Tasks for C++."
type: docs
weight: 10
url: /cpp/default-project-properties/
---

## **Default Project Properties**
Microsoft Project lets users set default project properties that speed up the process of setting up a project. The default properties define when a new task starts and finishes, sets the default overtime and standard pay rates and more. Aspose.Tasks for C++ supports these features.

The [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) exposes a number of properties for managing a project's default properties:

- [DefaultStartTime](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a1e88187695eadca5c8fa31664f34ca01): a new tasks' default start time, takes a DateTime value.
- [DefaultFinishTime](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a47199d6e2538eda4b481c514fa936b94): a new tasks' default finishing time, takes a DateTime value.
- [DefaultFixedCostAccrual](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#ab3603049689a8040d60aa0d3c47fc5f6): an assignment's default fixed cost accrual, takes one of the values defined by the [CostAccrualType]() enumeration.
- [DefaultStandardRate](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#ac4b528e39b563eecaabd35e59a338074): the default standard pay rate, takes a double.
- [DefaultOvertimeRate](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a99b4429ac923c9db80a9959758caf635): the default overtime pay rate, takes a double.
- [DefaultTaskEVMethod](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#ac677f43d27527f02af79242b17bc7148): the default task earned value method, takes one of the values defined by the [EarnedValueMethodType]() enumeration.
- [DefaultTaskType](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a9d1f6f82c34b1fe3aafee983b0132061): the project's default task type, takes one of the values defined by the [TaskType]() enumeration.

To see the default project information in Microsoft Project:

1. Open a project.
2. On the **Tools** menu, click **Options**.
3. Go to the **General** tab.
   Here, you can see the settings for the default standard and overtime rates.
4. Go to the **Schedule** tab.
   Here, you can see the settings for the default task type and default task start time.

**Default project information in Microsoft Project, as written by Aspose.Tasks**

![show default project properties in Microsoft Project](working-with-project-properties_2.png)

### **Reading Default Properties**
The code example given below demonstrates how to read a project's default properties and writes them to a console window.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-ReadDefaultProperties-DefaultProperties.cpp" >}}

### **Writing Default Properties**
The code example given below demonstrates how to set a project's default properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-WriteDefaultProperties-WriteDefaultProperties.cpp" >}}
