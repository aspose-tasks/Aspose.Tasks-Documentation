---
title: Change Progress of a Task in PHP
type: docs
weight: 30
url: /java/change-progress-of-a-task-in-php/
---

## **Aspose.Tasks - Change Progress of a Task**
To Change Progress of a Task presentation using **Aspose.Tasks Java for PHP**, simply invoke **ChangeProgressOfTask** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project();

print $project->getCalculationMode();

$task = $project->getRootTask()->getChildren()->add("Task");

$tsk = new Tsk();

$task->set($tsk->DURATION, $project->getDuration(2));

$task->set($tsk->PERCENT_COMPLETE, 50);

print "Changed progress of task.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Change Progress of a Task (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/ChangeProgressOfTask.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTasks/ChangeProgressOfTask.php)
