---
title: Read Calendar Information from Project Files
description: "Learn how to read project calendars using Aspose.Tasks for .NET."
type: docs
weight: 30
url: /net/reading-calendar-information/
---

## **Retrieving Calendar Information**
Microsoft Project lets users associate a variety of different calendars with working time, tasks and resources. These features are also available in Aspose.Tasks. This topic explains how to retrieve information about which calendars are used in a project. Aspose.Tasks can retrieve calendar information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

The [Calendars](https://apireference.aspose.com/tasks/net/aspose.tasks/project/properties/calendars) property exposed by the [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class supports List of [Aspose.Tasks.Calendar](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar) objects. This property can be used to retrieve the calendar information carried by the project.

To view calendar information in Microsoft Project:

1. Open a project.
2. From the **Project** menu, select **Change Working Time**.

The following piece of code retrieves the calendar information from a project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithCalendars-RetrieveCalendarInfo.cs" >}}

## **Reading Work Weeks Information from Calendar**
Aspose.Tasks for .NET API can read Work weeks information from any of the Project's calendar. The WorkWeek class can be used to achieve this.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithCalendars-ReadWorkWeeksInformation.cs" >}}

## **Getting Working Hours On or Between Dates**
Working hours are typically defined as a range of hours over a day, on specific days of the week. For example, 09:00 – 17:00, Monday to Friday. With Aspose.Tasks for .NET, it is possible to calculate the number of working hours that fall on a date, or between two dates. Finding out the number of working dates between two dates help project managers figure out whether there are enough hours to get work done, or if they need to find more resources to complete a task. It is recommended that for calculating the working hours between two dates, complete date and time (hours, minutes and seconds) should be provided for exact calculation. If the only date is given as finish date value say 2016, 8, 18, it will be considered as 0:0:0 hours on that day and, hence, finish date day will not be included in the calculation. However, if the finish date is given as 2016,8,18,17,0,0, then the proper result will be calculated.

The [Calendar](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar) class exposes two methods(overloaded) for finding working hours on or between dates. [GetWorkingHours(DateTime dt)](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar/methods/getworkinghours) and [GetWorkingHours(DateTime startdt, DateTime enddt)](https://apireference.aspose.com/tasks/net/aspose.tasks.calendar/getworkinghours/methods/1) to define the working hours between two dates.

The following example shows how to find the duration in minutes, hours and days between two dates.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithCalendars-CalculateWorkHours.cs" >}}
