---
title: Writing Updated TaskLink Data to MPP in PHP
type: docs
weight: 40
url: /java/writing-updated-tasklink-data-to-mpp-in-php/
---

## **Aspose.Tasks - Writing Updated TaskLink Data to MPP**
To Write Updated TaskLink Data to MPP using **Aspose.Tasks Java for PHP**, simply invoke **UpdateTaskLink** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 $one_sec = 10000000; # microsecond * 10

$one_min = 60 * $one_sec;

$one_hour = 60 * $one_min;

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$tsk = new Tsk();

$prj = new Prj();

\# Add tasks

$task1 = $project->getRootTask()->getChildren()->add("1");

$timeUnitType=new TimeUnitType();

$task1->set($tsk->DURATION, $project->getDuration(8, $timeUnitType->Hour));

$task1->set($tsk->START, $project->get($prj->START_DATE));

$task1->set($tsk->FINISH, $project->get($prj->CALENDAR)->getTaskFinishDateFromDuration($task1,(double)(string)($task1->get($tsk->DURATION))));

$task2 = $project->getRootTask()->getChildren()->add("2");

$task2->set($tsk->DURATION, $project->getDuration(8, $timeUnitType->Hour));

$task2->set($tsk->START, $project->get($prj->START_DATE));

$task2->set($tsk->FINISH, $project->get($prj->CALENDAR)->getTaskFinishDateFromDuration($task2, (double)(string)($task2->get($tsk->DURATION))));

$project->getRootTask()->getChildren()->add($task1);

$project->getRootTask()->getChildren()->add($task2);

\# Add four TaskLinks with different TaskLinkTypes

$taskLinkType=new TaskLinkType();

$link1 = $project->getTaskLinks()->add($task1, $task2, $taskLinkType->StartToStart);


\# Save the Project

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "TaskLinks.mpp", $saveFileFormat->MPP);

print "Saved task links data.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Writing Updated TaskLink Data to MPP (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskLinks/UpdateTaskLink.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTaskLinks/UpdateTaskLink.php)
