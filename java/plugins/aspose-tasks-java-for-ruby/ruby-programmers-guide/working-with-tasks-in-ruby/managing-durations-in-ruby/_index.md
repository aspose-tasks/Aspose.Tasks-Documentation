---
title: Managing Durations in Ruby
type: docs
weight: 70
url: /java/managing-durations-in-ruby/
---

## **Aspose.Tasks - Managing Durations**
To Manage Durations using **Aspose.Tasks Java for Ruby**, simply invoke **ManagingDuration** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new

task = project.getRootTask().getChildren().add("Task")

tsk = Rjb::import('com.aspose.tasks.Tsk')

\# task duration in days (default time unit)

duration = task.get(tsk.DURATION)

puts "Duration in Days: " + duration.toString()

\# convert to hours time unit

duration = duration.convert(Rjb::import('com.aspose.tasks.TimeUnitType').Hour)

puts "Duration in Hours: "+ duration.toString()

\# Decrease task duration

task.set(tsk.DURATION, task.get(tsk.DURATION).subtract(0.5))

puts "0.5 weeks: " + task.get(tsk.DURATION).toString()

{{< /highlight >}}
## **Download Running Code**
Download **Managing Durations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/managingduration.rb)
