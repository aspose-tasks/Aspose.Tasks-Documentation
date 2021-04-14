---
title: Reading Group Definition Data in PHP
description: "This article explains how to read group definition data from Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
type: docs
weight: 90
url: /java/reading-group-definition-data-in-php/
---

## **Aspose.Tasks - Reading Group Definition Data**
To read Group Definition Data using **Aspose.Tasks Java for PHP**, simply invoke **ReadingGroupDefinitionData** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
print "Task Groups Count: " . $project->getTaskGroups()->size();
$task_group = $project->getTaskGroups()->toList()->get(0);
print "\nPercent Complete:" .  (string)$task_group->getName();
print "\nGroup Criteria count: " . (string)$task_group->getGroupCriteria()->size();
{{< /highlight >}}

## **Download Running Code**
Download **Reading Group Definition Data (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ReadingGroupDefinitionData.php)
