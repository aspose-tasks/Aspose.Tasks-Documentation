---
title: Handling Critical and Effort-driven Tasks in PHP
description: "Learn how to handle Microsoft Project (MPP/XML) critical and effort-driven tasks using Aspose.Tasks Java for PHP."
type: docs
weight: 50
url: /java/handling-critical-and-effort-driven-tasks-in-php/
---

## **Aspose.Tasks - Handling Critical and Effort-driven Tasks**
To Handle Critical and Effort-driven Tasks using **Aspose.Tasks Java for PHP**, simply invoke **CriticalAndEffortDrivenTasks** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$collector = new ChildTasksCollector();
$taskUtils = new TaskUtils();
$taskUtils->apply($project->getRootTask(), $collector, 0);
$tsk = new Tsk();
$tasks = $collector->getTasks();
$i = 0;
while ($i < sizeof($tasks))
{
    $task = $tasks -> get($i);
    print $str_effort_driven = $task -> get($tsk -> IS_EFFORT_DRIVEN) != null ? "\nEffortDriven" : "\nNon-EffortDriven";
    print $str_is_critical = $task -> get($tsk -> IS_CRITICAL) != null ? "\nCritical" : "\nNon-Critical";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Handling Critical and Effort-driven Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/CriticalAndEffortDrivenTasks.php)
