---
title: General Properties in Ruby
type: docs
weight: 40
url: /java/general-properties-in-ruby/
---

## **Aspose.Tasks - Getting General Properties**
To Get General Properties using **Aspose.Tasks Java for Ruby**, call **get_general_properties** method of **TasksProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_general_properties()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    # Create a ChildTasksCollector instance

    collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new

	# Collect all the tasks from RootTask using TaskUtils

	Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)

	tasks = collector.getTasks()



	tsk = Rjb::import('com.aspose.tasks.Tsk')

	# Parse through all the collected tasks

	i = 0

	while i < tasks.size()

		task = tasks.get(i)

	    puts "Task Id:" + task.get(tsk.ID).to_string

	    puts "Task Uid: " + task.get(tsk.UID).to_string

	    puts "Task Name: " + task.get(tsk.NAME).to_string

	    puts "Task Start: " + task.get(tsk.START).to_string

	    puts "Task Finish: "+  task.get(tsk.FINISH).to_string

	    puts "---------------------------------------------"

	    i +=1

	end

end

{{< /highlight >}}
## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/tasksproperties.rb)
