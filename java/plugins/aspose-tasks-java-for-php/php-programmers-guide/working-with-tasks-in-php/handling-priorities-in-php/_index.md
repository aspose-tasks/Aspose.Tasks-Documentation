---
title: Handling Priorities in PHP
type: docs
weight: 60
url: /java/handling-priorities-in-php/
---

## **Aspose.Tasks - Handling Priorities**
To Handle Priorities using **Aspose.Tasks Java for PHP**, simply invoke **HandlingPriorities** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Create a ChildTasksCollector instance

$collector = new ChildTasksCollector();

\# Collect all the tasks from RootTask using TaskUtils

$taskUtils=new TaskUtils();

$taskUtils->apply($project->getRootTask(), $collector, 0);

$tasks = $collector->getTasks();

$tsk = new Tsk();

\# Parse through all the collected tasks

$i = 0;

while ($i < sizeof($tasks)) {

$task = $tasks -> get($i);

print "Priority: " . (string)$task -> get($tsk -> PRIORITY).PHP_EOL;

print "---------------------------------------------".PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Handling Priorities (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/HandlingPriorities.php)
