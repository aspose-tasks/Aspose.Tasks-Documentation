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
The Duration and DurationFormat properties exposed by the [Task](/pages/createpage.action?spaceKey=tasksjava&title=com.aspose.tasks.Task+class&linkCreation=true&fromPageId=16581038) class are used to determine the planned duration and format of the duration of a task:

- Duration sets and gets a task's planned duration.
- DurationFormat sets and gets formats defined by the TimeUnitType enumeration.
### **Duration in Microsoft Project**
To see a task's duration in Microsoft Project:

1. From the **View** menu, select **More Views** and then **Task Entry**. 

   **Setting task duration in Microsoft Project** 

![todo:image_alt_text](managing-durations_1.png)
### **Setting task duration using Aspose.Tasks**
The following examples set the task duration to 1 day.

**Java**

{{< highlight csharp >}}

 // Create a new project

Project project = new Project();

Task task = project.getRootTask().getChildren().add("Task");

// task duration in days (default time unit)

Duration duration = task.get(Tsk.DURATION);

System.out.println("Duration in Days" + duration.toString());

// convert to hours time unit

duration = duration.convert(TimeUnitType.Hour);

System.out.println("Duration in Hours"+ duration.toString());

// get Duration instance

task.set(Tsk.DURATION, project.getDuration(1, TimeUnitType.Week));

System.out.println("1 wk" +  task.get(Tsk.DURATION).toString());

// Decrease task duration

task.set(Tsk.DURATION, task.get(Tsk.DURATION).subtract(0.5));

System.out.println("0.5 wks" + task.get(Tsk.DURATION).toString());

{{< /highlight >}}
