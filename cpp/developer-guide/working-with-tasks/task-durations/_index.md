---
title: Working With Task Durations
description: "Learn how to work with Microsoft Project (MPP/XML) task durations using Aspose.Tasks for C++."
type: docs
weight: 50
url: /cpp/task-durations/
---

{{% alert color="primary" %}}

Tasks take time, they have a duration. Realistic task durations help give a realistic project end date. Aspose.Tasks for C++ API allows developers to set task durations in projects.

{{% /alert %}}

## **Working with Durations**
The Duration and DurationFormat properties exposed by the [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class are used to determine the planned duration and format of the duration of a task:

- Duration sets and gets a task's planned duration (TimeSpan).
- DurationFormat sets and gets formats defined by the TimeUnitType enumeration.

### **Duration in Microsoft Project**
To see a task's duration in Microsoft Project one can select **More Views** and then **Task Entry** from the **View** menu.

### **Setting task duration using Aspose.Tasks**
The code example given below demonstrates how to increase and decrease the task duration to 1 week and half week respectively.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-WriteTaskDuration-WriteTaskDuration.cpp" >}}

## **Calculating Durations**
It can be useful to calculate the duration of a task in different units such as minutes, hours, etc.

The [Tsk](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.tsk) class provides the Duration property for accessing task duration, which returns the Duration class object. The Convert method exposed as part of Duration class can then be used to calculate task durations in different units. This method takes TimeUnitType as the input argument and returns the duration as a double value.

The following code example demonstrates how to use this method to retrieve a task's duration in different units: minute, day, hour, week and month.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-CalculateTaskDurations-CalculateTaskDurations.cpp" >}}
