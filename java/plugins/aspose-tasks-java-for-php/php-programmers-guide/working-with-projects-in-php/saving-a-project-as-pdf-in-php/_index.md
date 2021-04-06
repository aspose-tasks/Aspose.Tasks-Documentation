---
title: Saving a Project as PDF in PHP
type: docs
weight: 110
url: /java/saving-a-project-as-pdf-in-php/
---

## **Aspose.Tasks - Saving a Project as PDF**
To Save a Project as PDF using **Aspose.Tasks Java for PHP**, simply invoke **SaveProjectAsPdf** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project($dataDir . 'test_tasks.mpp');

$options = new PdfSaveOptions();

\# Set the LegendOnEachPage property to false to hide legends

\# Set the row height to fit cell content

$timescale=new Timescale();

$presentationFormat=new PresentationFormat();

$options->setFitContent(true);

$options->setTimescale($timescale->Months);

$options->setPresentationFormat($presentationFormat->TaskUsage);

$options->setLegendOnEachPage(false);

$project->save($dataDir . "project.pdf", $options);

print "Saved project as pdf, please check the output file.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Saving a Project as PDF (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/SaveProjectAsPdf.php)
