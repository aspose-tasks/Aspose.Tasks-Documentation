---
title: General Properties in PHP
description: "Learn how to read Microsoft Project (MPP/XML) general properties using Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/general-properties-in-php/
---

## **Aspose.Tasks - Getting General Properties**
To get General Properties using **Aspose.Tasks Java for PHP**, call **get_general_properties** method of **TasksProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$collector = new ChildTasksCollector();
$taskUtils = new TaskUtils();
$taskUtils->apply($project->getRootTask(), $collector, 0);
$tasks = $collector->getTasks();
puts tasks.size()
$tsk = new Tsk();
$i = 0;
while ($i < sizeof($tasks))
{
    $task = $tasks -> get($i);
    print "Task Id:" . $task -> get($tsk -> ID);
    print "\nTask Uid: " . $task -> get($tsk -> UID);
    print "\nTask Name: " . $task -> get($tsk -> NAME);
    print "\nTask Start: " . $task -> get($tsk -> START);
    print "\nTask Finish: " . $task -> get($tsk -> FINISH);
    print "\n---------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
