---
title: Read a Task's Timephased Data in Ruby
type: docs
weight: 120
url: /java/read-a-task-s-timephased-data-in-ruby/
---

## **Aspose.Tasks - Read a Task's Timephased Data**
To Read a Task's Timephased Data using **Aspose.Tasks Java for Ruby**, simply invoke **GetTaskTimephasedData** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
prj = Rjb::import('com.aspose.tasks.Prj')
tsk = Rjb::import('com.aspose.tasks.Tsk')
cal = Rjb::import('java.util.Calendar').getInstance()
cal.set(2013,7,17,8,0,0)
project.set(prj.START_DATE, cal.getTime())
project.set(prj.NEW_TASKS_ARE_MANUAL, Rjb::import('com.aspose.tasks.NullableBool').new(false))
task = project.getRootTask().getChildren().add("Task")
rsc = project.getResources().add("Rsc")
rsc.set(Rjb::import('com.aspose.tasks.Rsc').STANDARD_RATE, Rjb::import('java.math.BigDecimal').valueOf(10))
rsc.set(Rjb::import('com.aspose.tasks.Rsc').OVERTIME_RATE, Rjb::import('java.math.BigDecimal').valueOf(15))
task.set(tsk.DURATION, project.getDuration(6))
assignment = project.getResourceAssignments().add(task, rsc)
d = Rjb::import('java.util.Date').new(0)
assignment.set(Rjb::import('com.aspose.tasks.Asn').STOP, Rjb::import('java.util.Date').new(0))
assignment.set(Rjb::import('com.aspose.tasks.Asn').RESUME, Rjb::import('java.util.Date').new(0))
assignment.set(Rjb::import('com.aspose.tasks.Asn').WORK_CONTOUR, Rjb::import('com.aspose.tasks.WorkContourType').BackLoaded)
project.setBaseline(Rjb::import('com.aspose.tasks.BaselineType').Baseline)
task.set(tsk.PERCENT_COMPLETE, 50)
td = assignment.getTimephasedData(assignment.get(Rjb::import('com.aspose.tasks.Asn').START), 
				assignment.get(Rjb::import('com.aspose.tasks.Asn').FINISH), 
Rjb::import('com.aspose.tasks.TimephasedDataType').AssignmentRemainingWork).toList()
puts "Size: " + td.size().to_s
puts "Value: " + td.get(0).getValue().to_s
{{< /highlight >}}

## **Download Running Code**
Download **Read a Task's Timephased Data (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/gettasktimephaseddata.rb)
