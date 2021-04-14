---
title: Calculate Task Duration in Different Units in PHP
description: "Learn how to calculate Microsoft Project (MPP/XML) task durations using Aspose.Tasks Java for PHP."
type: docs
weight: 20
url: /java/calculate-task-duration-in-different-units-in-php/
---

## **Aspose.Tasks - Calculate Task Duration in Different Units**
To Calculate Task Duration in Different Units using **Aspose.Tasks Java for PHP**, simply invoke **CalculateTaskDuration** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$tsk = new Tsk();
$time_unit_type = new TimeUnitType();
$task = $project->getRootTask()->getChildren()->getById(1);
print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Minute))."\n";
print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Day))."\n";
print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Hour))."\n";
print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Week))."\n";
print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Month))."\n";
{{< /highlight >}}

## **Download Running Code**
Download **Calculate Task Duration in Different Units (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/CalculateTaskDuration.php)
