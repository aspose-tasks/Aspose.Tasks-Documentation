---
title: Currency Properties in PHP
type: docs
weight: 20
url: /java/currency-properties-in-php/
---

## **Aspose.Tasks - Reading Currency Properties**
To Read Currency Properties using **Aspose.Tasks Java for PHP**, call **get_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_currency_properties($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$prj = new Prj();

\# Display currency properties

print "Currency Code : " . (string)$project->get($prj->CURRENCY_CODE).PHP_EOL;//.toString()

print "<br>Currency Digits : " . (string)$project->get($prj->CURRENCY_DIGITS).PHP_EOL;//.toString()

print "<br>Currency Symbol : " . (string)$project->get($prj->CURRENCY_SYMBOL).PHP_EOL;//.toString()

print "Currency Symbol Position: ". (string)$project->get($prj->CURRENCY_SYMBOL_POSITION).PHP_EOL;//.toString()

}

{{< /highlight >}}
## **Aspose.Tasks - Writing Currency Properties**
To Write Currency Properties using **Aspose.Tasks Java for PHP**, call **set_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function set_currency_properties($dataDir=null){

\# Instantiate project object

$project = new Project();

$prj = new Prj();

\# Set currency properties

$currencySymbolPositionType=new CurrencySymbolPositionType();

$project->set($prj->CURRENCY_CODE, "AUD");

$project->set($prj->CURRENCY_DIGITS, 2);

$project->set($prj->CURRENCY_SYMBOL, "$");

$project->set($prj->CURRENCY_SYMBOL_POSITION, $currencySymbolPositionType->After);

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "currency_properties.xml", $saveFileFormat->XML);

print "Set currency properties, please check the output file.".PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **Currency Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/CurrencyProperties.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithProjects/CurrencyProperties.php)
