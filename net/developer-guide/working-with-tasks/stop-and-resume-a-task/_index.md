---
title: Stop and Resume a Task
description: "Learn how to stop or resume Microsoft Project (MPP/XML) tasks using Aspose.Tasks for .NET."
type: docs
weight: 120
url: /net/stop-and-resume-a-task/
---

A tasks' stop date is the date that it should (or did) end. Sometimes, a task has to be stopped temporarily and then resumed later. Microsoft Project can calculate stop dates, or let users enter them manually.

## **Working with Stopped and Resumed Tasks**
The [Stop](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/stop) and [Resume](https://reference.aspose.com/tasks/net/aspose.tasks/tsk/fields/resume) properties exposed by the [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) class are used to read or write a task's stop and resume date:

- Stop: the date a task stops (DateTime).
- Resume: the data and time a task restarts (DateTime).

### **Microsoft Project view of Stop and Resume Dates**
To see a task's stop and resume dates:

1. In the Task Entry form, on the **Insert** menu, select **Column**.
2. Add the Stop and Resume columns.

### **Getting Stop and Resume Dates**
The stop and resume dates are NA if the task has never stopped. For date values equal to NA, Aspose.Tasks takes the value "1/1/2000" if you're using the evaluation version. When fully licensed, Aspose.Tasks uses DateTime.MinValue for NA values. The following examples display the stop and resume dates for all the tasks in a project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadStopResumeDates.cs" >}}
