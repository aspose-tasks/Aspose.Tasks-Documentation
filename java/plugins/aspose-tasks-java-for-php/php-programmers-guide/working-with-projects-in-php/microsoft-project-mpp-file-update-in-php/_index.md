---
title: Microsoft Project MPP File Update in PHP
type: docs
weight: 80
url: /java/microsoft-project-mpp-file-update-in-php/
---

## **Aspose.Tasks - Update Project File**
To Update Project File using **Aspose.Tasks Java for PHP**, simply invoke **UpdateProjectFile** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# create a new task

$task = $project->getRootTask()->getChildren()->add("Task1");

\# set start date

$cal=new Calendar();

$cal = $cal->getInstance();

$cal->set(2015, 7, 1, 8, 0,0);

$tsk=new Tsk();

$task->set($tsk->START, $cal->getTime());

$cal->set(2015, 7, 1, 17, 0, 0);

$task->set($tsk->FINISH , $cal->getTime());

\# Save the project as MPP project file

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "AfterLinking.mpp", $saveFileFormat->MPP);

print "Project file updated, please check the output file.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Update Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/UpdateProjectFile.php)
