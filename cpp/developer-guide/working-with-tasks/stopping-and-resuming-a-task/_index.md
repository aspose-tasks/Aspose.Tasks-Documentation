---
title: Stopping and Resuming a Task
description: "Learn how to stop or resume Microsoft Project (MPP/XML) tasks using Aspose.Tasks for C++."
type: docs
weight: 120
url: /cpp/stopping-and-resuming-a-task/
---

{{% alert color="primary" %}}

A tasks' stop date is the date that it should (or did) end. Sometimes, a task has to be stopped temporarily and then resumed later. Microsoft Project can calculate stop dates, or let users enter them manually.

{{% /alert %}}

## **Working with Stopped and Resumed Tasks**
The Stop and Resume properties exposed by the [Tsk](https://reference.aspose.com/tasks/net/aspose.tasks/tsk) class are used to read or write a task's stop and resume date:

- Stop: the date a task stops (DateTime).
- Resume: the date and time a task restarts (DateTime).

### **Microsoft Project view of Stop and Resume Dates**
To see a task's stop and resume dates:

1. In the Task Entry form, on the **Insert** menu, select **Column**.
2. Add the Stop and Resume columns.

### **Getting Stop and Resume Dates**
The stop and resume dates are NA if the task has never stopped. For date values equal to NA, Aspose.Tasks for C++ API takes the value "1/1/2000" if you're using the evaluation version. When fully licensed, Aspose.Tasks for C++ API uses DateTime.MinValue for NA values. The following code example demonstrates the stop and resume dates for all the tasks in a project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadStopResumeDates-ReadStopResumeDates.cpp" >}}
