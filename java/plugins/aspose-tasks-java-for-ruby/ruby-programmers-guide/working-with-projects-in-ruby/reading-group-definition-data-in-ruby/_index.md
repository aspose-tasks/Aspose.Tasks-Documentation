---
title: Reading Group Definition Data in Ruby
description: "This article explains how to read group definition data from Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 90
url: /java/reading-group-definition-data-in-ruby/
---

## **Aspose.Tasks - Reading Group Definition Data**
To read Group Definition Data using **Aspose.Tasks Java for Ruby**, simply invoke **ReadingGroupDefinitionData** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
puts "Task Groups Count: " + project.getTaskGroups().size().to_s
task_group = project.getTaskGroups().toList().get(0)
puts "Percent Complete:" +  task_group.getName().to_s
puts "Group Criteria count: " + task_group.getGroupCriteria().size().to_s
{{< /highlight >}}

## **Download Running Code**
Download **Reading Group Definition Data (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/readinggroupdefinitiondata.rb)
