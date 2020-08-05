---
title: Calculate Task Duration in Different Units in Ruby
type: docs
weight: 20
url: /java/calculate-task-duration-in-different-units-in-ruby/
---

## **Aspose.Tasks - Calculate Task Duration in Different Units**
To Calculate Task Duration in Different Units using **Aspose.Tasks Java for Ruby**, simply invoke **CalculateTaskDuration** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

tsk = Rjb::import('com.aspose.tasks.Tsk')

time_unit_type = Rjb::import('com.aspose.tasks.TimeUnitType')

\# Get a task to calculate its duration in different formats

task = project.getRootTask().getChildren().getById(1)

\# Get the duration in Minutes

puts task.get(tsk.DURATION).convert(time_unit_type.Minute).toDouble()

\# Get the duration in Days

puts task.get(tsk.DURATION).convert(time_unit_type.Day).toDouble()

\# Get the duration in Hours

puts task.get(tsk.DURATION).convert(time_unit_type.Hour).toDouble()

\# Get the duration in Weeks

puts task.get(tsk.DURATION).convert(time_unit_type.Week).toDouble()

\# Get the duration in Months

puts task.get(tsk.DURATION).convert(time_unit_type.Month).toDouble()

{{< /highlight >}}
## **Download Running Code**
Download **Calculate Task Duration in Different Units (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/calculatetaskduration.rb)
