---
title: Calculate Task Duration in Different Units
description: "Learn how to calculate Microsoft Project (MPP/XML) task durations using Aspose.Tasks for .NET."
type: docs
weight: 200
url: /net/calculate-task-duration-in-different-units/
---

## **Calculating Durations**
It can be useful to calculate the duration of a task in different units such as minutes, hours, etc.

The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class offers provides the [Duration](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/duration) property for accessing task duration, which returns the Duration class object. The Convert method exposed as part of Duration class can then be used to calculate task durations in different units. This method takes TimeUnitType as the input argument and returns the duration as a double value.

The following piece of code shows how to use this method to retrieve a task's duration in different units: minute, day, hour, week and month.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-CalculateTaskDurations-CalculateTaskDurations.cs" >}}
