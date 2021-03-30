---
title: Task Baseline Duration in Ruby
type: docs
weight: 30
url: /java/task-baseline-duration-in-ruby/
---

## **Aspose.Tasks - Task Baseline Duration**
To get Task Baseline Duration using **Aspose.Tasks Java for Ruby**, simply invoke **TaskBaselineDuration** module. Here you can see example code.

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

{{< /highlight >}}
## **Download Running Code**
Download **Task Baseline Duration (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskBaselines/taskbaselineduration.rb)
