---
title: WBS Associated with a Task in Ruby
type: docs
weight: 180
url: /java/wbs-associated-with-a-task-in-ruby/
---

## **Aspose.Tasks - WBS Associated with a Task**
To WBS Associated with a Task using **Aspose.Tasks Java for Ruby**, simply invoke **WBSAssociatedWithTask** module. Here you can see example code.

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
    puts "WBS: " + task.get(tsk.WBS).to_string
    puts "WBS Level: " + task.get(tsk.WBS_LEVEL).to_s
    i +=1
end
{{< /highlight >}}

## **Download Running Code**
Download **WBS Associated with a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/wbsassociatedwithtask.rb)
