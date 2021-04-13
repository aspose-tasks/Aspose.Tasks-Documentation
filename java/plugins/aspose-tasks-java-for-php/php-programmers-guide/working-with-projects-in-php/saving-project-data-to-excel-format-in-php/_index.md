---
title: Saving Project Data to Excel Format in PHP
description: "This article explains how to export project data to Excel using Aspose.Tasks Java for PHP."
keywords: "Convert Project Data to XLSX, Convert MPP to XLSX, Export MPP Project to XLSX, MPP to Excel, save project data to Excel, Aspose.Tasks Java for PHP, PHP"
type: docs
weight: 130
url: /java/saving-project-data-to-excel-format-in-php/
---

## **Aspose.Tasks - Saving Project Data to Excel Format**
To Save Project Data to Excel Format using **Aspose.Tasks Java for PHP**, simply invoke **SaveProjectDataToExcel** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$saveFileFormat = new SaveFileFormat();
$project->save("Project.XLSX", $saveFileFormat->XLSX);
print "Saved project data to Excel, please check the output file".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Saving Project Data to Excel Format (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/SaveProjectDataToExcel.php)
