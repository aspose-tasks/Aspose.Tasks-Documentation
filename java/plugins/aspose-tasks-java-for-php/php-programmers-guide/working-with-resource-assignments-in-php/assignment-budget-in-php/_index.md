---
title: Working with Resource Assignment Budgets in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) resource assignment budgets using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/assignment-budget-in-php/
---

## **Aspose.Tasks - Assignment Budget**
To get Assignment Budget using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentBudget** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource_assignments = $project->getResourceAssignments()->toList();
$asn=new Asn();
$i = 0;
while ($i < sizeof($resource_assignments))
{
    $assignment = $resource_assignments->get($i);
    print "Budget Cost: " . (string)$assignment -> get($asn -> BUDGET_COST).PHP_EOL;
    print "Budget Work: " . (string)$assignment -> get($asn -> BUDGET_WORK).PHP_EOL;
    print "--------------------------------------------------------" . PHP_EOL;
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Assignment Budget (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentBudget.php)
