---
title: Task Baseline Duration in PHP
type: docs
weight: 30
url: /java/task-baseline-duration-in-php/
---

## **Aspose.Tasks - Task Baseline Duration**
To get Task Baseline Duration using **Aspose.Tasks Java for PHP**, simply invoke **TaskBaselineDuration** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 $onesec = 10000000;

$onemin = 60 * $onesec;

$onehour = 60 * $onemin;

\# Instantiate project object

$project = new Project();

\# Creating TaskBaseline:

$task = $project->getRootTask()->getChildren()->add("Task");

$baselineType=new BaselineType();

$project->setBaseline($baselineType->Baseline);

$baseline = $task->getBaselines()->toList()->get(0);

$duration = (double)(string)($baseline->getDuration());

$baseline_duration = $duration / $onehour;

print $baseline_duration .PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Task Baseline Duration (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskBaselines/TaskBaselineDuration.php)
