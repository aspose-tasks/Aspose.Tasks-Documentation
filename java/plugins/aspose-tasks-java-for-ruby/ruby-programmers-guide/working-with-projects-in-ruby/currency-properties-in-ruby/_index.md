---
title: Currency Properties in Ruby
description: "Learn how to manage Microsoft Project (MPP/XML) currency properties using Aspose.Tasks Java for Ruby."
type: docs
weight: 20
url: /java/currency-properties-in-ruby/
---

## **Aspose.Tasks - Reading Currency Properties**
To read Currency Properties using **Aspose.Tasks Java for Ruby**, call **get_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
prj = Rjb::import('com.aspose.tasks.Prj')
puts "Currency Code : " + project.get(prj.CURRENCY_CODE).toString()
puts "Currency Digits : " + project.get(prj.CURRENCY_DIGITS).toString()
puts "Currency Symbol : " + project.get(prj.CURRENCY_SYMBOL).toString()
puts "Currency Symbol Position: " + project.get(prj.CURRENCY_SYMBOL_POSITION).toString()
{{< /highlight >}}

## **Aspose.Tasks - Writing Currency Properties**
To write Currency Properties using **Aspose.Tasks Java for Ruby**, call **set_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
prj = Rjb::import('com.aspose.tasks.Prj')
project.set(prj.CURRENCY_CODE, "AUD")
project.set(prj.CURRENCY_DIGITS, 2)
project.set(prj.CURRENCY_SYMBOL, "$")
project.set(prj.CURRENCY_SYMBOL_POSITION, Rjb::import('com.aspose.tasks.CurrencySymbolPositionType').After)
project.save("currency_properties.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Set currency properties, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Currency Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/currencyproperties.rb)
