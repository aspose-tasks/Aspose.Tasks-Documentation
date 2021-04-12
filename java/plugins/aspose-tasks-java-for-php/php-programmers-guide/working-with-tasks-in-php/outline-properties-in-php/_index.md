---
title: Outline Properties in PHP
description: "Learn how to work Microsoft Project (MPP/XML) outline values using Aspose.Tasks Java for PHP."
type: docs
weight: 90
url: /java/outline-properties-in-php/
---

## **Aspose.Tasks - Getting Outline Properties**
To get Outline Properties using **Aspose.Tasks Java for PHP**, call **get_outline_properties** method of **TasksProperties** module. Here you can see example code.

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
    $task=$tasks->get($i);
    print "Outline Level: " . (string)$task->get($tsk -> OUTLINE_LEVEL).PHP_EOL;
    print "Outline Number: " . (string)$task->get($tsk -> OUTLINE_NUMBER).PHP_EOL;
    print "---------------------------------------------".PHP_EOL;
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
