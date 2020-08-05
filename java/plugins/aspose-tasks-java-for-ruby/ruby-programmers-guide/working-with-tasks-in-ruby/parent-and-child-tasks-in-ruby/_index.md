---
title: Parent and Child Tasks in Ruby
type: docs
weight: 100
url: /java/parent-and-child-tasks-in-ruby/
---

## **Aspose.Tasks - Getting Parent and Child Tasks**
To Get Parent and Child Tasks using **Aspose.Tasks Java for Ruby**, call **get_parent_and_child_tasks** method of **ParentAndChildTasks** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_parent_and_child_tasks()	

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    # Create a ChildTasksCollector instance

    collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new

    # Collect all the tasks from RootTask using TaskUtils

    Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)

    tsk = Rjb::import('com.aspose.tasks.Tsk')

    tasks = collector.getTasks()

    # Parse through all the collected tasks

    i = 0

    while i < tasks.size()

	task = tasks.get(i)

	puts "Task Name = " + task.get(tsk.NAME).to_string

	i +=1

    end

end

{{< /highlight >}}
## **Download Running Code**
Download **Parent and Child Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/parentandchildtasks.rb)
