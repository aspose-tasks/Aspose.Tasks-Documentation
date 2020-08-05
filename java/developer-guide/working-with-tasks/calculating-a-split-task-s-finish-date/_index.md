---
title: Calculating a Split Task's Finish Date
type: docs
weight: 70
url: /java/calculating-a-split-task-s-finish-date/
---

{{% alert color="primary" %}} 

Microsoft Project allows users to split tasks when the schedule is interrupted. Aspose.Tasks allows you to calculate the finishing date of a split task.

{{% /alert %}} 
## **Split Tasks**
The getTaskFinishDateFromDuration method exposed by the [Calendar](/pages/createpage.action?spaceKey=tasksjava&title=com.aspose.tasks.Calendar+Class&linkCreation=true&fromPageId=16581075) class is used to calculate a split task's finishing date from the start date, split parts, and duration. The getTaskFinishDateFromDuration method takes a split task and duration as its arguments and returns the tasks finish date.
### **Split Tasks in Microsoft Project**
To view the start date of a split task in Microsoft Project:

1. From the **View** menu, select **Gantt Chart**.
   The parts of a split task are connected by a line of dots. 

   **The split task in Microsoft Project** 

![todo:image_alt_text](/plugins/servlet/confluence/placeholder/unknown-attachment)
### **Calculating a Split Task's Finish Date with Aspose.Tasks**
The following code examples calculate a split task's finish date.



{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-SplitTaskFinishDate-split-task-finish-date.java" >}}
