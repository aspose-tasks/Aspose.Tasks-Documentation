---
title: Stop and Resume a Task in Ruby
description: "Learn how to stop or resume Microsoft Project (MPP/XML) tasks using Aspose.Tasks Java for Ruby."
type: docs
weight: 170
url: /java/stop-and-resume-a-task-in-ruby/
---

## **Aspose.Tasks - Stop and Resume a Task**
To Stop and Resume a Task using **Aspose.Tasks Java for Ruby**, simply invoke **StopAndResumeTask** module. Here you can see example code.

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
    if task.get(tsk.STOP).toString() == "1/1/2015"
        puts "NA"
    else
        puts "Task Stop: " + task.get(tsk.STOP).toString()
    end

    if task.get(tsk.RESUME).toString() == "1/1/2015"
        puts "NA"
    else
        puts "Task Resume: " + task.get(tsk.RESUME).toString()
    end
        puts "---------------------------------------------"
    i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Stop and Resume a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/stopandresumetask.rb)
