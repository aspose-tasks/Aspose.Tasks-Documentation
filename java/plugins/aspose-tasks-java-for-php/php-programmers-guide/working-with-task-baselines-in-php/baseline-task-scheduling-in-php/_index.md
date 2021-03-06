---
title: Baseline Task Scheduling in PHP
description: "Learn how to edit Microsoft Project (MPP/XML) task baselines using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/baseline-task-scheduling-in-php/
---

## **Aspose.Tasks - Baseline Task Scheduling**
To get Baseline Task Scheduling using **Aspose.Tasks Java for PHP**, simply invoke **TaskBaselineSchedule** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$oneSecond = 10000000;
$oneMinute = 60 * $oneSecond;
$oneHour = 60 * $oneMinute;
$project = new Project();
$task = $project->getRootTask()->getChildren()->add("Task");
$baselineType = new BaselineType();
$project->setBaseline($baselineType->Baseline);
$baseline = $task->getBaselines()->toList()->get(0);
$duration = (double)(string)($baseline->getDuration());
$baseline_duration = $duration / $oneHour;
print $baseline_duration;
print "Baseline Start: "  . (string)$baseline->getStart();
print "\nBaseline Finish: " . (string)$baseline->getFinish();
{{< /highlight >}}

## **Download Running Code**
Download **Baseline Task Scheduling (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskBaselines/TaskBaselineSchedule.php)
