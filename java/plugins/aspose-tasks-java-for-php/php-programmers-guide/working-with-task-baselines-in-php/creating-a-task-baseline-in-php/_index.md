---
title: Creating a Task Baseline in PHP
type: docs
weight: 20
url: /java/creating-a-task-baseline-in-php/
---

## **Aspose.Tasks - Creating a Task Baseline**
To Create a Task Baseline using **Aspose.Tasks Java for PHP**, simply invoke **CreateTaskBaseline** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Set baseline for the entire project

$baselineType=new BaselineType();

$project->setBaseline($baselineType->Baseline);

print "Set baseline for the project.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Creating a Task Baseline (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskBaselines/CreateTaskBaseline.php)
