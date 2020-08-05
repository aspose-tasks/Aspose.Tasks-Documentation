---
title: Public API Changes in Aspose.Tasks for Java 9.3.0
type: docs
weight: 190
url: /java/public-api-changes-in-aspose-tasks-for-java-9-3-0/
---

|**The following public classes were added:**|**Description**|
| :- | :- |
|com.aspose.tasks.LoadOptions |Allows to specify additional load parameters when loading a project from file or stream. |
|com.aspose.tasks.WorkWeekCollection |Represents a collection of WorkWeek objects. |
|**The following public constructors were added to existing classes:**|** |
|com.aspose.tasks.Project(InputStream, LoadOptions) |Initializes a new instance of the Project class from the Stream with the specified instance of the LoadOptions class. |
|com.aspose.tasks.Project(String, LoadOptions) |Initializes a new instance of the Project class from a template (existent mpp or mpt file)<br>with the specified instance of the LoadOptions class. |
|**The following public methods were added to existing classes:**|** |
|com.aspose.tasks.Calendar.getWorkWeeks |Returns the collection of work weeks that is associated with the calendar. |
|com.aspose.tasks.Group.getMaintainHierarchy |Returns a flag which determines whether to show all the levels of summary tasks for subtasks within this group. |
|com.aspose.tasks.Group.setMaintainHierarchy(boolean) |Sets a flag which determines whether to show all the levels of summary tasks for subtasks within this group. |
|com.aspose.tasks.getShowInMenu |Returns a flag which determines whether to show the group name in the Group drop-down list in the Ribbon. |
|com.aspose.tasks.setShowInMenu(boolean) |Sets a flag which determines whether to show the group name in the Group drop-down list in the Ribbon. |
|com.aspose.tasks.Project.save(OutputStream, /**SaveFileFormat**/int) |Saves the project data to the output stream. |
|com.aspose.tasks.Project.save(OutputStream, SaveOptions) |Saves the project to the output stream using the specified save options. |
|**The following fields were added to public enums:**|** |
|com.aspose.tasks.DateFormat.DateDdMmYyyy |Date format like 17/03/2016 |
|com.aspose.tasks.DateLabel.DayDdMmYyyy |Day format like 17/03/2016 |

