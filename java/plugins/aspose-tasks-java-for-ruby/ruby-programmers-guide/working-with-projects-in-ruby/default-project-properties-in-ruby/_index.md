---
title: Default Project Properties in Ruby
type: docs
weight: 30
url: /java/default-project-properties-in-ruby/
---

## **Aspose.Tasks - Default Project Properties**
To get Default Project Properties using **Aspose.Tasks Java for Ruby**, call **get_default_project_properties** method of **ProjectProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}



def get_default_project_properties()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'Sample.xml')

    prj = Rjb::import('com.aspose.tasks.Prj')

    # Display default properties

    puts "Project Version : " + project.get(prj.SAVE_VERSION).to_string

    puts "New Task Default Start: "+ project.get(prj.DEFAULT_START_TIME).to_string

    puts "New Task Default Type: "+ project.get(prj.DEFAULT_TASK_TYPE).to_string

    puts "Resouce Default Standard Rate: "+ project.get(prj.DEFAULT_STANDARD_RATE).to_string

    puts "Resource Default Overtime Rate: "+ project.get(prj.DEFAULT_OVERTIME_RATE).to_string

    puts "Default Task EV Method: "+ project.get(prj.DEFAULT_TASK_EV_METHOD).to_string

    puts "Default Cost Accrual: "+ project.get(prj.DEFAULT_FIXED_COST_ACCRUAL).to_string

end

{{< /highlight >}}
## **Download Running Code**
Download **Default Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/projectproperties.rb)
