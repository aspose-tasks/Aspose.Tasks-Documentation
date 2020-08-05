---
title: Reading Table Data from MPP files in PHP
type: docs
weight: 100
url: /java/reading-table-data-from-mpp-files-in-php/
---

## **Aspose.Tasks - Reading Table Data from MPP files**
To Read Table Data from MPP files using **Aspose.Tasks Java for PHP**, simply invoke **ReadingTableData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$t1 = $project->getTables()->toList()->get(0);

print "Table Fields Count" . (string)$t1->getTableFields()->size();

$f = $t1->getTableFields()->get(0);

print "Field width: " . (string)$f->getWidth().PHP_EOL;

print "Field Title: " . (string)$f->getTitle().PHP_EOL;

print "Field Title Alignment: " . (string)$f->getAlignTitle().PHP_EOL;

print "Field Align Data: " . $f->getAlignData().PHP_EOL;

$f = $t1->getTableFields()->get(1);

print "Field width: " . (string)$f->getWidth().PHP_EOL;

print "Field Title: " . (string)$f->getTitle().PHP_EOL;

print "Field Title Alignment: " . (string)$f->getAlignTitle().PHP_EOL;

print "Field Align Data: " . (string)$f->getAlignData().PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Reading Table Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ReadingTableData.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithProjects/ReadingTableData.php)
