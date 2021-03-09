---
title: Parent and Child Tasks in PHP
type: docs
weight: 100
url: /java/parent-and-child-tasks-in-php/
---

## **Aspose.Tasks - Getting Parent and Child Tasks**
To Get Parent and Child Tasks using **Aspose.Tasks Java for PHP**, call **get_parent_and_child_tasks** method of **ParentAndChildTasks** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_parent_and_child_tasks($dataDir=null)

{

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Create a ChildTasksCollector instance

$collector = new ChildTasksCollector();

\# Collect all the tasks from RootTask using TaskUtils

$taskUtils = new TaskUtils();

$taskUtils->apply($project->getRootTask(), $collector, 0);

$tsk = new Tsk();

$tasks = $collector->getTasks();

\# Parse through all the collected tasks

$i = 0;

while ($i < sizeof($tasks)){

$task = $tasks->get($i);

print "Task Name = " . (string)$task->get($tsk->NAME);//.to_string

$i+= 1;

}

}

{{< /highlight >}}
## **Download Running Code**
Download **Parent and Child Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/ParentAndChildTasks.php)
