---
title: Calculating Percentages in PHP
description: "Learn how to calculate percentages in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
type: docs
weight: 20
url: /java/calculating-percentages-in-php/
---

## **Aspose.Tasks - Calculating Percentages**
To Calculate Percentage of the completed work using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentPercentWorkComplete** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource_assignments = $project->getResourceAssignments()->toList();
$i = 0;
$asn = new Asn();
while ($i < sizeof($resource_assignments))
{
    $assignment = $resource_assignments -> get($i);
    print "Percentage of the Completed Work: " . (string)$assignment -> get($asn -> PERCENT_WORK_COMPLETE);
    print "\n--------------------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Calculating Percentages (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentPercentWorkComplete.php)
