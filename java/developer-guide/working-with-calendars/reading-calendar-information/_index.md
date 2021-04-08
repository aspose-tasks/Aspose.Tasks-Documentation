---
title: Reading Calendar Information
description: "Learn how to read Microsoft Project (MPP/XML) calendar properties using Aspose.Tasks Java for Ruby."
type: docs
weight: 30
url: /java/reading-calendar-information/
---

## **Retrieving Calendar Information**
Microsoft Project lets users associate a variety of different calendars with working time, tasks and resources. These features are also available in Aspose.Tasks. This article explains how to retrieve information about which calendars are used in a project. Aspose.Tasks can retrieve calendar information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

The CalendarS property exposed by the [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project) class supports List of [Aspose.Tasks.Calendar](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Calendar) objects. This property can be used to retrieve the calendar information carried by the project.

To view calendar information in Microsoft Project:

1. Open a project.
2. From the **Project** menu, select **Change Working Time**.

The following piece of code retrieves the calendar information from a project.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RetrieveCalendarInfo-retrieve-calendar-info.java" >}}

## **Reading Work Weeks Information from Calendar**
Aspose.Tasks for Java API can read Work weeks information from any of the Project’s calendar. The WorkWeek class can be used to achieve this.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Calendars-ReadWorkWeeks-ReadWorkWeeksInformation.java" >}}

## **Getting Working Hours On or Between Dates**
Working hours are typically defined as a range of hours over a day, on specific days of the week. For example, 09:00 – 17:00, Monday to Friday. With Aspose.Tasks for Java, it is possible to calculate the number of working hours that fall on a date, or between two dates. Finding out the number of working dates between two dates help project managers figure out whether there are enough hours to get work done, or if they need to find more resources to complete a task.

### **Calculating Working Hours**
The [Calendar](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Calendar) class exposes two overloaded methods for finding working hours on or between dates:

- getWorkingHours(Date dt) returns a long data type to hold the working hours on a date passed.
- getWorkingHours(Date startdt, Date enddt) returns a WorkUnit object to define the working hours between two dates.

The following example shows how to find the duration in minutes, hours and days between two dates.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Calendars-GetWorkingHours-GetWorkingHours.java" >}}
