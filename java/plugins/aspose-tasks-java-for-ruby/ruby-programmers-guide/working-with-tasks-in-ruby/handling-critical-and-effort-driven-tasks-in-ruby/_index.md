---
title: Handling Critical and Effort-driven Tasks in Ruby
type: docs
weight: 50
url: /java/handling-critical-and-effort-driven-tasks-in-ruby/
---

## **Aspose.Tasks - Handling Critical and Effort-driven Tasks**
To Handle Critical and Effort-driven Tasks using **Aspose.Tasks Java for Ruby**, simply invoke **CriticalAndEffortDrivenTasks** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'

\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Create a ChildTasksCollector instance

collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new

\# Collect all the tasks from RootTask using TaskUtils

Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)

tsk = Rjb::import('com.aspose.tasks.Tsk')

\# Parse through all the collected tasks

tasks = collector.getTasks()

i = 0

while i < tasks.size()

    task = tasks.get(i)

    puts str_ed = task.get(tsk.IS_EFFORT_DRIVEN) != nil ? "EffortDriven" : "Non-EffortDriven"

    puts str_crit = task.get(tsk.IS_CRITICAL) != nil ? "Critical" : "Non-Critical"

    i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Handling Critical and Effort-driven Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/criticalandeffortdriventasks.rb)
