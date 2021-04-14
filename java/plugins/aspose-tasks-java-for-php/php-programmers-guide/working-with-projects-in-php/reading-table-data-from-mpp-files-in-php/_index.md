---
title: Reading Table Data from MPP files in PHP
description: "This article explains how to read table data from Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
keywords: "read table data, read MPP table data, Export table data MPP, Aspose.Tasks Java for PHP, PHP"
type: docs
weight: 100
url: /java/reading-table-data-from-mpp-files-in-php/
---

## **Aspose.Tasks - Reading Table Data from MPP files**
To read Table Data from MPP files using **Aspose.Tasks Java for PHP**, simply invoke **ReadingTableData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$t1 = $project->getTables()->toList()->get(0);
print "Table Fields Count" . (string)$t1->getTableFields()->size();
$f = $t1->getTableFields()->get(0);
print "Field width: " . (string)$f->getWidth();
print "\nField Title: " . (string)$f->getTitle();
print "\nField Title Alignment: " . (string)$f->getAlignTitle();
print "\nField Align Data: " . $f->getAlignData();
$f = $t1->getTableFields()->get(1);
print "\nField width: " . (string)$f->getWidth();
print "\nField Title: " . (string)$f->getTitle();
print "\nField Title Alignment: " . (string)$f->getAlignTitle();
print "\nField Align Data: " . (string)$f->getAlignData();
{{< /highlight >}}

## **Download Running Code**
Download **Reading Table Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ReadingTableData.php)
