---
title: Baseline Task Scheduling in Ruby
description: "Learn how to edit Microsoft Project (MPP/XML) task baselines using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/baseline-task-scheduling-in-ruby/
---

## **Aspose.Tasks - Baseline Task Scheduling**
To get Baseline Task Scheduling using **Aspose.Tasks Java for Ruby**, simply invoke **TaskBaselineSchedule** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'

oneSecond = 10000000

oneMinute = 60 * oneSecond

oneHour = 60 * oneMinute

\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new

\# Creating TaskBaseline:

task = project.getRootTask().getChildren().add("Task")

project.setBaseline(Rjb::import('com.aspose.tasks.BaselineType').Baseline)

baseline = task.getBaselines().toList().get(0)

duration = baseline.getDuration().toDouble()

baseline_duration = duration / oneHour

puts baseline_duration

puts "Baseline Start: "  + baseline.getStart().to_string

puts "Baseline Finish: " + baseline.getFinish().to_string

{{< /highlight >}}
## **Download Running Code**
Download **Baseline Task Scheduling (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskBaselines/taskbaselineschedule.rb)
