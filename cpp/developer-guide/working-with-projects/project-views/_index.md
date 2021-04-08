---
title: Project Views
description: "Learn how to work with Microsoft Project (MPP/XML) views using Aspose.Tasks Java for C++."
type: docs
weight: 70
url: /cpp/project-views/
---

## **Reading Specific Gantt Chart View Data**
Gantt charts provide a graphical representation of a project plan. Sometimes it is necessary to read particular data associated with a Gantt chart view, such as the bar-style information, gridline properties, progress lines properties and time scale information. Aspose.Tasks for C++ API provides the capability to access all the properties individually with the GanttChartView class that inherits from View. This feature is supported for Microsoft Project 2003, 2007, 2010 and 2013 MPP file formats.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-ReadSpecificGantChartViewData-ReadSpecificGantChartViewData.cpp" >}}

## **Configure Gantt Chart View by Showing Selected Custom Fields**
Extended attributes added to a project may be assigned to a task. It may be desirable to add this custom field to a saved MPP file's default view, or you might want selected custom fields to be shown automatically rather than selecting them manually. This article describes how to achieve this by customizing the Table of a Project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-ConfigureTheGantChartViewShowSelectedColumnFields-ConfigureTheGantChartViewShowSelectedColumnFields.cpp" >}}

## **Customizing Timescale Tier Labels according to Current Culture Information**
Aspose.Tasks for C++ API provides the capability to customize Timescale tier labels according to the current CultureInfo of the machine. The DateTimeConverter(DateTime date) delegate provides a converter method to convert date to a string in view timescale tiers. In addition, TimescaleTier.DateTimeConverter enables rendering of date in the desired format.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-CustomizeTimescaleTierLabels-CustomizeTimescaleTierLabels.cpp" >}}

## **Setting Timescale Count for Project**
The TimeScaleTier class makes it possible to set the TimeScale count information for a project. The below example shows how to achieve this objective using the Aspose.Tasks API

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-SetTimeScaleCount-SetTimeScaleCount.cpp" >}}

## **Support for Text Styling**
Text styling can be applied to a Gantt Chart View using TableTextStyle as shown in the following code sample.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-SupportForTextStyle-SupportForTextStyle.cpp" >}}

## **Saving MPP with Default GanttChartView**
The following code example demonstrates the ability to save the MPP by setting the default view as a Gantt Chart.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectViews-SaveWithDefaultGanttChartView-SaveWithDefaultGanttChartView.cpp" >}}
