---
title: Get Number of Pages in Project in PHP
description: "Learn how to get the number of pages in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
type: docs
weight: 70
url: /java/get-number-of-pages-in-project-in-php/
---

## **Aspose.Tasks - Get Number of Pages in Project**
To get Number of Pages in Project using **Aspose.Tasks Java for PHP**, simply invoke **GetNumberOfPages** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$presentation_format = new PresentationFormat();
$timescale = new Timescale();
print "Number of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->Days);
print "\nNumber of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->Months);
print "\nNumber of Pages = " . (string)$project->getPageCount($presentation_format->ResourceUsage, $timescale->ThirdsOfMonths);
{{< /highlight >}}

## **Download Running Code**
Download **Get Number of Pages in Project (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/GetNumberOfPages.php)
