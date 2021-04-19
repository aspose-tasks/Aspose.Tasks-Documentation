---
title: Render Resource Usage or Sheet Views in Ruby
description: "Learn how to read Microsoft Project (MPP/XML) resource usage and resource sheet views using Aspose.Tasks Java for Ruby."
type: docs
weight: 30
url: /java/rendering-resource-usage-and-resource-sheet-view-in-ruby/
---

## **Aspose.Tasks - Rendering Resource Usage**
To render Resource Usage using **Aspose.Tasks Java for Ruby**, call **render_resource_usage** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Days)
options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').ResourceUsage)
project.save("result_days.pdf", options)
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').ThirdsOfMonths)
project.save("result_thirdsOfMonths.pdf", options)
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Months)
project.save("result_months.pdf", options)
puts "Created resource usage files."
{{< /highlight >}}

## **Aspose.Tasks - Rendering Resource Sheet View**
To render Resource Sheet View using **Aspose.Tasks Java for Ruby**, call **render_resource_sheetview** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new
options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').ResourceSheet)
project.save("result.pdf", options)
puts "Created resource sheet view file."
{{< /highlight >}}

## **Download Running Code**
Download **Rendering Resource Usage and Resource Sheet View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/renderresourceusageandsheetview.rb)
