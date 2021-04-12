---
title: Managing Task Durations in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) task durations using Aspose.Tasks Java for Ruby."
type: docs
weight: 70
url: /java/managing-durations-in-ruby/
---

## **Aspose.Tasks - Managing Durations**
To manage durations using **Aspose.Tasks Java for Ruby**, simply invoke **ManagingDuration** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
task = project.getRootTask().getChildren().add("Task")
tsk = Rjb::import('com.aspose.tasks.Tsk')
duration = task.get(tsk.DURATION)
puts "Duration in Days: " + duration.toString()
duration = duration.convert(Rjb::import('com.aspose.tasks.TimeUnitType').Hour)
puts "Duration in Hours: "+ duration.toString()
task.set(tsk.DURATION, task.get(tsk.DURATION).subtract(0.5))
puts "0.5 weeks: " + task.get(tsk.DURATION).toString()
{{< /highlight >}}

## **Download Running Code**
Download **Managing Durations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/managingduration.rb)
