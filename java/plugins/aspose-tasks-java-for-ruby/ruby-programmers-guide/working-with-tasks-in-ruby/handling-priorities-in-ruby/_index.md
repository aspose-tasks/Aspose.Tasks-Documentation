---
title: Handling Priorities in Ruby
type: docs
weight: 60
url: /java/handling-priorities-in-ruby/
---

## **Aspose.Tasks - Handling Priorities**
To Handle Priorities using **Aspose.Tasks Java for Ruby**, simply invoke **HandlingPriorities** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Create a ChildTasksCollector instance

collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new

\# Collect all the tasks from RootTask using TaskUtils

Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)

tasks = collector.getTasks()

tsk = Rjb::import('com.aspose.tasks.Tsk')

\# Parse through all the collected tasks

i = 0

while i < tasks.size()

    task = tasks.get(i)

    puts "Priority: " + task.get(tsk.PRIORITY).toString()

    puts "---------------------------------------------"

    i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Handling Priorities (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/handlingpriorities.rb)
