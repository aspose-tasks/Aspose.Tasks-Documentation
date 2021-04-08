---
title: Managing Currency Digits in Ruby
description: "Learn how to manage Microsoft Project (MPP/XML) currency digits using Aspose.Tasks Java for Ruby."
type: docs
weight: 20
url: /java/managing-currency-digits-in-ruby/
---

## **Aspose.Tasks - Getting Currency Digits**
To get Currency Digits using **Aspose.Tasks Java for Ruby**, call **get_currency_digits** method of **CurrencyDigits** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
puts "Currency Digits: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_DIGITS).to_string
{{< /highlight >}}

## **Aspose.Tasks - Setting Currency Digits**
To set Currency Digits using **Aspose.Tasks Java for Ruby**, call **set_currency_digits** method of **CurrencyDigits** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_DIGITS, 2)
project.save("ProjectCurrencyDigits.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)
puts "Set currency digits."
{{< /highlight >}}

## **Download Running Code**
Download **Managing Currency Digits (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencydigits.rb)
