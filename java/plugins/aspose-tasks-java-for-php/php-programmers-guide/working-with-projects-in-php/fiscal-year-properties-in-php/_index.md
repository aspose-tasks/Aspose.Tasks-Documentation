---
title: Fiscal Year Properties in PHP
description: "Learn how to get Microsoft Project (MPP/XML) fiscal year properties using Aspose.Tasks Java for PHP."
type: docs
weight: 50
url: /java/fiscal-year-properties-in-php/
---

## **Aspose.Tasks - Reading Fiscal Year Properties**
To read Fiscal Year Properties using **Aspose.Tasks Java for PHP**, call **get_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
print "Fiscal Year Start Date : " . (string)$project->get($prj->FY_START_DATE).PHP_EOL;//.toString();
print "Fiscal Year Numbering : " . (string)$project->get($prj->FISCAL_YEAR_START).PHP_EOL;//.toString()
{{< /highlight >}}

## **Aspose.Tasks - Writing Fiscal Year Properties**
To write Fiscal Year Properties using **Aspose.Tasks Java for PHP**, call **set_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$prj = new Prj();
$month = new Month();
$project->set($prj->FY_START_DATE, $month->July);
$project->set($prj->FISCAL_YEAR_START, new NullableBool(true));
$saveFileFormat = new SaveFileFormat();
$project->save("fiscal_year_properties.xml", $saveFileFormat->XML);
print "Set fiscal year properties, please check the output file.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Fiscal Year Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/FiscalYearProperties.php)
