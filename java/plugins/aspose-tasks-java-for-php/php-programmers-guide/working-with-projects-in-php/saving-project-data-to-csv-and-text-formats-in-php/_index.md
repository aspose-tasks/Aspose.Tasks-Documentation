---
title: Saving Project Data to CSV and Text Formats in PHP
type: docs
weight: 120
url: /java/saving-project-data-to-csv-and-text-formats-in-php/
---

## **Aspose.Tasks - Saving a Project as CSV**
To Save a Project as CSV using **Aspose.Tasks Java for PHP**, call **save_to_csv** method of **SaveProjectDataToOtherFormats** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function save_to_csv($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Save the Project as CSV

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "Project.csv", $saveFileFormat->CSV);

print "Saved project data to CSV, please check the output file".PHP_EOL;

}

{{< /highlight >}}
## **Aspose.Tasks - Saving a Project as Text**
To Save a Project as Text using **Aspose.Tasks Java for PHP**, call **save_to_text** method of **SaveProjectDataToOtherFormats** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function save_to_text($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Save the Project as Text

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "Project.txt", $saveFileFormat->TXT);

print "Saved project data to Text, please check the output file".PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **Saving Project Data to CSV and Text Formats (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/SaveProjectDataToOtherFormats.php)
