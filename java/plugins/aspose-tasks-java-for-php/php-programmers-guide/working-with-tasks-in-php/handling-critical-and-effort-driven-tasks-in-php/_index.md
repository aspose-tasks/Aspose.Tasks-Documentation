---
title: Handling Critical and Effort-driven Tasks in PHP
type: docs
weight: 50
url: /java/handling-critical-and-effort-driven-tasks-in-php/
---

## **Aspose.Tasks - Handling Critical and Effort-driven Tasks**
To Handle Critical and Effort-driven Tasks using **Aspose.Tasks Java for PHP**, simply invoke **CriticalAndEffortDrivenTasks** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Create a ChildTasksCollector instance

$collector = new ChildTasksCollector();

\# Collect all the tasks from RootTask using TaskUtils

$taskUtils=new TaskUtils();

$taskUtils->apply($project->getRootTask(), $collector, 0);

$tsk = new Tsk();

\# Parse through all the collected tasks

$tasks = $collector->getTasks();

$i = 0;

while ($i < sizeof($tasks)) {

$task = $tasks -> get($i);

print $str_ed = $task -> get($tsk -> IS_EFFORT_DRIVEN) != null ? "EffortDriven" : "Non-EffortDriven".PHP_EOL;

print $str_crit = $task -> get($tsk -> IS_CRITICAL) != null ? "Critical" : "Non-Critical".PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Handling Critical and Effort-driven Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/CriticalAndEffortDrivenTasks.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTasks/CriticalAndEffortDrivenTasks.php)
