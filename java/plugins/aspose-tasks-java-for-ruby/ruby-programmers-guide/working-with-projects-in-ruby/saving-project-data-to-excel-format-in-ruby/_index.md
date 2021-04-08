---
title: Saving Project Data to Excel Format in Ruby
description: "This article explains how to export Project data to Excel using Aspose.Tasks Java for Ruby."
keywords: "Convert Project Data to XLSX, Convert MPP to XLSX, Export MPP Project to XLSX, MPP to Excel, save project data to Excel, Aspose.Tasks Java for Ruby, Ruby"
type: docs
weight: 130
url: /java/saving-project-data-to-excel-format-in-ruby/
---

## **Aspose.Tasks - Saving Project Data to Excel Format**
To Save Project Data to Excel Format using **Aspose.Tasks Java for Ruby**, simply invoke **SaveProjectDataToExcel** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.save("Project.XLSX", Rjb::import('com.aspose.tasks.SaveFileFormat').XLSX)
puts "Saved project data to Excel, please check the output file"
{{< /highlight >}}

## **Download Running Code**
Download **Saving Project Data to Excel Format (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/saveprojectdatatoexcel.rb)
