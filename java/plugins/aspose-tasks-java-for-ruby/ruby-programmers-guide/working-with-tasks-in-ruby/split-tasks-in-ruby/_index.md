---
title: Split Tasks in Ruby
description: "Learn how to split Microsoft Project (MPP/XML) tasks using Aspose.Tasks Java for Ruby."
type: docs
weight: 160
url: /java/split-tasks-in-ruby/
---

## **Aspose.Tasks - Split Tasks**
To Split Tasks using **Aspose.Tasks Java for Ruby**, simply invoke **SplitTasks** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
prj = Rjb::import('com.aspose.tasks.Prj')
tsk = Rjb::import('com.aspose.tasks.Tsk')
calendar = project.get(prj.CALENDAR)
cal = Rjb::import('java.util.Calendar').getInstance()
cal.set(2011, 3, 15, 8, 0, 0)
project.set(prj.START_DATE, cal.getTime())
cal.set(2011, 3, 21, 17, 0, 0)
project.set(prj.FINISH_DATE, cal.getTime())
rootTask = project.getRootTask()
rootTask.set(tsk.NAME, "Root")
taskToSplit = rootTask.getChildren().add("Task1")
taskToSplit.set(tsk.DURATION, project.getDuration(3))
splitResourceAssignment = project.getResourceAssignments().add(taskToSplit, nil)
splitResourceAssignment.timephasedDataFromTaskDuration(calendar)
cal = Rjb::import('java.util.Calendar').getInstance()
cal2 = Rjb::import('java.util.Calendar').getInstance()
cal.set(2011, 3, 16, 8, 0, 0)
cal2.set(2011, 3, 16, 17, 0, 0)
splitResourceAssignment.splitTask(cal.getTime(), cal2.getTime(), calendar)
cal.set(2011, 3, 18, 8, 0, 0)
cal2.set(2011, 3, 18, 17, 0, 0)
splitResourceAssignment.splitTask(cal.getTime(), cal2.getTime(), calendar)
splitResourceAssignment.set(Rjb::import('com.aspose.tasks.Asn').WORK_CONTOUR, Rjb::import('com.aspose.tasks.WorkContourType').Contoured)
project.save("SplitTasks.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
{{< /highlight >}}

## **Download Running Code**
Download **Split Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/splittasks.rb)
