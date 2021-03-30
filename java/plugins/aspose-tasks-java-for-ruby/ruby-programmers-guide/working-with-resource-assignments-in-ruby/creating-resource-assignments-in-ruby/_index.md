---
title: Creating Resource Assignments in Ruby
type: docs
weight: 30
url: /java/creating-resource-assignments-in-ruby/
---

## **Aspose.Tasks - Creating Resource Assignments**
To Create Resource Assignments using **Aspose.Tasks Java for Ruby**, simply invoke **CreateResourceAssignment** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

task = project.getRootTask().getChildren().add("Task")

rsc = project.getResources().add("Rsc")

assignment = project.getResourceAssignments().add(task, rsc)

puts "Created resource assignment."

{{< /highlight >}}
## **Download Running Code**
Download **Creating Resource Assignments (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/createresourceassignment.rb)
