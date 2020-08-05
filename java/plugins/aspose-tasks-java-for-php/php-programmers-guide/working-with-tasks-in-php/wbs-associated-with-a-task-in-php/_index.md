---
title: WBS Associated with a Task in PHP
type: docs
weight: 170
url: /java/wbs-associated-with-a-task-in-php/
---

## **Aspose.Tasks - WBS Associated with a Task**
To WBS Associated with a Task using **Aspose.Tasks Java for PHP**, simply invoke **WbsAssociatedWithTask** module. Here you can see example code.

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

print "WBS: " . (string)$task -> get($tsk -> WBS).PHP_EOL;

print "WBS Level: " . (string)$task -> get($tsk -> WBS_LEVEL).PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **WBS Associated with a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/WbsAssociatedWithTask.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTasks/WbsAssociatedWithTask.php)
