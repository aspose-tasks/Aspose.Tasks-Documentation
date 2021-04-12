---
title: Creating an Empty Project File in Ruby
description: "Learn how to create Microsoft Project (MPP/XML) empty project using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/creating-an-empty-project-file-in-ruby/
---

## **Aspose.Tasks - Creating an Empty Project File**
To create an Empty Project File using **Aspose.Tasks Java for Ruby**, simply invoke **CreateEmptyProject** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
project_stream =  Rjb::import('java.io.FileOutputStream').new("Project1.xml")
project.save(project_stream, Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
project_stream.close()
puts "Created project Successfully."
{{< /highlight >}}

## **Download Running Code**
Download **Creating an Empty Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/createemptyproject.rb)
