---
title: Parent and Child Tasks in Ruby
type: docs
weight: 100
url: /java/parent-and-child-tasks-in-ruby/
---

## **Aspose.Tasks - Getting Parent and Child Tasks**
To get parent and Child Tasks using **Aspose.Tasks Java for Ruby**, call **get_parent_and_child_tasks** method of **ParentAndChildTasks** module. Here you can see example code.

{{< highlight ruby >}}
def get_parent_and_child_tasks()	
    project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
    collector = Rjb::import('com.aspose.tasks.ChildTasksCollector').new
    Rjb::import('com.aspose.tasks.TaskUtils').apply(project.getRootTask(), collector, 0)
    tsk = Rjb::import('com.aspose.tasks.Tsk')
    tasks = collector.getTasks()
    i = 0
    while i < tasks.size()
    	task = tasks.get(i)
        puts "Task Name = " + task.get(tsk.NAME).to_string
        i += 1
    end
end
{{< /highlight >}}

## **Download Running Code**
Download **Parent and Child Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/parentandchildtasks.rb)
