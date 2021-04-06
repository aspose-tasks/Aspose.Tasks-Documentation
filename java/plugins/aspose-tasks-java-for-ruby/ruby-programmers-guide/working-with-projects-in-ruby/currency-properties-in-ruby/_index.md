---
title: Currency Properties in Ruby
type: docs
weight: 20
url: /java/currency-properties-in-ruby/
---

## **Aspose.Tasks - Reading Currency Properties**
To Read Currency Properties using **Aspose.Tasks Java for Ruby**, call **get_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_currency_properties()

        data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



       

        project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

        prj = Rjb::import('com.aspose.tasks.Prj')

        # Display currency properties

        puts "Currency Code : " + project.get(prj.CURRENCY_CODE).toString()

        puts "<br>Currency Digits : " + project.get(prj.CURRENCY_DIGITS).toString()

        puts "<br>Currency Symbol : " + project.get(prj.CURRENCY_SYMBOL).toString()

        puts "Currency Symbol Position: " + project.get(prj.CURRENCY_SYMBOL_POSITION).toString()

    end

{{< /highlight >}}
## **Aspose.Tasks - Writing Currency Properties**
To Write Currency Properties using **Aspose.Tasks Java for Ruby**, call **set_currency_properties** method of **CurrencyProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def set_currency_properties()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new

    prj = Rjb::import('com.aspose.tasks.Prj')

    # Set currency properties

    project.set(prj.CURRENCY_CODE, "AUD")

    project.set(prj.CURRENCY_DIGITS, 2)

    project.set(prj.CURRENCY_SYMBOL, "$")

    project.set(prj.CURRENCY_SYMBOL_POSITION, Rjb::import('com.aspose.tasks.CurrencySymbolPositionType').After)

    project.save(data_dir + "currency_properties.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)

    puts "Set currency properties, please check the output file."

end

{{< /highlight >}}
## **Download Running Code**
Download **Currency Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/currencyproperties.rb)
