---
title: Fiscal Year Properties in Ruby
type: docs
weight: 50
url: /java/fiscal-year-properties-in-ruby/
---

## **Aspose.Tasks - Reading Fiscal Year Properties**
To Read Fiscal Year Properties using **Aspose.Tasks Java for Ruby**, call **get_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
prj = Rjb::import('com.aspose.tasks.Prj')
puts "Fiscal Year Start Date : " + project.get(prj.FY_START_DATE).toString()
puts "Fiscal Year Numbering : " + project.get(prj.FISCAL_YEAR_START).toString()
{{< /highlight >}}

## **Aspose.Tasks - Writing Fiscal Year Properties**
To Write Fiscal Year Properties using **Aspose.Tasks Java for Ruby**, call **set_fiscal_year_properties** method of **FiscalYearProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
prj = Rjb::import('com.aspose.tasks.Prj')
project.set(prj.FY_START_DATE, Rjb::import('com.aspose.tasks.Month').July)
project.set(prj.FISCAL_YEAR_START, Rjb::import('com.aspose.tasks.NullableBool').new(true))
project.save("fiscal_year_properties.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Set fiscal year properties, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Fiscal Year Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/fiscalyearproperties.rb)
