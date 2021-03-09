---
title: General Properties in PHP
type: docs
weight: 40
url: /java/general-properties-in-php/
---

## **Aspose.Tasks - Getting General Properties**
To Get General Properties using **Aspose.Tasks Java for PHP**, call **get_general_properties** method of **TasksProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_general_properties($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Create a ChildTasksCollector instance

$collector = new ChildTasksCollector();

\# Collect all the tasks from RootTask using TaskUtils

$taskUtils=new TaskUtils();

$taskUtils->apply($project->getRootTask(), $collector, 0);

$tasks = $collector->getTasks();

#puts tasks.size()

#abort()

$tsk = new Tsk();

\# Parse through all the collected tasks

#tasks.each do |task|

$i = 0;

while ($i < sizeof($tasks)) {

$task = $tasks -> get($i);

print "Task Id:" . $task -> get($tsk -> ID).PHP_EOL;

print "Task Uid: " . $task -> get($tsk -> UID).PHP_EOL;

print "Task Name: " . $task -> get($tsk -> NAME).PHP_EOL;

print "Task Start: " . $task -> get($tsk -> START).PHP_EOL;

print "Task Finish: " . $task -> get($tsk -> FINISH).PHP_EOL;

print "---------------------------------------------".PHP_EOL;

$i += 1;

}

}

{{< /highlight >}}
## **Download Running Code**
Download **General Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/TasksProperties.php)
