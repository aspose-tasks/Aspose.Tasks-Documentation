---
title: Rendering Resource Usage and Resource Sheet View in Ruby
type: docs
weight: 30
url: /java/rendering-resource-usage-and-resource-sheet-view-in-ruby/
---

## **Aspose.Tasks - Rendering Resource Usage**
To Render Resource Usage using **Aspose.Tasks Java for Ruby**, call **render_resource_usage** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def render_resource_usage()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    # Define the SaveOptions with required TimeScale settings as Days

    options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new

    options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Days)

    # Set the Presentation format to ResourceUsage

    options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').ResourceUsage)

    # Save the Project

    project.save(data_dir + "result_days.pdf", options)

    # Set the Tiemscale settings to ThirdsOfMonths

    options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').ThirdsOfMonths)

    # Save the Project

    project.save(data_dir + "result_thirdsOfMonths.pdf", options)

    # Set the Timescale settings to Months

    options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Months)

    # Save the project

    project.save(data_dir + "result_months.pdf", options)

    puts "Created resource usage files."

end

{{< /highlight >}}
## **Aspose.Tasks - Rendering Resource Sheet View**
To Render Resource Sheet View using **Aspose.Tasks Java for Ruby**, call **render_resource_sheetview** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def render_resource_sheetview()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    # Define the SaveOptions with required TimeScale settings as Days

    options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new



    # Set the Presentation format to ResourceSheet

    options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').ResourceSheet)

    project.save(data_dir + "result.pdf", options)

    puts "Created resource sheet view file."

end

{{< /highlight >}}
## **Download Running Code**
Download **Rendering Resource Usage and Resource Sheet View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/renderresourceusageandsheetview.rb)
