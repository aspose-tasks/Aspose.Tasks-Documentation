---
title: Predecessor and Successor Tasks in PHP
type: docs
weight: 30
url: /java/predecessor-and-successor-tasks-in-php/
---

## **Aspose.Tasks - Predecessor and Successor Tasks**
To get Predecessor and Successor Tasks using **Aspose.Tasks Java for PHP**, simply invoke **PredecessorAndSuccessorTask** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$tsk = new Tsk();

$allinks = $project->getTaskLinks()->toList();

$i = 0;

while ($i < sizeof($allinks)) {

$tsklnk = $allinks -> get($i);

print "Predecessor " . (string)$tsklnk -> getPredTask() -> get($tsk-> NAME).PHP_EOL;

print "Successor " . (string)$tsklnk -> getSuccTask() -> get($tsk -> NAME).PHP_EOL;

print "------------------------------------------------------".PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Predecessor and Successor Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskLinks/PredecessorAndSuccessorTask.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithTaskLinks/PredecessorAndSuccessorTask.php)
