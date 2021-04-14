---
title: Managing Task Costs in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) task costs using Aspose.Tasks Java for PHP."
type: docs
weight: 80
url: /java/managing-task-costs-in-php/
---

## **Aspose.Tasks - Managing Task Costs**
To manage Task Costs using **Aspose.Tasks Java for PHP**, simply invoke **ManagingTaskCosts** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$task = $project->getRootTask()->getChildren()->add("Task");
$tsk = new Tsk();
$bigDecimal = new BigDecimal();
$task->set($tsk->COST, $bigDecimal->valueOf(800));
print "Task Remaining Cost: " . (string)$task->get($tsk->REMAINING_COST);
print "\nTask Fixed Cost: " . (string)$task->get($tsk->FIXED_COST);
print "\nTask Cost Variance: " . (string)$task->get($tsk->COST_VARIANCE);
print "\nProject Cost: " . (string)$project->getRootTask()->get($tsk->COST);
print "\nProject Fixed Cost: " . (string)$project->getRootTask()->get($tsk->FIXED_COST);
print "\nProject Remaining Cost: " . (string)$project->getRootTask()->get($tsk->REMAINING_COST);
print "\nProject Variance Cost: " . (string)$project->getRootTask()->get($tsk->COST_VARIANCE);
{{< /highlight >}}

## **Download Running Code**
Download **Managing Task Costs (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/ManagingTaskCosts.php)
