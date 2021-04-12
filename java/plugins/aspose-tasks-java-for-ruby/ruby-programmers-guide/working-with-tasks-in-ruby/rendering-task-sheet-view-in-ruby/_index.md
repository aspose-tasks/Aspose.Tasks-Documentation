---
title: Rendering Task Sheet View in Ruby
description: "Learn how to render Microsoft Project (MPP/XML) task sheet views using Aspose.Tasks Java for Ruby."
type: docs
weight: 130
url: /java/rendering-task-sheet-view-in-ruby/
---

## **Aspose.Tasks - Rendering Task Sheet View**

To render Task Sheet View using **Aspose.Tasks Java for Ruby**, simply invoke **RenderTaskSheetView** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
options = Rjb::import('com.aspose.tasks.PdfSaveOptions').new
options.setPresentationFormat(Rjb::import('com.aspose.tasks.PresentationFormat').TaskSheet)
project.save("taskSheet.pdf", options)
puts "Created task sheet view file."
{{< /highlight >}}

## **Download Running Code**
Download **Rendering Task Sheet View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/rendertasksheetview.rb)
