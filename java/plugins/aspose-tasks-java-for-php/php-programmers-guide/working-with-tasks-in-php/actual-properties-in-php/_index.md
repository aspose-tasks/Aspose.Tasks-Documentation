---
title: Actual Properties in PHP
type: docs
weight: 10
url: /java/actual-properties-in-php/
---

## **Aspose.Tasks - Getting Actual Properties**
To Get Actual Properties using **Aspose.Tasks Java for PHP**, call **get_actual_properties** method of **TasksProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_actual_properties($dataDir=null){

\# Instantiate project object

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

print "Task Name : " . (string)$task -> get($tsk -> NAME).PHP_EOL;

print "Actual Start: " . (string)$task -> get($tsk -> ACTUAL_START).PHP_EOL;

print "Actual Finish: " . (string)$task -> get($tsk -> ACTUAL_FINISH).PHP_EOL;

print "Actual Duration: " . (string)$task -> get($tsk -> ACTUAL_DURATION).PHP_EOL;

print "Actual Cost: " . (string)$task->get($tsk -> ACTUAL_COST).PHP_EOL;

print "---------------------------------------------".PHP_EOL;

$i += 1;

}

}

{{< /highlight >}}
## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
