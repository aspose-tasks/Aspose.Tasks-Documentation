---
title: Task Baseline Duration
type: docs
weight: 20
url: /net/task-baseline-duration/
---

## **Task Baseline Duration**
The [Duration](http://www.aspose.com/api//net/tasks/aspose.tasks/taskbaseline/properties/duration) and [EstimatedDuration]() properties of the [TaskBaseLine]() class can be used to read and write the scheduled duration when the baseline was saved and determine whether the scheduled duration was estimated or not respectively.

- Duration supports the TimeSpan data type.
- EstimatedDuration supports the Boolean data type.

After saving a baseline, the task baseline duration can be viewed in Microsoft Project:

1. On the **View** menu, select **More Views** and ten **Task Entry**.
1. From the **Insert** menu, select **Columns**.
1. Add the Baseline Duration column.
### **Getting Task Baseline Duration using Aspose.Tasks**
The code below displays the task baseline duration in console window after traversing the task baselines of a task.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskBaselines-GetTaskBaselineDuration-GetTaskBaselineDuration.cs" >}}
