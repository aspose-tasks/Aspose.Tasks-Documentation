---
title: Handling Critical and Effort-driven Tasks in Ruby
description: "Learn how to handle Microsoft Project (MPP/XML) critical and effort-driven tasks using Aspose.Tasks Java for Ruby."
type: docs
weight: 50
url: /java/handling-critical-and-effort-driven-tasks-in-ruby/
---

## **Aspose.Tasks - Handling Critical and Effort-driven Tasks**
To Handle Critical and Effort-driven Tasks using **Aspose.Tasks Java for Ruby**, simply invoke **CriticalAndEffortDrivenTasks** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new
Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)
tsk = Rjb::import('com.aspose.tasks.Tsk')
tasks = collector.getTasks()
i = 0
while i < tasks.size()
    task = tasks.get(i)
    puts str_ed = task.get(tsk.IS_EFFORT_DRIVEN) != nil ? "EffortDriven" : "Non-EffortDriven"
    puts str_crit = task.get(tsk.IS_CRITICAL) != nil ? "Critical" : "Non-Critical"
    i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Handling Critical and Effort-driven Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/criticalandeffortdriventasks.rb)
