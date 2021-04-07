---
title: Handling Priorities in Ruby
description: "Learn how to handle Microsoft Project (MPP/XML) priorities using Aspose.Tasks Java for Ruby."
type: docs
weight: 60
url: /java/handling-priorities-in-ruby/
---

## **Aspose.Tasks - Handling Priorities**
To Handle Priorities using **Aspose.Tasks Java for Ruby**, simply invoke **HandlingPriorities** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new
Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)
tasks = collector.getTasks()
tsk = Rjb::import('com.aspose.tasks.Tsk')
i = 0
while i < tasks.size()
    task = tasks.get(i)
    puts "Priority: " + task.get(tsk.PRIORITY).toString()
    puts "---------------------------------------------"
    i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Handling Priorities (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/handlingpriorities.rb)
