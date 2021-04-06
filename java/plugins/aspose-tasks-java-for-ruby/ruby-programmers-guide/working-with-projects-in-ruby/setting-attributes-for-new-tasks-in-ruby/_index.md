---
title: Setting Attributes for New Tasks in Ruby
type: docs
weight: 140
url: /java/setting-attributes-for-new-tasks-in-ruby/
---

## **Aspose.Tasks - Setting Attributes for New Tasks**
To set attributes for new tasks using **Aspose.Tasks Java for Ruby**, simply invoke **SetAttributesForNewTasks** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
prj = Rjb::import('com.aspose.tasks.Prj')
project.set(prj.NEW_TASK_START_DATE, Rjb::import('com.aspose.tasks.TaskStartDateType').CurrentDate)
project.save("set_attributes_for_new_tasks.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Set attributes for new tasks, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Setting Attributes for New Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/setattributesfornewtasks.rb)
