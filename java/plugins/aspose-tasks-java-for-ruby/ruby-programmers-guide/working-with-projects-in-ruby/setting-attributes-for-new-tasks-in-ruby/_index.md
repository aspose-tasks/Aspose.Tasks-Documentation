---
title: Setting Attributes for New Tasks in Ruby
type: docs
weight: 140
url: /java/setting-attributes-for-new-tasks-in-ruby/
---

## **Aspose.Tasks - Setting Attributes for New Tasks**
To Set Attributes for New Tasks using **Aspose.Tasks Java for Ruby**, simply invoke **SetAttributesForNewTasks** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

prj = Rjb::import('com.aspose.tasks.Prj')

\# Set new task property

project.set(prj.NEW_TASK_START_DATE, Rjb::import('com.aspose.tasks.TaskStartDateType').CurrentDate)

project.save(data_dir + "set_attributes_for_new_tasks.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)

puts "Set attributes for new tasks, please check the output file."

{{< /highlight >}}
## **Download Running Code**
Download **Setting Attributes for New Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/setattributesfornewtasks.rb)
