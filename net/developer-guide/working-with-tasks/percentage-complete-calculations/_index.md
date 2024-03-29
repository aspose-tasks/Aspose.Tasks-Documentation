---
title: Percentage Complete Calculations
description: "Learn how to work with Microsoft Project (MPP/XML) percentage complete values using Aspose.Tasks for .NET."
type: docs
weight: 180
url: /net/percentage-complete-calculations/
---

Microsoft Project shows the percentage of a task that's been completed. The percentage can be added manually, by a project manager, or automatically calculated by the application. Aspose.Tasks for .NET supports several percentage calculations related to tasks.

## **Percentages**
The [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes a number of properties used to calculate percentages:

- [PercentComplete](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/percentcomplete) represents the completed percentage of a task's duration (integer).
- [PercentWorkComplete](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/percentworkcomplete) represents the completed percentage of a task's work (integer).
- [PhysicalPercentComplete](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/physicalpercentcomplete) represents the completed percentage as entered by a project manager (integer).

To see the physical percent complete in Microsoft Project:

1. On the Task Entry form, from the **Insert** menu, select **Column**.
2. Add the column.

To see the completed percentage in Microsoft Project one can double-click the desired column in the Task Entry form.

### **Getting Percentages in Aspose.Tasks**
The following example shows how to get the percentages of work relating to tasks using Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskPercentageCompletion.cs" >}}
