---
title: Assignment Budget in Php
type: docs
weight: 10
url: /java/assignment-budget-in-php/
---

## **Aspose.Tasks - Assignment Budget**
To Get Assignment Budget using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentBudget** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$resource_assignments = $project->getResourceAssignments()->toList();

\# Parse through all the collected resource assignments

$asn=new Asn();

$i = 0;

while ($i < sizeof($resource_assignments)){

$ra = $resource_assignments->get($i);

print "Buget Cost: " . (string)$ra -> get($asn -> BUDGET_COST).PHP_EOL;

print "Buget Work: " . (string)$ra -> get($asn -> BUDGET_WORK).PHP_EOL;

print "--------------------------------------------------------" . PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Assignment Budget (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentBudget.php)
