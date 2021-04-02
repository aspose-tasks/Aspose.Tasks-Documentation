---
title: Working with Calendar Properties
description: "The page describes the general properties of project calendars using Aspose.Tasks for .NET."
type: docs
weight: 20
url: /net/working-with-calendar-properties/
---

## **Working with General Calendar Properties**
Microsoft Project uses calendars and other information to calculate project end dates. Aspose.Tasks supports calendar functionality. This article illustrates the calendar properties that can be set and shows how they are applied in code.

The [Calendar](https://apireference.aspose.com/tasks/net/aspose.tasks/extendedattributedefinition) exposes a number of properties used to define the base calendar in Microsoft Outlook:

- [BaseCalendar](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar/properties/basecalendar) – the base calendar. This property supports the Calendar object for reading and writing the base calendar for the current calendar instance and is only applicable is the current calendar instance is not already a base calendar.
- [Name](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar/properties/name) – the calendar's name. Get or set the property with a string.
- [Uid](https://apireference.aspose.com/tasks/net/aspose.tasks/calendar/properties/uid) – the calendar's unique ID. Integer.

The code that follows gets the general calendar properties.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithCalendars-GeneralCalendarProperties-ReadCalendarProps.cs" >}}
