---
title: Microsoft Project MPP File Update in Ruby
description: "Learn how to update Microsoft Project (MPP/XML) project files using Aspose.Tasks Java for Ruby."
type: docs
weight: 80
url: /java/microsoft-project-mpp-file-update-in-ruby/
---

## **Aspose.Tasks - Update Project File**
To Update Project File using **Aspose.Tasks Java for Ruby**, simply invoke **UpdateProjectFile** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
task = project.getRootTask().getChildren().add("Task1")
cal = Rjb::import('java.util.Calendar').getInstance()
cal.set(2015, 7, 1, 8, 0,0);
task.set(Rjb::import('com.aspose.tasks.Tsk').START, cal.getTime())
cal.set(2015, 7, 1, 17, 0, 0)
task.set(Rjb::import('com.aspose.tasks.Tsk').FINISH , cal.getTime())
project.save("AfterLinking.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)
puts "Project file updated, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Update Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/updateprojectfile.rb)
