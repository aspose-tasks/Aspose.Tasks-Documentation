---
title: Calculate Task Duration in Different Units in Ruby
description: "Learn how to calculate Microsoft Project (MPP/XML) task durations using Aspose.Tasks Java for Ruby."
type: docs
weight: 20
url: /java/calculate-task-duration-in-different-units-in-ruby/
---

## **Aspose.Tasks - Calculate Task Duration in Different Units**
To Calculate Task Duration in Different Units using **Aspose.Tasks Java for Ruby**, simply invoke **CalculateTaskDuration** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
tsk = Rjb::import('com.aspose.tasks.Tsk')
time_unit_type = Rjb::import('com.aspose.tasks.TimeUnitType')
task = project.getRootTask().getChildren().getById(1)
puts task.get(tsk.DURATION).convert(time_unit_type.Minute).toDouble()
puts task.get(tsk.DURATION).convert(time_unit_type.Day).toDouble()
puts task.get(tsk.DURATION).convert(time_unit_type.Hour).toDouble()
puts task.get(tsk.DURATION).convert(time_unit_type.Week).toDouble()
puts task.get(tsk.DURATION).convert(time_unit_type.Month).toDouble()
{{< /highlight >}}

## **Download Running Code**
Download **Calculate Task Duration in Different Units (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/calculatetaskduration.rb)
