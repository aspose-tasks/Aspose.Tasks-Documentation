---
title: Writing Updated TaskLink Data to MPP in Ruby
type: docs
weight: 40
url: /java/writing-updated-tasklink-data-to-mpp-in-ruby/
---

## **Aspose.Tasks - Writing Updated TaskLink Data to MPP**
To Write Updated TaskLink Data to MPP using **Aspose.Tasks Java for Ruby**, simply invoke **UpdateTaskLink** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'

one_sec = 10000000 # microsecond * 10

one_min = 60 * one_sec

one_hour = 60 * one_min

\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

tsk = Rjb::import('com.aspose.tasks.Tsk')

prj = Rjb::import('com.aspose.tasks.Prj')

\# Add tasks

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

\# Add four TaskLinks with different TaskLinkTypes

link1 = project.getTaskLinks().add(task1, task2, Rjb::import('com.aspose.tasks.TaskLinkType').StartToStart)

\# Save the Project

project.save(data_dir + "TaskLinks.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)

puts "Saved task links data."

{{< /highlight >}}
## **Download Running Code**
Download **Writing Updated TaskLink Data to MPP (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskLinks/updatetasklink.rb)
