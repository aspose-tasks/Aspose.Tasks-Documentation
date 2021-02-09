---
title: Baseline Task Scheduling
type: docs
weight: 30
url: /net/baseline-task-scheduling/
---

## **Baseline Task Scheduling**
The Start and Finish properties exposed by the [TaskBaseLine](https://apireference.aspose.com/tasks/net/aspose.tasks/taskbaseline) class are used to read and write a task's start and finish dates when the baseline was saved. Both properties support the DateTime data type.

After saving a baseline, the task baseline schedule can be viewed in Microsoft Project:

1. From the **View** menu, select **More Views** and then **Task Entry**.
1. From the **Insert** menu, select **Columns**.
1. Add the desired columns.


**Baseline start and end dates in Microsoft Project** 

![todo:image_alt_text](baseline-task-scheduling_1.png)
### **Getting Task Baseline Schedule using Aspose.Tasks**
The code below displays the task baseline schedule in a console window after traversing a task's baselines.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskBaselines-GetTaskBaselineSchedule-GetTaskBaselineSchedule.cs" >}}
