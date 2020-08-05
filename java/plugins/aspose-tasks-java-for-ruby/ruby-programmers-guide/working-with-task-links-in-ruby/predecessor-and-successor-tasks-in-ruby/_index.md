---
title: Predecessor and Successor Tasks in Ruby
type: docs
weight: 30
url: /java/predecessor-and-successor-tasks-in-ruby/
---

## **Aspose.Tasks - Predecessor and Successor Tasks**
To get Predecessor and Successor Tasks using **Aspose.Tasks Java for Ruby**, simply invoke **PredecessorAndSuccessorTask** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

tsk = Rjb::import('com.aspose.tasks.Tsk')

allinks = project.getTaskLinks().toList()

i = 0

while i < allinks.size()

  tsklnk = allinks.get(i)

  puts "Predecessor " + tsklnk.getPredTask().get(tsk.NAME).to_string

  puts "Successor " + tsklnk.getSuccTask().get(tsk.NAME).to_string

  puts "------------------------------------------------------"

  i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Predecessor and Successor Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/TaskLinks/predecessorandsuccessortask.rb)
