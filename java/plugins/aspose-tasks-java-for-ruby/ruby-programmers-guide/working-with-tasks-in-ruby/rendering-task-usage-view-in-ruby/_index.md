---
title: Rendering Task Usage View in Ruby
type: docs
weight: 140
url: /java/rendering-task-usage-view-in-ruby/
---

## **Aspose.Tasks - Rendering Task Usage View**
To render Task Usage View using **Aspose.Tasks Java for Ruby**, simply invoke **RenderTaskUsageView** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Days)
options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').TaskUsage)
project.save("task_days.pdf", options)
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').ThirdsOfMonths)
project.save("task_thirdsOfMonths.pdf", options)
options.setTimescale(Rjb::import('com.aspose.tasks.Timescale').Months)
project.save("task_months.pdf", options)
puts "Created task usage view files."
{{< /highlight >}}

## **Download Running Code**
Download **Rendering Task Usage View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/rendertaskusageview.rb)
