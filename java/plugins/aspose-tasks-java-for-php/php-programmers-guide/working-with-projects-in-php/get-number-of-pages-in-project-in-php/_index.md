---
title: Get Number of Pages in Project in PHP
type: docs
weight: 70
url: /java/get-number-of-pages-in-project-in-php/
---

## **Aspose.Tasks - Get Number of Pages in Project**
To Get Number of Pages in Project using **Aspose.Tasks Java for PHP**, simply invoke **GetNumberOfPages** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project($dataDir . 'test_tasks.mpp');

$presentation_format = new PresentationFormat();

$timescale = new Timescale();

\# Get number of pages

print "Number of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->Days).PHP_EOL;

\# Get number of pages (Months)

print "Number of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->Months).PHP_EOL;

\# Get number of pages (ThirdsOfMonths)

print "Number of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->ThirdsOfMonths).PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Get Number of Pages in Project (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/GetNumberOfPages.php)
