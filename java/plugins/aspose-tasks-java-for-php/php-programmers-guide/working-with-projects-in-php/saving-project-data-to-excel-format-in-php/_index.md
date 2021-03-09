---
title: Saving Project Data to Excel Format in PHP
type: docs
weight: 130
url: /java/saving-project-data-to-excel-format-in-php/
---

## **Aspose.Tasks - Saving Project Data to Excel Format**
To Save Project Data to Excel Format using **Aspose.Tasks Java for PHP**, simply invoke **SaveProjectDataToExcel** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Save the Project as XLSX

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "Project.XLSX", $saveFileFormat->XLSX);

print "Saved project data to Excel, please check the output file".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Saving Project Data to Excel Format (Aspose.Tasks)** from any of the below mentioned social coding sites:

- GitHub (https:https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/SaveProjectDataToExcel.php)
