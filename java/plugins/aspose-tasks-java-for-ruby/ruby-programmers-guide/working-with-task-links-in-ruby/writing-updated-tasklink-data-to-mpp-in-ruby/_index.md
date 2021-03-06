---
title: Writing Updated TaskLink Data to MPP in Ruby
description: "Learn how to write Microsoft Project (MPP/XML) task links using Aspose.Tasks Java for Ruby."
type: docs
weight: 40
url: /java/writing-updated-tasklink-data-to-mpp-in-ruby/
---

## **Aspose.Tasks - Writing Updated TaskLink Data to MPP**
To write Updated TaskLink Data to MPP using **Aspose.Tasks Java for Ruby**, simply invoke **UpdateTaskLink** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
one_sec = 10000000
one_min = 60 * one_sec
one_hour = 60 * one_min
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
tsk = Rjb::import('com.aspose.tasks.Tsk')
prj = Rjb::import('com.aspose.tasks.Prj')
task1 = project.getRootTask().getChildren().add("1")
task1.set(tsk.DURATION, project.getDuration(8, Rjb::import('com.aspose.tasks.TimeUnitType').Hour))
task1.set(tsk.START, project.get(prj.START_DATE))
task1.set(tsk.FINISH, project.get(prj.CALENDAR).getTaskFinishDateFromDuration(task1, task1.get(tsk.DURATION).toDouble()))
task2 = project.getRootTask().getChildren().add("2")
task2.set(tsk.DURATION, project.getDuration(8, Rjb::import('com.aspose.tasks.TimeUnitType').Hour))
task2.set(tsk.START, project.get(prj.START_DATE))
task2.set(tsk.FINISH, project.get(prj.CALENDAR).getTaskFinishDateFromDuration(task2, task2.get(tsk.DURATION).toDouble()))
project.getRootTask().getChildren().add(task1)
project.getRootTask().getChildren().add(task2)
link1 = project.getTaskLinks().add(task1, task2, Rjb::import('com.aspose.tasks.TaskLinkType').StartToStart)
project.save("TaskLinks.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)
puts "Saved task links data."
{{< /highlight >}}

## **Download Running Code**
Download **Writing Updated TaskLink Data to MPP (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskLinks/updatetasklink.rb)
