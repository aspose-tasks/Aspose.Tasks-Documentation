---
title: Creating an Empty Project File in PHP
type: docs
weight: 10
url: /java/creating-an-empty-project-file-in-php/
---

## **Aspose.Tasks - Creating an Empty Project File**
To create an Empty Project File using **Aspose.Tasks Java for PHP**, simply invoke **CreateEmptyProject** module. Here you can see example code.

{{< highlight php >}}
$project = new Project();
$project_stream =  new FileOutputStream("Project1.xml");
$saveFileFormat = new SaveFileFormat();
$project->save($project_stream, $saveFileFormat->XML);
$project_stream->close();
print "Created project Successfully.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Creating an Empty Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/CreateEmptyProject.php)
