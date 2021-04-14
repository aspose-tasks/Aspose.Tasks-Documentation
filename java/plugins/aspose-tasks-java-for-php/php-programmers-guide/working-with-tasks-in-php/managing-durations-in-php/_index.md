---
title: Managing Task Durations in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) task durations using Aspose.Tasks Java for PHP."
type: docs
weight: 70
url: /java/managing-durations-in-php/
---

## **Aspose.Tasks - Managing Durations**
To manage durations using **Aspose.Tasks Java for PHP**, simply invoke **ManagingDuration** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$task = $project->getRootTask()->getChildren()->add("Task");
$tsk = new Tsk();
$duration = $task->get($tsk->DURATION);
print "Duration in Days: " . $duration->toString();
$timeUnitType = new TimeUnitType();
$duration = $duration->convert($timeUnitType->Hour);
print "Duration in Hours: ". (string)$duration;
$task->set($tsk->DURATION, $task->get($tsk->DURATION)->subtract(0.5));
print "\n0.5 weeks: " . (string)$task->get($tsk->DURATION);
{{< /highlight >}}

## **Download Running Code**
Download **Managing Durations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/ManagingDuration.php)
