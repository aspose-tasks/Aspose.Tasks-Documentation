---
title: Managing Currency Codes in Ruby
type: docs
weight: 10
url: /java/managing-currency-codes-in-ruby/
---

## **Aspose.Tasks - Getting Currency Code**
To Get Currency Code using **Aspose.Tasks Java for Ruby**, call **get_currency_code** method of **CurrencyCodes** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_currency_code()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    puts "Currency Code: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_CODE).to_string

end

{{< /highlight >}}
## **Aspose.Tasks - Setting Currency Code**
To Set Currency Code using **Aspose.Tasks Java for Ruby**, call **set_currency_code** method of **CurrencyCodes** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def set_currency_code()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_CODE, "USD")

    puts "Set currency code."

end

{{< /highlight >}}
## **Download Running Code**
Download **Managing Currency Codes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencycodes.rb)
