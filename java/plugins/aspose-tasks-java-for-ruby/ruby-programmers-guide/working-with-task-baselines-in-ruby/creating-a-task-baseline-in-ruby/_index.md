---
title: Creating a Task Baseline in Ruby
type: docs
weight: 20
url: /java/creating-a-task-baseline-in-ruby/
---

## **Aspose.Tasks - Creating a Task Baseline**
To Create a Task Baseline using **Aspose.Tasks Java for Ruby**, simply invoke **CreateTaskBaseline** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Set baseline for the entire project

project.setBaseline(Rjb::import('com.aspose.tasks.BaselineType').Baseline)

puts "Set baseline for the project."

{{< /highlight >}}
## **Download Running Code**
Download **Creating a Task Baseline (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskBaselines/createtaskbaseline.rb)
