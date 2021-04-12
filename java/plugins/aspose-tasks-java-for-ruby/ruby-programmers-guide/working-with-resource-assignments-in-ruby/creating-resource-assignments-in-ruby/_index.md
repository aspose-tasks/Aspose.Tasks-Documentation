---
title: Creating Resource Assignments in Ruby
description: "Learn how to create resource assignments linking tasks and resources in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 30
url: /java/creating-resource-assignments-in-ruby/
---

## **Aspose.Tasks - Creating Resource Assignments**
To create Resource Assignments using **Aspose.Tasks Java for Ruby**, simply invoke **CreateResourceAssignment** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
task = project.getRootTask().getChildren().add("Task")
rsc = project.getResources().add("Rsc")
assignment = project.getResourceAssignments().add(task, rsc)
puts "Created resource assignment."
{{< /highlight >}}

## **Download Running Code**
Download **Creating Resource Assignments (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/createresourceassignment.rb)
