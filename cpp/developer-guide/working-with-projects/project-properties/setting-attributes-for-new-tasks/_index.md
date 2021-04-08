---
title: Setting Attributes for New Tasks
description: "Learn how to set Microsoft Project (MPP/XML) project attributes for newly created tasks using Aspose.Tasks for C++."
type: docs
weight: 60
url: /cpp/setting-attributes-for-new-tasks/
---

## **Setting Attributes for New Tasks**
Microsoft Project allows setting default properties for new tasks added. This topic explains how to set the default start date for new tasks using Aspose.Tasks for C++ API.

The [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) class exposes the [NewTaskStartDate](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a206158d8e6e22155f3b987f4ba86378e) property that defines the start date for a new task. This property supports the values defined by the [TaskStartDateType](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a206158d8e6e22155f3b987f4ba86378e) enumeration type.

To see the task attribute:

1. Open the file with Microsoft Project.
2. On the **Tools** menu, select **Options**.
3. Select the **Schedule** tab.

The tab looks like the one shown below.

**New tasks set to start on the current date** 

![edit task's schedule options in Microsoft Project](working-with-project-properties_6.png)

The code example given below demonstrates how to set the new task start date.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-SetAttributesForNewTasks-SetAttributesForNewTasks.cpp" >}}
