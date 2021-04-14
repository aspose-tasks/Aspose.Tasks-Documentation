---
title: Creating Resource Assignments in PHP
description: "Learn how to create resource assignments linking tasks and resources in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
type: docs
weight: 30
url: /java/creating-resource-assignments-in-php/
---

## **Aspose.Tasks - Creating Resource Assignments**
To create resource assignments using **Aspose.Tasks Java for PHP**, simply invoke **CreateResourceAssignment** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$task = $project->getRootTask()->getChildren()->add("Task");
$rsc = $project->getResources()->add("Rsc");
$assignment = $project->getResourceAssignments()->add($task, $rsc);
print "Created resource assignment.";
{{< /highlight >}}

## **Download Running Code**
Download **Creating Resource Assignments (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/CreateResourceAssignment.php)
