---
title: Percentage Complete Calculations
description: "Learn how to work with Microsoft Project (MPP/XML) percentage complete values using Aspose.Tasks for C++."
type: docs
weight: 170
url: /cpp/percentage-complete-calculations/
---

{{% alert color="primary" %}}

Microsoft Project shows the percentage of a task that's been completed. The percentage can be added manually, by a project manager, or automatically calculated by the application. Aspose.Tasks for C++ supports several percentage calculations related to tasks.

{{% /alert %}}

## **Percentages**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes a number of properties used to calculate percentages:

- PercentComplete represents the completed percentage of a task's duration (integer).
- PercentWorkComplete represents the completed percentage of a task's work (integer).
- PhysicalPercentComplete represents the completed percentage as entered by a project manager (integer).

To see the physical percentage complete in Microsoft Project:

1. On the Task Entry form, from the **Insert** menu, select **Column**.
2. Add the column.

To see the completed percentage in Microsoft Project:

1. On the Task Entry form, double-click the desired column.

### **Getting Percentages**
The following code example demonstrates how to get the percentages of work relating to tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskPercentageCompletion-ReadTaskPercentageCompletion.cpp" >}}

## **Changing Task Progress**
Aspose.Tasks for C++ API supports changing a task's progress in terms of its percentage completion through the [Task](https://apireference.aspose.com/tasks/net/aspose.tasks/task) class' SetPercentComplete() method. This method takes an integer argument as input for the percentage work completed.

The following piece of code shows how to change the progress of a task.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ChangeTaskProgress-ChangeTaskProgress.cpp" >}}
