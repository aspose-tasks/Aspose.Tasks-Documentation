---
title: Managing Assignment Cost in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) resource assignment costs using Aspose.Tasks Java for PHP."
type: docs
weight: 70
url: /java/managing-assignment-cost-in-php/
---

## **Aspose.Tasks - Managing Assignment Cost**
To manage Assignment Cost using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentCost** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource_assignments = $project->getResourceAssignments()->toList();
$asn = new Asn();
$i = 0;
while ($i < sizeof($resource_assignments))
{
    $assignment = $resource_assignments -> get($i);
    print "COST: " . (string)$assignment -> get($asn -> COST);
    print "\nACWP: " . (string)$assignment -> get($asn -> ACWP);
    print "\nBCWP: " . (string)$assignment -> get($asn -> BCWP);
    print "\nBCWS: " . (string)$assignment -> get($asn -> BCWS);
    print "\n--------------------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Managing Assignment Cost (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentCost.php)
