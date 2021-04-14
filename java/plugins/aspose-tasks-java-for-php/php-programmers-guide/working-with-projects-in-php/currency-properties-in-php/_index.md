---
title: Currency Properties in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) currency properties using Aspose.Tasks Java for PHP."
type: docs
weight: 20
url: /java/currency-properties-in-php/
---

## **Aspose.Tasks - Reading Currency Properties**
To read Currency Properties using **Aspose.Tasks Java for PHP**, call **get_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
print "Currency Code : " . (string)$project->get($prj->CURRENCY_CODE);
print "\nCurrency Digits : " . (string)$project->get($prj->CURRENCY_DIGITS);
print "\nCurrency Symbol : " . (string)$project->get($prj->CURRENCY_SYMBOL);
print "\nCurrency Symbol Position: ". (string)$project->get($prj->CURRENCY_SYMBOL_POSITION);
{{< /highlight >}}

## **Aspose.Tasks - Writing Currency Properties**
To write Currency Properties using **Aspose.Tasks Java for PHP**, call **set_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$prj = new Prj();
$currencySymbolPositionType = new CurrencySymbolPositionType();
$project->set($prj->CURRENCY_CODE, "AUD");
$project->set($prj->CURRENCY_DIGITS, 2);
$project->set($prj->CURRENCY_SYMBOL, "$");
$project->set($prj->CURRENCY_SYMBOL_POSITION, $currencySymbolPositionType->After);
$saveFileFormat = new SaveFileFormat();
$project->save("currency_properties.xml", $saveFileFormat->XML);
print "Set currency properties, please check the output file.";
{{< /highlight >}}

## **Download Running Code**
Download **Currency Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/CurrencyProperties.php)
