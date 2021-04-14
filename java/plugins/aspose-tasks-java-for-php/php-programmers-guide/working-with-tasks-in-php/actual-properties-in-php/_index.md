---
title: Actual Properties in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) actual properties using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/actual-properties-in-php/
---

## **Aspose.Tasks - Getting Actual Properties**
To get Actual Properties using **Aspose.Tasks Java for PHP**, call **get_actual_properties** method of **TasksProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$collector = new ChildTasksCollector();
$taskUtils = new TaskUtils();
$taskUtils->apply($project->getRootTask(), $collector, 0);
$tasks = $collector->getTasks();
$tsk = new Tsk();
$i = 0;
while ($i < sizeof($tasks))
{
    $task = $tasks -> get($i);
    print "Task Name : " . (string)$task -> get($tsk -> NAME);
    print "\nActual Start: " . (string)$task -> get($tsk -> ACTUAL_START);
    print "\nActual Finish: " . (string)$task -> get($tsk -> ACTUAL_FINISH);
    print "\nActual Duration: " . (string)$task -> get($tsk -> ACTUAL_DURATION);
    print "\nActual Cost: " . (string)$task->get($tsk -> ACTUAL_COST);
    print "\n---------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
