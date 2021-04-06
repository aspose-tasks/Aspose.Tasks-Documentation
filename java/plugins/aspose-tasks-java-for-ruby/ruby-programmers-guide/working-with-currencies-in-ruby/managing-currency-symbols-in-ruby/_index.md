---
title: Managing Currency Symbols in Ruby
description: "Learn how to deal with work variances in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 30
url: /java/managing-currency-symbols-in-ruby/
---

## **Aspose.Tasks - Getting Currency Symbols**
To get Currency Symbols using **Aspose.Tasks Java for Ruby**, call **get_currency_symbol** method of **CurrencySymbols** module. Here you can see example code.

{{< highlight ruby >}}
def get_currency_symbol()
    project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
    puts "Currency Symbol: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_SYMBOL).to_string
end
{{< /highlight >}}

## **Aspose.Tasks - Setting Currency Symbols**
To set currency symbols using **Aspose.Tasks Java for Ruby**, call **set_currency_symbol** method of **CurrencySymbols** module. Here you can see example code.
{{< highlight ruby >}}
def set_currency_symbol()
    project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
    project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_SYMBOL, "$$")
    project.save("ProjectCurrencySymbols.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)
    puts "Set currency symbol."
end
{{< /highlight >}}

## **Download Running Code**
Download **Managing Currency Symbols (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencysymbols.rb)
