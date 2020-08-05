---
title: Saving a Project as PDF in Ruby
type: docs
weight: 110
url: /java/saving-a-project-as-pdf-in-ruby/
---

## **Aspose.Tasks - Saving a Project as PDF**
To Save a Project as PDF using **Aspose.Tasks Java for Ruby**, simply invoke **SaveProjectAsPdf** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new

\# Set the LegendOnEachPage property to false to hide legends

\# Set the row height to fit cell content

options.setFitContent(true)

options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Months)

options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').TaskUsage)

options.setLegendOnEachPage(false)

project.save(data_dir + "project.pdf", options)

puts "Saved project as pdf, please check the output file."

{{< /highlight >}}
## **Download Running Code**
Download **Saving a Project as PDF (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/saveprojectaspdf.rb)
