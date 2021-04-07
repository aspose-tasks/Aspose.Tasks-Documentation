---
title: Managing Currency Codes in PHP
type: docs
weight: 10
url: /java/managing-currency-codes-in-php/
---

## **Aspose.Tasks - Getting Currency Code**
To get currency code using **Aspose.Tasks Java for PHP**, call **get_currency_code** method of **CurrencyCodes** module. Here you can see example code.
{{< highlight php >}}
public static function get_currency_code()
{
    $project = new Project('test_tasks.mpp');
    $prj = new Prj();
    print "Currency Code: " . (string)$project->get($prj->CURRENCY_CODE).PHP_EOL;
}
{{< /highlight >}}

## **Aspose.Tasks - Setting Currency Code**
To set currency code using **Aspose.Tasks Java for PHP**, call **set_currency_code** method of **CurrencyCodes** module. Here you can see example code.

{{< highlight php >}}
public static function set_currency_code()
{
    $project = new Project('test_tasks.mpp');
    $prj = new Prj();
    $project->set($prj->CURRENCY_CODE, "USD");
    print "Set currency code.".PHP_EOL;
}
{{< /highlight >}}

## **Download Running Code**
Download **Managing Currency Codes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCurrencies/CurrencyCodes.php)
