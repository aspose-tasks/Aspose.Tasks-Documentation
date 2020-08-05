---
title: Working with Filter Data from MPP files in PHP
type: docs
weight: 170
url: /java/working-with-filter-data-from-mpp-files-in-php/
---

## **Aspose.Tasks - Reading Filter Definition Data**
To Read Filter Definition Data using **Aspose.Tasks Java for PHP**, call **get_filter_definition_data** method of **FilterData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_filter_definition_data($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$task_filters = $project->getTaskFilters()->toList();

print "Task Filters Count: " . (string)$task_filters->size().PHP_EOL;

print "All Tasks: " . (string)$task_filters->get(0)->getName().PHP_EOL;

print "Task Item: " . (string)$task_filters->get(0)->getFilterType().PHP_EOL;

print "Task Filters Show In Menu: " . (string)$task_filters->get(0)->getShowInMenu().PHP_EOL;

print "Task filter ShowRelatedSummaryRows: "  . (string)$task_filters->get(0)->getShowRelatedSummaryRows().PHP_EOL;

$rsc_filters = $project->getResourceFilters()->toList();

print "Project.ResourceFilters count: " .  (string)$rsc_filters->size().PHP_EOL;

print "Resource Filter Item Type: Item.ResourceType: "  . (string)$rsc_filters->get(0)->getFilterType().PHP_EOL;

print "Resource filter ShowInMenu"  . (string)$rsc_filters->get(0)->getShowInMenu().PHP_EOL;

print "Resource filter ShowRelatedSummaryRows: " . (string)$rsc_filters->get(0)->getShowRelatedSummaryRows().PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **Working with Filter Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/FilterData.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithProjects/FilterData.php)
