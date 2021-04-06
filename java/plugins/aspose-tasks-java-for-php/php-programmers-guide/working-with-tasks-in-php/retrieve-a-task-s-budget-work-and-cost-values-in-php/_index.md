---
title: Retrieve a Task's Budget Work and Cost Values in PHP
type: docs
weight: 150
url: /java/retrieve-a-task-s-budget-work-and-cost-values-in-php/
---

## **Aspose.Tasks - Retrieve a Task's Budget Work and Cost Values**
To Retrieve a Task's Budget Work and Cost Values using **Aspose.Tasks Java for PHP**, simply invoke **GetBudgetWorkAndCostValue** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project($dataDir . 'test_tasks.mpp');

$project_summary = $project->getRootTask();

$tsk = new Tsk();

$rsc = new Rsc();

print "Project Budget Work = " . (string)$project_summary->get($tsk->BUDGET_WORK).PHP_EOL;

print "Project Budget Cost = " . (string)$project_summary->get($tsk->BUDGET_COST).PHP_EOL;

\# Get resource by Uid

$resource = $project->getResources()->getByUid(1);

\# Display resource budget work

print "Resource BudgetWork = " . (string)$resource->get($rsc->BUDGET_WORK).PHP_EOL;

\# Get next resource by Uid

$resource = $project->getResources()->getByUid(2);

\# Display resource budget cost

print "Resource BudgetCost = " . (string)$resource->get($rsc->BUDGET_COST).PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Retrieve a Task's Budget Work and Cost Values (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/GetBudgetWorkAndCostValue.php)
