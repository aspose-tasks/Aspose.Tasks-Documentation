---
title: Calculating a Split Task's Finish Date
description: "Learn how to calculate Microsoft Project (MPP/XML) split task's finish dates using Aspose.Tasks for Java."
type: docs
weight: 70
url: /java/calculating-split-task-s-finish-date/
aliases:
   - /java/calculating-a-split-task-s-finish-date/
---

{{% alert color="primary" %}}

Microsoft Project allows users to split tasks when the schedule is interrupted. Aspose.Tasks allows you to calculate the finishing date of a split task.

{{% /alert %}}

## **Split Tasks**
The getTaskFinishDateFromDuration method exposed by the [Calendar](https://apireference.aspose.com/tasks/java/com.aspose.tasks/calendar) class is used to calculate a split task's finishing date from the start date, split parts, and duration. The getTaskFinishDateFromDuration method takes a split task and duration as its arguments and returns the tasks finish date.

### **Split Tasks in Microsoft Project**
To view the start date of a split task in Microsoft Project from the **View** menu, select **Gantt Chart**. The parts of a split task are connected by a line of dots. 

**The split task in Microsoft Project**
![split task in Microsoft Project](Split-Tasks-001.png)

### **Calculating a Split Task's Finish Date with Aspose.Tasks**
The following code examples calculate a split task's finish date.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-SplitTaskFinishDate-split-task-finish-date.java" >}}
