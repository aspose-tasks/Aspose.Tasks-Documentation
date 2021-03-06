---
title: Stop and Resume a Task in PHP
description: "Learn how to stop or resume Microsoft Project (MPP/XML) tasks using Aspose.Tasks Java for PHP."
type: docs
weight: 160
url: /java/stop-and-resume-a-task-in-php/
---

## **Aspose.Tasks - Stop and Resume a Task**
To Stop and Resume a Task using **Aspose.Tasks Java for PHP**, simply invoke **StopAndResumeTask** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$collector = new ChildTasksCollector();
$taskUtils = new TaskUtils();
$taskUtils->apply($project->getRootTask(), $collector, 0);
$tasks = $collector->getTasks();
$tsk = new Tsk();
$i = 0;
while ($i < sizeof($tasks)) {
    $task = $tasks->get($i);
    if ((string)$task->get($tsk->STOP) == "1/1/2015")
    {
        print "NA";
    }
    else
    {
        print "Task Stop: " . (string)$task->get($tsk->STOP);
    }
    if ((string)$task->get($tsk->RESUME) == "1/1/2015")
    {
        print "\nNA";
    }
    else
    {
        print "\nTask Resume: " . (string)$task->get($tsk->RESUME);
    }
    print "\n---------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Stop and Resume a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/StopAndResumeTask.php)
