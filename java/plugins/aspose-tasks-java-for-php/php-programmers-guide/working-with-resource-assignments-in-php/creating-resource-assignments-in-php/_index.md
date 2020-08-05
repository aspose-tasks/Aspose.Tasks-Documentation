---
title: Creating Resource Assignments in Php
type: docs
weight: 30
url: /java/creating-resource-assignments-in-php/
---

## **Aspose.Tasks - Creating Resource Assignments**
To Create Resource Assignments using **Aspose.Tasks Java for PHP**, simply invoke **CreateResourceAssignment** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$task = $project->getRootTask()->getChildren()->add("Task");

$rsc = $project->getResources()->add("Rsc");

$assn = $project->getResourceAssignments()->add($task, $rsc);

print "Created resource assignment.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Creating Resource Assignments (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/CreateResourceAssignment.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithResourceAssignments/CreateResourceAssignment.php)
