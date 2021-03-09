---
title: Fiscal Year Properties in PHP
type: docs
weight: 50
url: /java/fiscal-year-properties-in-php/
---

## **Aspose.Tasks - Reading Fiscal Year Properties**
To Read Fiscal Year Properties using **Aspose.Tasks Java for PHP**, call **get_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_fiscal_year_properties($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$prj = new Prj();

\# Display fiscal year properties

print "Fiscal Year Start Date : " . (string)$project->get($prj->FY_START_DATE).PHP_EOL;//.toString();

print "Fiscal Year Numbering : " . (string)$project->get($prj->FISCAL_YEAR_START).PHP_EOL;//.toString()

}

{{< /highlight >}}
## **Aspose.Tasks - Writing Fiscal Year Properties**
To Write Fiscal Year Properties using **Aspose.Tasks Java for PHP**, call **set_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function set_fiscal_year_properties($dataDir=null){

\# Instantiate project object

$project = new Project();

$prj = new Prj();

\# Set fiscal year properties

$month=new Month();

$project->set($prj->FY_START_DATE, $month->July);

$project->set($prj->FISCAL_YEAR_START, new NullableBool(true));

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "fiscal_year_properties.xml", $saveFileFormat->XML);

print "Set fiscal year properties, please check the output file.".PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **Fiscal Year Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/FiscalYearProperties.php)
