---
title: Creating a Task Link in Ruby
description: "Learn how to create task links in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/creating-a-task-link-in-ruby/
---

## **Aspose.Tasks - Creating a Task Link**
To create a Task Link using **Aspose.Tasks Java for Ruby**, simply invoke **CreateTaskLink** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
pred = project.getRootTask().getChildren().add("Task 1")
succ = project.getRootTask().getChildren().add("Task 2")
link = project.getTaskLinks().add(pred, succ)
puts "Created task link."
{{< /highlight >}}

## **Download Running Code**
Download **Creating a Task Link (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskLinks/createtasklink.rb)
