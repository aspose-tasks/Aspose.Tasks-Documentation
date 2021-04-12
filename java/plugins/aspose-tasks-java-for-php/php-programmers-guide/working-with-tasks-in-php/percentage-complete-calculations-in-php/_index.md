---
title: Percentage Complete Calculations in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) percentage complete values using Aspose.Tasks Java for PHP."
type: docs
weight: 110
url: /java/percentage-complete-calculations-in-php/
---

## **Aspose.Tasks - Percentage Complete Calculations**
To get Complete Percentage Calculations using **Aspose.Tasks Java for PHP**, simply invoke **TasksPercentage** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$collector = new ChildTasksCollector();
$taskUtils = new TaskUtils();
$taskUtils->apply($project->getRootTask(), $collector, 0);
$tsk = new Tsk();
$tasks = $collector->getTasks();
$i = 0;
while ($i < sizeof($tasks)) {
    $task = $tasks -> get($i);
    print (string)$task -> get($tsk -> PERCENT_COMPLETE).PHP_EOL;
    print (string)$task -> get($tsk -> PERCENT_WORK_COMPLETE).PHP_EOL;
    print (string)$task -> get($tsk -> PHYSICAL_PERCENT_COMPLETE).PHP_EOL;
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Percentage Complete Calculations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksPercentage.php)
