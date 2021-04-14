---
title: Working with Filter Data from MPP files in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) project filters using Aspose.Tasks Java for PHP."
type: docs
weight: 170
url: /java/working-with-filter-data-from-mpp-files-in-php/
---

## **Aspose.Tasks - Reading Filter Definition Data**
To read Filter Definition Data using **Aspose.Tasks Java for PHP**, call **get_filter_definition_data** method of **FilterData** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$task_filters = $project->getTaskFilters()->toList();
print "Task Filters Count: " . (string)$task_filters->size();
print "\nAll Tasks: " . (string)$task_filters->get(0)->getName();
print "\nTask Item: " . (string)$task_filters->get(0)->getFilterType();
print "\nTask Filters Show In Menu: " . (string)$task_filters->get(0)->getShowInMenu();
print "\nTask filter ShowRelatedSummaryRows: "  . (string)$task_filters->get(0)->getShowRelatedSummaryRows();
$rsc_filters = $project->getResourceFilters()->toList();
print "\nProject.ResourceFilters count: " .  (string)$rsc_filters->size();
print "\nResource Filter Item Type: Item.ResourceType: "  . (string)$rsc_filters->get(0)->getFilterType();
print "\nResource filter ShowInMenu"  . (string)$rsc_filters->get(0)->getShowInMenu();
print "\nResource filter ShowRelatedSummaryRows: " . (string)$rsc_filters->get(0)->getShowRelatedSummaryRows();
{{< /highlight >}}

## **Download Running Code**
Download **Working with Filter Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/FilterData.php)
