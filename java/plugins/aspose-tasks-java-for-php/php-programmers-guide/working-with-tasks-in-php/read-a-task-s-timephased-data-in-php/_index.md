---
title: Read a Task's Timephased Data in PHP
type: docs
weight: 120
url: /java/read-a-task-s-timephased-data-in-php/
---

## **Aspose.Tasks - Read a Task's Timephased Data**
To read a Task's Timephased Data using **Aspose.Tasks Java for PHP**, simply invoke **GetTaskTimephasedData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
$tsk = new Tsk();
$cal = new Calendar();
$cal = $cal->getInstance();
$cal->set(2013,7,17,8,0,0);
$project->set($prj->START_DATE, $cal->getTime());
$project->set($prj->NEW_TASKS_ARE_MANUAL, new NullableBool(false));
$task = $project->getRootTask()->getChildren()->add("Task");
$rsc = $project->getResources()->add("Rsc");
$resource = new Rsc();
$bigDecimal = new BigDecimal();
$rsc->set($resource->STANDARD_RATE, $bigDecimal->valueOf(10));
$rsc->set($resource->OVERTIME_RATE, $bigDecimal->valueOf(15));
$task->set($tsk->DURATION, $project->getDuration(6));
$assignment = $project->getResourceAssignments()->add($task, $rsc);
$d = new Date(0);
$assignment = new Asn();
$assignment->set($assignment->STOP, new Date(0));
$assignment->set($assignment->RESUME, new Date(0));
$workContourType = new WorkContourType();
$assignment->set($assignment->WORK_CONTOUR, $workContourType->BackLoaded);
$baselineType = new BaselineType();
$project->setBaseline($baselineType->Baseline);
$task->set($tsk->PERCENT_COMPLETE, 50);
$timephasedDataType = new TimephasedDataType();
$td = $assignment->getTimephasedData($assignment->get($assignment->START),
$assignment->get($assignment->FINISH),
$timephasedDataType->AssignmentRemainingWork)->toList();
print "Size: " . (string)$td->size().PHP_EOL;
print "Value: " . (string)$td->get(0)->getValue().PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Read a Task's Timephased Data (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTasks/GetTaskTimephasedData.php)
