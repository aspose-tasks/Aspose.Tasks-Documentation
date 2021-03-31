---
title: Managing Durations
type: docs
weight: 60
url: /java/managing-durations/
---

{{% alert color="primary" %}} 

Tasks take time: they have a duration. Realistic task duration help give a realistic project end date. Aspose.Tasks allows developers set task duration in projects.

{{% /alert %}} 
## **Working with Durations**
The Duration and DurationFormat properties exposed by the [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task/) class are used to determine the planned duration and format of the duration of a task:

- Duration sets and gets a task's planned duration.
- DurationFormat sets and gets formats defined by the TimeUnitType enumeration.
### **Duration in Microsoft Project**
To see a task's duration in Microsoft Project:

1. From the **View** menu, select **More Views** and then **Task Entry**. 

   **Setting task duration in Microsoft Project** 

![how to manage task duration in Microsoft Project](managing-durations_1.png)
### **Setting task duration using Aspose.Tasks**
The following examples increases and decreases the task duration to 1 week and half week respectively.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-ManageDurations-ManageDurations.java" >}}
