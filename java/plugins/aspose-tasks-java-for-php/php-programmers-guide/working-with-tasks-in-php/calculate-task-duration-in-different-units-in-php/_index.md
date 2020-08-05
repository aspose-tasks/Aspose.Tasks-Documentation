---
title: Calculate Task Duration in Different Units in PHP
type: docs
weight: 20
url: /java/calculate-task-duration-in-different-units-in-php/
---

## **Aspose.Tasks - Calculate Task Duration in Different Units**
To Calculate Task Duration in Different Units using **Aspose.Tasks Java for PHP**, simply invoke **CalculateTaskDuration** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$tsk = new Tsk();

$time_unit_type = new TimeUnitType();

\# Get a task to calculate its duration in different formats

$task = $project->getRootTask()->getChildren()->getById(1);

\# Get the duration in Minutes

print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Minute)).PHP_EOL;

\# Get the duration in Days

print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Day)).PHP_EOL;

\# Get the duration in Hours

print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Hour)).PHP_EOL;

\# Get the duration in Weeks

print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Week)).PHP_EOL;

\# Get the duration in Months

print (double)(string)($task->get($tsk->DURATION)->convert($time_unit_type->Month)).PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Calculate Task Duration in Different Units (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/CalculateTaskDuration.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTasks/CalculateTaskDuration.php)
