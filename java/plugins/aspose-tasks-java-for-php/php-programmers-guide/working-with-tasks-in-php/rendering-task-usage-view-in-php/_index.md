---
title: Rendering Task Usage View in PHP
type: docs
weight: 140
url: /java/rendering-task-usage-view-in-php/
---

## **Aspose.Tasks - Rendering Task Usage View**
To Render Task Usage View using **Aspose.Tasks Java for PHP**, simply invoke **RenderTaskUsageView** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project('test_tasks.mpp');

\# Define the SaveOptions with required TimeScale settings as Days

$options = new PdfSaveOptions();

$timescale=new Timescale();

$options->setTimescale($timescale->Days);

\# Set the Presentation format to ResourceUsage

$presentationFormat=new PresentationFormat();

$options->setPresentationFormat($presentationFormat->TaskUsage);

\# Save the Project

$project->save("task_days.pdf", $options);

\# Set the Timescale settings to ThirdsOfMonths

$options->setTimescale($timescale->ThirdsOfMonths);

\# Save the Project

$project->save("task_thirdsOfMonths.pdf", $options);

\# Set the Timescale settings to Months

$options->setTimescale($timescale->Months);

\# Save the project

$project->save("task_months.pdf", $options);

print "Created task usage view files.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Rendering Task Usage View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/RenderTaskUsageView.php)
