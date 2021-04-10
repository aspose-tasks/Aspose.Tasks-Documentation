---
title: Aspose.Tasks for .NET 21.4 Release Notes
type: docs
weight: 97
url: /net/aspose-tasks-for-net-21-4-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for .Net 21.4](https://downloads.aspose.com/tasks/net/new-releases/-aspose.tasks-for-.net-21.4/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-4788 | Add support for SaveOptions.TaskFilter and SaveOptions.TasksComparer options when project is saved to CSV or XLSX formats | Enhancement |
| TASKSNET-4769 | Remove an ability to set Tsk.Id when using CalculationMode.Manual and CalculationMode.Automatic | Enhancement |
| TASKSNET-4793 | Fix exported value of "Outline Code *" attributes when project is saved to non-MPP formats. | Bug |
| TASKSNET-4792 | Fix headers in exported xlsx when custom ProjectView is specified. | Bug |
| TASKSNET-4772 | Fix parsing of "Round" operator in formulas | Bug |
| TASKSNET-4770 | Fix wrong calendar exception usage | Bug |
| TASKSNET-4751 | Fix OverflowException while reading MPP file | Bug |
| TASKSNET-4749 | Fix tasks splitting in case of splits beginning \ ending in middle of the day. | Bug |
| TASKSNET-4746 | Fix chart rendering to take chart position into account | Bug |
| TASKSNET-4697 | Fix incorrect ids of task children | Bug |
| TASKSNET-4695 | Fix incorrect resource unit price while converting to CSV | Bug |
| TASKSNET-4694 | Fix incorrect unit of work time in 2010 and 2007 formats while exporting to CSV | Bug |
| TASKSNET-4693 | Fix task splitting in MPP export not working as expected | Bug |
| TASKSNET-4374 | Fix file resaved with Aspose.Tasks cannot be opened by MSP 2016 | Bug |
## **Public API and Backwards Incompatible Changes**
|**The following public methods and properties were deleted:**|**Description**|
| :- | :- |
| Aspose.Tasks.ResourceAssignment.Set(Aspose.Tasks.Key{System.DateTime,Aspose.Tasks.AsnKey},System.DateTime) |  |
| Aspose.Tasks.Task.Get(Aspose.Tasks.Key{System.String,Aspose.Tasks.TaskKey}) |  |
| Aspose.Tasks.Task.Set(Aspose.Tasks.Key{System.DateTime,Aspose.Tasks.TaskKey},System.DateTime) |  |