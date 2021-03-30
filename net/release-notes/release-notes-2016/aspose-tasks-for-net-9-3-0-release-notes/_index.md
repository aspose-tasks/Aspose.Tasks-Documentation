---
title: Aspose.Tasks for .NET 9.3.0 Release Notes
type: docs
weight: 60
url: /net/aspose-tasks-for-net-9-3-0-release-notes/
---

## **Major Features**
Improved security and implemented a lot of optimization. We have supported Primavera SQLite database for reading. Recalculation option for ActualWork and RemainingWork

task fields was supported. Some bugs have been fixed. Please see the list of changes below.
### **All Changes**

|**Key** |**Summary** |**Category** |
| :- | :- | :- |
|TASKS-34444 |Support for Primavera SQLite DB |New Feature |
|TASKS-34499 |Support recalculation option for ActualWork and RemainingWork task fields |New Feature |
|TASKS-34509 |Provide new date format DateFormat.DateDdMMYyyy to render date like 19/07/2016 |Enhancement |
|TASKS-34409 |Aspose.Tasks API reads only first value of each list item |Bug |
|TASKS-34441 |Wrong working times read from project Calendar |Bug |
|TASKS-34468 |Resaving MPP loses Resource Calendar Work Weeks time information |Bug |
|TASKS-34479 |Extended attributes missing while reading task from MPP |Bug |
|TASKS-34480 |Writing Formulas in Custom Fields |Bug |
|TASKS-34486 |Lookup option not selected when Number and Duration extended attributes both added simultaneously |Bug |
|TASKS-34490 |Duration extended attribute removed from task after saving the MPP |Bug |
|TASKS-34497 |Remaining work and actual work not summarized correctly |Bug |
|TASKS-34500 |The signature of Aspose.Tasks.msi is corrupt or invalid |Bug |
|TASKS-34502 |Reading MPP file raises ProjectReadingException |Bug |
|TASKS-34513 |Resaving the MPP file raises exception |Bug |
### **Public API and Backwards Incompatible Changes**
The following public classes were added:

Class Name Description
Aspose.Tasks.LoadOptions Allows to specify additional load parameters when loading a project from file or
stream.
Aspose.Tasks.WorkWeekCollection Represents a collection of WorkWeek objects.
The following public properties were added to existing classes:

Aspose.Tasks.Group.MaintainHierarchy Determines whether to show all the levels of summary tasks for subtasks within group.
Aspose.Tasks.Group.ShowInMenu Returns true if Project shows the group name in the Group drop-down list in the
Ribbon.
The following fields were added to public enums:

Aspose.Tasks.DateFormat.DateDdMmYyyy Date format like 17/03/2016
Aspose.Tasks.Visualization.DateLabel.DayDdMmYyyy Day format like 17/03/2016
