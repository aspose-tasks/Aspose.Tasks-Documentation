---
title: Creating a Task Baseline in Ruby
type: docs
weight: 20
url: /java/creating-a-task-baseline-in-ruby/
---

## **Aspose.Tasks - Creating a Task Baseline**
To create a Task Baseline using **Aspose.Tasks Java for Ruby**, simply invoke **CreateTaskBaseline** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.setBaseline(Rjb::import('com.aspose.tasks.BaselineType').Baseline)
puts "Set baseline for the project."
{{< /highlight >}}

## **Download Running Code**
Download **Creating a Task Baseline (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskBaselines/createtaskbaseline.rb)
