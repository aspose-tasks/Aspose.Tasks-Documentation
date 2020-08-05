---
title: Public API Changes in Aspose.Tasks for .NET 9.3.0
type: docs
weight: 190
url: /net/public-api-changes-in-aspose-tasks-for-net-9-3-0/
---

|**The following public classes were added:** |**Description** |
| :- | :- |
|Aspose.Tasks.LoadOptions |Allows to specify additional load parameters when loading a project from file or stream. |
|Aspose.Tasks.WorkWeekCollection |Represents a collection of WorkWeek objects. |
|**The following public constructors were added to existing class:** |** |
|Aspose.Tasks.Project(Stream, Aspose.Tasks.LoadOptions) |Initializes a new instance of the Project class from the Stream with the specified instance of the LoadOptions class. |
|Aspose.Tasks.Project(string, Aspose.Tasks.LoadOptions) |Initializes a new instance of the Project class from a template (existent mpp or mpt file) with the specified instance of the LoadOptions class. |
|**The following public properties were added to existing classes:** |** |
|Aspose.Tasks.Group.MaintainHierarchy |Determines whether to show all the levels of summary tasks for subtasks within group. |
|Aspose.Tasks.Group.ShowInMenu |Returns true if Project shows the group name in the Group drop-down list in the Ribbon. |
|Aspose.Tasks.Calendar.WorkWeeks |Returns WorkWeekCollections object that is associated with the calendar. |
|**The following fields were added to public enums:** |** |
|Aspose.Tasks.DateFormat.DateDdMmYyyy |Date format like 17/03/2016 |
|Aspose.Tasks.Visualization.DateLabel.DayDdMmYyyy |Day format like 17/03/2016 |

