---
title: Managing Task Costs in Ruby
description: "Learn how to manage Microsoft Project (MPP/XML) task costs using Aspose.Tasks Java for Ruby."
type: docs
weight: 80
url: /java/managing-task-costs-in-ruby/
---

## **Aspose.Tasks - Managing Task Costs**
To manage Task Costs using **Aspose.Tasks Java for Ruby**, simply invoke **ManagingTaskCosts** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
task = project.getRootTask().getChildren().add("Task")
tsk = Rjb::import('com.aspose.tasks.Tsk')
task.set(tsk.COST, Rjb::import('java.math.BigDecimal').valueOf(800))
puts "Task Remaining Cost: " + task.get(tsk.REMAINING_COST).to_string
puts "Task Fixed Cost: " + task.get(tsk.FIXED_COST).to_string
puts "Task Cost Variance: " + task.get(tsk.COST_VARIANCE).to_string
puts "Project Cost: " + project.getRootTask().get(tsk.COST).to_string
puts "Project Fixed Cost: " + project.getRootTask().get(tsk.FIXED_COST).to_string
puts "Project Remaining Cost: " + project.getRootTask().get(tsk.REMAINING_COST).to_string
puts "Project Variance Cost: " + project.getRootTask().get(tsk.COST_VARIANCE).to_string
{{< /highlight >}}

## **Download Running Code**
Download **Managing Task Costs (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/managingtaskcosts.rb)
