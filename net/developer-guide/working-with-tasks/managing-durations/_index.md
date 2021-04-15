---
title: Managing Task Durations
description: "Learn how to manage Microsoft Project (MPP/XML) task durations using Aspose.Tasks for .NET."
type: docs
weight: 60
url: /net/managing-durations/
---

Tasks take time, they have a duration. Realistic task durations help give a realistic project end date. Aspose.Tasks allows developers to set task durations in projects.

## **Working with Durations**
The [Duration](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/duration) and [DurationFormat](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/durationformat) properties exposed by the [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class are used to determine the planned duration and format of the duration of a task:

- Duration sets and gets a task's planned duration (TimeSpan).
- DurationFormat sets and gets formats defined by the TimeUnitType enumeration.

### **Duration in Microsoft Project**
To see a task's duration in Microsoft Project one can select **More Views** and then **Task Entry** From the **View** menu.

### **Setting task duration using Aspose.Tasks**
The following examples increases and decreases the task duration to 1 week and half week respectively.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WriteTaskDuration.cs" >}}
