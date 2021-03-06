---
title: Predecessor and Successor Tasks in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) predecessor and successor tasks using Aspose.Tasks Java for PHP."
type: docs
weight: 30
url: /java/predecessor-and-successor-tasks-in-php/
---

## **Aspose.Tasks - Predecessor and Successor Tasks**
To get Predecessor and Successor Tasks using **Aspose.Tasks Java for PHP**, simply invoke **PredecessorAndSuccessorTask** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$tsk = new Tsk();
$allLinks = $project->getTaskLinks()->toList();
$i = 0;
while ($i < sizeof($allLinks)) {
    $tskLink = $allLinks -> get($i);
    print "Predecessor " . (string)$tskLink -> getPredTask() -> get($tsk-> NAME);
    print "\nSuccessor " . (string)$tskLink -> getSuccTask() -> get($tsk -> NAME);
    print "\n------------------------------------------------------";
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Predecessor and Successor Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskLinks/PredecessorAndSuccessorTask.php)
