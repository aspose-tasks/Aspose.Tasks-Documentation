---
title: Managing Currency Symbols in Ruby
type: docs
weight: 30
url: /java/managing-currency-symbols-in-ruby/
---

## **Aspose.Tasks - Getting Currency Symbols**
To Get Currency Symbols using **Aspose.Tasks Java for Ruby**, call **get_currency_symbol** method of **CurrencySymbols** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_currency_symbol()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    puts "Currency Symbol: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_SYMBOL).to_string

end

{{< /highlight >}}
## **Aspose.Tasks - Setting Currency Symbols**
To Set Currency Symbols using **Aspose.Tasks Java for Ruby**, call **set_currency_symbol** method of **CurrencySymbols** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def set_currency_symbol()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_SYMBOL, "$$")

    project.save(data_dir + "ProjectCurrSymbols.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)

    puts "Set currency symbol."

end

{{< /highlight >}}
## **Download Running Code**
Download **Managing Currency Symbols (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencysymbols.rb)
