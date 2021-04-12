---
title: Handling Overtime, Remaining Costs and Work in PHP
description: "Learn how to handle Microsoft Project (MPP/XML) overtime, remaining and work values using Aspose.Tasks Java for PHP."
type: docs
weight: 60
url: /java/handling-overtime-remaining-costs-and-work-in-php/
---

## **Aspose.Tasks - Handling Overtime, Remaining Costs and Work**
To Handle Overtime, Remaining Costs and Work using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentOvertimeAndRemainingCosts** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource_assignments = $project->getResourceAssignments()->toList();
$asn = new Asn();
$i = 0;
while ($i < sizeof($resource_assignments))
{
    $assignment = $resource_assignments -> get($i);
    print "Overtime Cost: " . $assignment -> get($asn -> OVERTIME_COST).PHP_EOL;
    print "Overtime Work: " . $assignment -> get($asn -> OVERTIME_WORK).PHP_EOL;
    print "Remaining Cost: " . $assignment -> get($asn -> REMAINING_COST).PHP_EOL;
    print "Remaining Overtime Cost: " . $assignment -> get($asn -> REMAINING_OVERTIME_COST).PHP_EOL;
    print "Remaining Overtime Work: " . $assignment -> get($asn -> REMAINING_OVERTIME_WORK).PHP_EOL;
    print "--------------------------------------------------------".PHP_EOL;
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Handling Overtime, Remaining Costs and Work (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentOvertimeAndRemainingCosts.php)
