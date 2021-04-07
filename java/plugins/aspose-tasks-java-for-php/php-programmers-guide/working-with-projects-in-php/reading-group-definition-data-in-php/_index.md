---
title: Reading Group Definition Data in PHP
type: docs
weight: 90
url: /java/reading-group-definition-data-in-php/
---

## **Aspose.Tasks - Reading Group Definition Data**
To Read Group Definition Data using **Aspose.Tasks Java for PHP**, simply invoke **ReadingGroupDefinitionData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}



$project = new Project('test_tasks.mpp');

print "Task Groups Count: " . $project->getTaskGroups()->size().PHP_EOL;

$task_group = $project->getTaskGroups()->toList()->get(0);

print "Percent Complete:" .  (string)$task_group->getName().PHP_EOL;

print "Group Criteria count: " . (string)$task_group->getGroupCriteria()->size().PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Reading Group Definition Data (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ReadingGroupDefinitionData.php)
