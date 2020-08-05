---
title: Updating and Removing Calendar
type: docs
weight: 20
url: /cpp/updating-and-removing-calendar/
---

## **Replacing a Calendar**
Calendars are used to see whether resources are available, and when tasks are scheduled. There are different types of calendars. This article looks at how to replace a base calendar, that is, the calendar used for projects and tasks, with another one.

Base calendars come in different forms:

- Standard: the default calendar has a Monday to Friday work week and a day that runs from 08:00 to 17:00.
- 24-hours: used for around the clock working, or for resources that run around the clock.
- Night shift: similar to the standard calendar, the night-shift calendar has a Monday to Saturday morning work week and a day that runs from 23:00 to 08:00.
### **Replacing a Calendar with a New Calendar**
The list of all calendars can be retrieved as CalendarCollection using the Project class. The CalendarCollection can then be used to Remove or Add a new calendar as shown in the following code sample.

The code example given below demonstrates how to replace an existing calendar with a new standard calendar.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithCalendars-CreatingUpdatingAndRemoving-ReplaceCalendarWithNewCalendar-ReplaceCalendarWithNewCalendar.cpp" >}}
## **Writing Updated Calendar Data to MPP**
With Aspose.Tasks, you can update calendar data in a Microsoft Project MPP file and save it back.

The following code shows how to update the calendar data of a project by adding a new calendar and saving it back to the original MPP file. The steps involved in this activity are:

1. Read the source MPP file.
1. Add the calendar data to the project.
1. Save the updated project data back to the MPP file.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithCalendars-CreatingUpdatingAndRemoving-WriteUpdatedCalendarDataToMPP-WriteUpdatedCalendarDataToMPP.cpp" >}}
