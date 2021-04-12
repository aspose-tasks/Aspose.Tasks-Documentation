---
title: Rendering Task Usage View in PHP
description: "Learn how to render Microsoft Project (MPP/XML) task usage views using Aspose.Tasks Java for PHP."
type: docs
weight: 140
url: /java/rendering-task-usage-view-in-php/
---

## **Aspose.Tasks - Rendering Task Usage View**

To render Task Usage View using **Aspose.Tasks Java for PHP**, simply invoke **RenderTaskUsageView** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$options = new PdfSaveOptions();
$timescale = new Timescale();
$options->setTimescale($timescale->Days);
$presentationFormat = new PresentationFormat();
$options->setPresentationFormat($presentationFormat->TaskUsage);
$project->save("task_days.pdf", $options);
$options->setTimescale($timescale->ThirdsOfMonths);
$project->save("task_thirdsOfMonths.pdf", $options);
$options->setTimescale($timescale->Months);
$project->save("task_months.pdf", $options);
print "Created task usage view files.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Rendering Task Usage View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/RenderTaskUsageView.php)
