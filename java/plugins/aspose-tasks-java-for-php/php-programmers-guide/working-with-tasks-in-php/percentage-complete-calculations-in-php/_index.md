---
title: Percentage Complete Calculations in PHP
type: docs
weight: 110
url: /java/percentage-complete-calculations-in-php/
---

## **Aspose.Tasks - Percentage Complete Calculations**
To get Complete Percentage Calculations using **Aspose.Tasks Java for PHP**, simply invoke **TasksPercentage** module. Here you can see example code.

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

$tasks = $collector->getTasks();

\# Parse through all the collected tasks

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
Download **Percentage Complete Calculations (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksPercentage.php)
