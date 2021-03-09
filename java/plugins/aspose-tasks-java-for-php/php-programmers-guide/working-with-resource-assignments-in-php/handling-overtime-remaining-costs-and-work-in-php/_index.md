---
title: Handling Overtime, Remaining Costs and Work in Php
type: docs
weight: 60
url: /java/handling-overtime-remaining-costs-and-work-in-php/
---

## **Aspose.Tasks - Handling Overtime, Remaining Costs and Work**
To Handle Overtime, Remaining Costs and Work using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentOvertimeAndRemainingCosts** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$resource_assignments = $project->getResourceAssignments()->toList();

\# Parse through all the collected resource assignments

$asn=new Asn();

$i = 0;

while ($i < sizeof($resource_assignments)) {

$ra = $resource_assignments -> get($i);

print "Overtime Cost: " . $ra -> get($asn -> OVERTIME_COST).PHP_EOL;

print "Overtime Work: " . $ra -> get($asn -> OVERTIME_WORK).PHP_EOL;

print "Remaining Cost: " . $ra -> get($asn -> REMAINING_COST).PHP_EOL;

print "Remaining Overtime Cost: " . $ra -> get($asn -> REMAINING_OVERTIME_COST).PHP_EOL;

print "Remaining Overtime Work: " . $ra -> get($asn -> REMAINING_OVERTIME_WORK).PHP_EOL;

print "--------------------------------------------------------".PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Handling Overtime, Remaining Costs and Work (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentOvertimeAndRemainingCosts.php)
