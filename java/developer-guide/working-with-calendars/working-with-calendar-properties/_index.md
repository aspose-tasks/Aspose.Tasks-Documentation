---
title: Working with Calendar Properties
description: "The page describes the general properties of project calendars using Aspose.Tasks for Java."
type: docs
weight: 20
url: /java/working-with-calendar-properties/
---

Microsoft Project use calendars and other information to calculate project end dates. Aspose.Tasks for Java supports the calendar functionality. This article illustrates the calendar properties that can be set and shows how they are applied in code.

**Calendar Properties**
The [Calendar](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Calendar) exposes several properties used to define the base calendar in Microsoft Outlook:

- BaseCalendar – the base calendar. This property supports the Calendar object for reading and writing the base calendar for the current calendar instance and is only applicable if the current calendar instance is not already a base calendar.
- Days – the days of the week that are weekdays. A list of WeekDay objects.
- Name – the calendar's name. Get or set the property with a string.
- Uid – the calendar's unique ID. Integer.
- WorkWeeks – a collection of effective work weeks.

The code that follows gets the general calendar properties.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Calendars-CalendarProperties-CalendarProperties.java" >}}
