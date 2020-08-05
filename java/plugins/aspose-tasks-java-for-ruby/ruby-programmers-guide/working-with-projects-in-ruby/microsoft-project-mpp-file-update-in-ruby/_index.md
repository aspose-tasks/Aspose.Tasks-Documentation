---
title: Microsoft Project MPP File Update in Ruby
type: docs
weight: 80
url: /java/microsoft-project-mpp-file-update-in-ruby/
---

## **Aspose.Tasks - Update Project File**
To Update Project File using **Aspose.Tasks Java for Ruby**, simply invoke **UpdateProjectFile** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# create a new task

task = project.getRootTask().getChildren().add("Task1")

\# set start date

cal = Rjb::import('java.util.Calendar').getInstance()

cal.set(2015, 7, 1, 8, 0,0);

task.set(Rjb::import('com.aspose.tasks.Tsk').START, cal.getTime())

cal.set(2015, 7, 1, 17, 0, 0)

task.set(Rjb::import('com.aspose.tasks.Tsk').FINISH , cal.getTime())

\# Save the project as MPP project file

project.save(data_dir + "AfterLinking.mpp", Rjb::import('com.aspose.tasks.SaveFileFormat').MPP)

puts "Project file updated, please check the output file."

{{< /highlight >}}
## **Download Running Code**
Download **Update Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/updateprojectfile.rb)
