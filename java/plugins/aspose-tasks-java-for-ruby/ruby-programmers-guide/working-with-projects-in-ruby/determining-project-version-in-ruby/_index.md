---
title: Determining Project Version in Ruby
description: "Learn how to check Microsoft Project (MPP/XML) version using Aspose.Tasks Java for Ruby."
type: docs
weight: 40
url: /java/determining-project-version-in-ruby/
---

## **Aspose.Tasks - Determining Project Version**
To Determine Project Version using **Aspose.Tasks Java for Ruby**, simply invoke **ProjectVersion** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('Sample.xml')
puts "Project Version : " + project.get(Rjb::import('com.aspose.tasks.Prj').SAVE_VERSION).to_string
puts "Last Saved : " + project.get(Rjb::import('com.aspose.tasks.Prj').LAST_SAVED).to_string
{{< /highlight >}}

## **Download Running Code**
Download **Determining Project Version (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/projectversion.rb)
