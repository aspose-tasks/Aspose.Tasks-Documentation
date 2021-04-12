---
title: Saving a Project as PDF in Ruby
description: "This article explains how to save project to PDF using Aspose.Tasks Java for Ruby."
keywords: "Convert Project Data to PDF, Convert MPP to PDF, Export MPP Project to PDF, MPP to PDF, save project data to PDF, Aspose.Tasks Java for Ruby, Ruby"
type: docs
weight: 110
url: /java/saving-a-project-as-pdf-in-ruby/
---

## **Aspose.Tasks - Saving a Project as PDF**
To Save a Project as PDF using **Aspose.Tasks Java for Ruby**, simply invoke **SaveProjectAsPdf** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new
options.setFitContent(true)
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Months)
options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').TaskUsage)
options.setLegendOnEachPage(false)
project.save("project.pdf", options)
puts "Saved project as pdf, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Saving a Project as PDF (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/saveprojectaspdf.rb)
