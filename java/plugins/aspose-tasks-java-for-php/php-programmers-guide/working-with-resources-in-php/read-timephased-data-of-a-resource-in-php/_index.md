---
title: Read Timephased Data of a Resource in PHP
type: docs
weight: 20
url: /java/read-timephased-data-of-a-resource-in-php/
---

## **Aspose.Tasks - Read Timephased Data of a Resource**
To Read Timephased Data of a Resource using **Aspose.Tasks Java for PHP**, simply invoke **ReadTimephasedResourceData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}


$project = new Project($dataDir . 'test_tasks.mpp');

\# Get the Resource by its ID

$resource = $project->getResources()->getByUid(1);

$prj = new Prj();

\# Print Timephased data of ResourceWork

print "Timephased data of Resource Work".PHP_EOL;

$result = $resource->getTimephasedData($project->get($prj->START_DATE), $project->get($prj->FINISH_DATE))->toList();

$i = 0;

while ($i < sizeof($result)) {

$td = $result -> get($i);

print "Start: " . (string)$td -> getStart().PHP_EOL;// . toString()

print "Work: " . (string)$td -> getValue().PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Read Timephased Data of a Resource (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/ReadTimephasedResourceData.php)
