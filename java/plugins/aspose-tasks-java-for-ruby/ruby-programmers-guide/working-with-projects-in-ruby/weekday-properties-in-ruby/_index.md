---
title: Weekday Properties in Ruby
type: docs
weight: 160
url: /java/weekday-properties-in-ruby/
---

## **Aspose.Tasks - Reading Weekday Properties**
To Read Weekday Properties using **Aspose.Tasks Java for Ruby**, call **get_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
prj = Rjb::import('com.aspose.tasks.Prj')
puts "Week Start Date : " + project.get(prj.WEEK_START_DAY).toString()
puts "Days Per Month : " + project.get(prj.DAYS_PER_MONTH).toString()
puts "Minutes Per Day : " + project.get(prj.MINUTES_PER_DAY).toString()
puts "Minutes Per Week : " + project.get(prj.MINUTES_PER_WEEK).toString()
{{< /highlight >}}

## **Aspose.Tasks - Writing Weekday Properties**
To Write Weekday Properties using **Aspose.Tasks Java for Ruby**, call **set_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
prj = Rjb::import('com.aspose.tasks.Prj')
project.set(prj.WEEK_START_DAY, Rjb::import('com.aspose.tasks.DayType').Monday)
project.set(prj.DAYS_PER_MONTH, 24)
project.set(prj.MINUTES_PER_DAY, 540)
project.set(prj.MINUTES_PER_WEEK, 3240)
project.save("weekday_properties.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Set weekday properties, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Weekday Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/weekdayproperties.rb)
