---
title: Render Resource Usage or Sheet Views in PHP
description: "Learn how to read Microsoft Project (MPP/XML) resource usage and resource sheet views using Aspose.Tasks Java for PHP."
type: docs
weight: 30
url: /java/rendering-resource-usage-and-resource-sheet-view-in-php/
---

## **Aspose.Tasks - Rendering Resource Usage**
To render Resource Usage using **Aspose.Tasks Java for PHP**, call **render_resource_usage** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$options = new PdfSaveOptions();
$timescale = new Timescale();
$options->setTimescale($timescale->Days);
$presentationFormat = new PresentationFormat();
$options->setPresentationFormat($presentationFormat->ResourceUsage);
$project->save("result_days.pdf", $options);
$options->setTimescale($timescale->ThirdsOfMonths);
$project->save("result_thirdsOfMonths.pdf", $options);
$options->setTimescale($timescale->Months);
$project->save("result_months.pdf", $options);
print "Created resource usage files.";
{{< /highlight >}}

## **Aspose.Tasks - Rendering Resource Sheet View**
To render Resource Sheet View using **Aspose.Tasks Java for PHP**, call **render_resource_sheetview** method of **RenderResourceUsageAndSheetView** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$options = new PdfSaveOptions();
$presentationFormat = new PresentationFormat();
$options->setPresentationFormat($presentationFormat->ResourceSheet);
$project->save("result.pdf", $options);
print "Created resource sheet view file.";
{{< /highlight >}}

## **Download Running Code**
Download **Rendering Resource Usage and Resource Sheet View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/RenderResourceUsageAndSheetView.php)
