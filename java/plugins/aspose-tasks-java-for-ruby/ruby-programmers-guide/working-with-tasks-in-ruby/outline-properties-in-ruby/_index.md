---
title: Outline Properties in Ruby
type: docs
weight: 90
url: /java/outline-properties-in-ruby/
---

## **Aspose.Tasks - Getting Outline Properties**
To get Outline Properties using **Aspose.Tasks Java for Ruby**, call **get_outline_properties** method of **TasksProperties** module. Here you can see example code.

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
    puts "Outline Level: " + task.get(tsk.OUTLINE_LEVEL).to_string
    puts "Outline Number: " + task.get(tsk.OUTLINE_NUMBER).to_string
    puts "---------------------------------------------"
    i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/tasksproperties.rb)
