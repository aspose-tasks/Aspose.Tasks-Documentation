---
title: Read Timephased Data of a Resource in PHP
description: "Learn how to generate or edit timephased data of Microsoft Project (MPP/XML) resources using Aspose.Tasks Java for PHP."
type: docs
weight: 20
url: /java/read-timephased-data-of-a-resource-in-php/
---

## **Aspose.Tasks - Read Timephased Data of a Resource**
To read timephased data of a resource using **Aspose.Tasks Java for PHP**, one can simply invoke **ReadTimephasedResourceData** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource = $project->getResources()->getByUid(1);
$prj = new Prj();
print "Timephased data of Resource Work";
$result = $resource->getTimephasedData($project->get($prj->START_DATE), $project->get($prj->FINISH_DATE))->toList();
$i = 0;
while ($i < sizeof($result)) {
    $td = $result -> get($i);
    print "\nStart: " . (string)$td -> getStart();// . toString()
    print "\nWork: " . (string)$td -> getValue();
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Read Timephased Data of a Resource (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/ReadTimephasedResourceData.php)
