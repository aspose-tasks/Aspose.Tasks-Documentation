---
title: Rendering Task Sheet View in PHP
type: docs
weight: 130
url: /java/rendering-task-sheet-view-in-php/
---

## **Aspose.Tasks - Rendering Task Sheet View**
To Render Task Sheet View using **Aspose.Tasks Java for PHP**, simply invoke **RenderTaskSheetView** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project('test_tasks.mpp');

\# Define the SaveOptions with required TimeScale settings as Days

$options = new PdfSaveOptions();

\# Set the Presentation format to ResourceUsage

$presentationFormat=new PresentationFormat();

$options->setPresentationFormat($presentationFormat->TaskSheet);

\# Save the Project

$project->save("taskSheet.pdf", $options);

print "Created task sheet view file.".PHP_EOL;


{{< /highlight >}}
## **Download Running Code**
Download **Rendering Task Sheet View (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/RenderTaskSheetView.php)
