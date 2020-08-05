---
title: Percentage Complete Calculations in Ruby
type: docs
weight: 110
url: /java/percentage-complete-calculations-in-ruby/
---

## **Aspose.Tasks - Percentage Complete Calculations**
To get Complete Percentage Calculations using **Aspose.Tasks Java for Ruby**, simply invoke **TasksPercentage** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'project.mpp')

\# Create a ChildTasksCollector instance

collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new

\# Collect all the tasks from RootTask using TaskUtils

Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)

tsk = Rjb::import('com.aspose.tasks.Tsk')

tasks = collector.getTasks()

\# Parse through all the collected tasks

i = 0

while i < tasks.size()

  task = tasks.get(i)

  puts task.get(tsk.PERCENT_COMPLETE).toString()

  puts task.get(tsk.PERCENT_WORK_COMPLETE).toString()

  puts task.get(tsk.PHYSICAL_PERCENT_COMPLETE).toString()

  i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Percentage Complete Calculations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/taskspercentage.rb)
