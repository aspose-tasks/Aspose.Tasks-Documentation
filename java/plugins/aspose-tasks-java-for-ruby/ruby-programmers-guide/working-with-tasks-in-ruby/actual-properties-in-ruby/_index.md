---
title: Actual Properties in Ruby
type: docs
weight: 10
url: /java/actual-properties-in-ruby/
---

## **Aspose.Tasks - Getting Actual Properties**
To get Actual Properties using **Aspose.Tasks Java for Ruby**, call **get_actual_properties** method of **TasksProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
def get_actual_properties()
    project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
    collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new
    Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)
    tasks = collector.getTasks()
    tsk = Rjb::import('com.aspose.tasks.Tsk')
    i = 0
    while i < tasks.size()
      task = tasks.get(i)
      puts "Task Name : " + task.get(tsk.NAME).to_string
      puts "Actual Start: " + task.get(tsk.ACTUAL_START).toString()
      puts "Actual Finish: " + task.get(tsk.ACTUAL_FINISH).toString()
      puts "Actual Duration: " + task.get(tsk.ACTUAL_DURATION).toString()
      puts "Actual Cost: " + task.get(tsk.ACTUAL_COST).toString()
      puts "---------------------------------------------"
      i += 1
    end
end
{{< /highlight >}}

## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/tasksproperties.rb)
