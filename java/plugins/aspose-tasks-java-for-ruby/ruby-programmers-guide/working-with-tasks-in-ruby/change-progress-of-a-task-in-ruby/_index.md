---
title: Change Progress of a Task in Ruby
type: docs
weight: 30
url: /java/change-progress-of-a-task-in-ruby/
---

## **Aspose.Tasks - Change Progress of a Task**
To Change Progress of a Task presentation using **Aspose.Tasks Java for Ruby**, simply invoke **ChangeProgressOfTask** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
puts project.getCalculationMode()
task = project.getRootTask().getChildren().add("Task")
tsk = Rjb::import('com.aspose.tasks.Tsk')
task.set(tsk.DURATION, project.getDuration(2))
task.set(tsk.PERCENT_COMPLETE, 50)
puts "Changed progress of task."
{{< /highlight >}}

## **Download Running Code**
Download **Change Progress of a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/changeprogressoftask.rb)
