---
title: Managing Currency Digits in Ruby
type: docs
weight: 20
url: /java/managing-currency-digits-in-ruby/
---

## **Aspose.Tasks - Getting Currency Digits**
To Get Currency Digits using **Aspose.Tasks Java for Ruby**, call **get_currency_digits** method of **CurrencyDigits** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_currency_digits()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'

    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    puts "Currency Digits: " + project.get(Rjb::import('com.aspose.tasks.Prj').CURRENCY_DIGITS).to_string

end

{{< /highlight >}}
## **Aspose.Tasks - Setting Currency Digits**
To Set Currency Digits using **Aspose.Tasks Java for Ruby**, call **set_currency_digits** method of **CurrencyDigits** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def set_currency_digits()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'

    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    project.set(Rjb::import('com.aspose.tasks.Prj').CURRENCY_DIGITS, 2)

    project.save(data_dir + "ProjectCurrDigits.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)

    puts "Set currency digits."

end

{{< /highlight >}}
## **Download Running Code**
Download **Managing Currency Digits (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Currencies/currencydigits.rb)
