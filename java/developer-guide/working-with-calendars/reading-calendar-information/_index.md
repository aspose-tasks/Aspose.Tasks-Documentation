---
title: Reading Calendar Information
type: docs
weight: 30
url: /java/reading-calendar-information/
---

## **Retrieving Calendar Information**
Microsoft Project lets users associate a variety of different calendars with working time, tasks and resources. These features are also available in Aspose.Tasks. This article explains how to retrieve information about which calendars are used in a project. Aspose.Tasks can retrieve calendar information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

The CalendarS property exposed by the [Project](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Project) class supports List of [Aspose.Tasks.Calendar](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Calendar) objects. This property can be used to retrieve the calendar information carried by the project.

To view calendar information in Microsoft Project:

1. Open a project.
1. From the **Project** menu, select **Change Working Time**.

**The Change Working Time dialog showing a list of calendars** 

![todo:image_alt_text](/plugins/servlet/confluence/placeholder/unknown-attachment)

**Programming Sample**

The following piece of code retrieves the calendar information from a project.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RetrieveCalendarInfo-retrieve-calendar-info.java" >}}
## **Getting Working Hours On or Between Dates**
Working hours are typically defined as a range of hours over a day, on specific days of the week. For example, 09:00 – 17:00, Monday to Friday. With Aspose.Tasks, it is possible to calculate the number of working hours that fall on a date, or between two dates. Finding out the number of working dates between two dates help project managers figure out whether there are enough hours to get work done, or if they need to find more resources to complete a task.
### **Calculating Working Hours**
The [Calendar](/pages/createpage.action?spaceKey=tasksjava&title=com.aspose.tasks.Calendar+Class&linkCreation=true&fromPageId=22285379) class exposes two overloaded methods for finding working hours on or between dates:

- getWorkingHours(Date dt) returns a long data type to hold the working hours on a date passed.
- getWorkingHours(Date startdt,Date enddt) returns a WorkUnit object to define the working hours between two dates.

**Programming Sample**

The following example shows how to find the duration in minutes, hours and days between two dates.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Calendars-GetWorkingHours-GetWorkingHours.java" >}}
