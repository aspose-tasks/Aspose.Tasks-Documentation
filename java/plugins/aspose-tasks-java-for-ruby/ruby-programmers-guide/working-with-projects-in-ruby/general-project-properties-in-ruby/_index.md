---
title: General Project Properties in Ruby
description: "Learn how to manage Microsoft Project (MPP/XML) general properties using Aspose.Tasks Java for Ruby."
type: docs
weight: 60
url: /java/general-project-properties-in-ruby/
---

## **Aspose.Tasks - General Project Properties**
To get General Project Properties using **Aspose.Tasks Java for Ruby**, call **get_general_project_properties** method of **ProjectProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('Sample.xml')
prj = Rjb::import('com.aspose.tasks.Prj')
if project.get(prj.SCHEDULE_FROM_START).getValue()
    puts "Project Start Date : " + project.get(prj.START_DATE).to_string
else
    puts "Project Finish Date : " + project.get(prj.FINISH_DATE).to_string
end
strSchedule = project.get(prj.SCHEDULE_FROM_START).getValue() ? "Project Start Date" : "Project Finish Date"
puts "Project Schedule From : " + strSchedule.to_s
puts "Current Date : " + project.get(prj.CURRENT_DATE).to_string
puts "Status Date : " + project.get(prj.STATUS_DATE).to_string
puts "Calendar : " + project.get(prj.CALENDAR).getName().to_s
{{< /highlight >}}

## **Download Running Code**
Download **General Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/projectproperties.rb)
