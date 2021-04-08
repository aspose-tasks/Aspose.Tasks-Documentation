---
title: Managing Currency Codes in Ruby
description: "Learn how to manage currency codes in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/managing-currency-codes-in-ruby/
---

## **Aspose.Tasks - Getting Currency Code**
To get Currency Code using **Aspose.Tasks Java for Ruby**, call **get_currency_code** method of **CurrencyCodes** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
puts "Currency Code: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_CODE).to_string
{{< /highlight >}}

## **Aspose.Tasks - Setting Currency Code**
To set currency code using **Aspose.Tasks Java for Ruby**, call **set_currency_code** method of **CurrencyCodes** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_CODE, "USD")
puts "Set currency code."
{{< /highlight >}}

## **Download Running Code**
Download **Managing Currency Codes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencycodes.rb)
