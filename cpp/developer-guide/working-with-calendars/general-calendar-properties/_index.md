---
title: General Calendar Properties
type: docs
weight: 30
url: /cpp/general-calendar-properties/
---

## **General Calendar Properties**
Microsoft Project uses calendars and other information to calculate project end dates. Aspose.Tasks for C++ API supports calendar functionality. This article illustrates the calendar properties that can be set and shows how they are applied in code.

The Calendar exposes a number of properties used to define the base calendar in Microsoft Outlook:

- BaseCalendar – the base calendar. This property supports the Calendar object for reading and writing the base calendar for the current calendar instance and is only applicable is the current calendar instance is not already a base calendar.
- Name – the calendar's name. Get or set the property with a string.
- Uid – the calendar's unique ID. Integer.

The code example given below demonstrates how to get the general calendar properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithCalendars-GeneralCalendarProperties-ReadCalendarProps.cpp" >}}
