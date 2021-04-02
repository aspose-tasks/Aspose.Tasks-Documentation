---
title: Working with Project Views
type: docs
weight: 100
url: /net/working-with-project-views/
---

## **Reading Specific Gantt Chart View Data**
Gantt charts provide a graphical representation of a project plan. Sometimes it is necessary to read particular data associated with a Gantt chart view, such as the bar-style information, gridline properties, progress lines properties and time scale information. Aspose.Tasks provides the capability to access all the properties individually with the [GanttChartView](https://apireference.aspose.com/tasks/net/aspose.tasks/ganttchartview) class that inherits from View. This feature is supported for Microsoft Project 2003, 2007, 2010 and 2013 MPP file formats.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-ReadSpecificGantChartViewData-ReadSpecificGantChartViewData.cs" >}}
## **Configure Gantt Chart View by Showing Selected Custom Fields**
Extended attributes added to a project may be assigned to a task. It may be desirable to add this custom field to a saved MPP file's default view, or you might want selected custom fields to be shown automatically rather than selecting them manually. This article describes how to achieve this by customizing the Table of a Project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-ConfigureTheGantChartViewShowSelectedColumnFields-ConfigureTheGantChartViewShowSelectedColumnFields.cs" >}}

## **Customizing Timescale Tier Labels according to Current Culture Information**
Aspose.Tasks for .NET API provides the capability to customize Timescale tier labels according to the current CultureInfo of the machine. The DateTimeConverter(DateTime date) delegate provides a converter method to convert date to a string in view timescale tiers. In addition, [TimescaleTier.DateTimeConverter](https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/timescaletier) enables rendering of date in the desired format.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-CustomizeTimescaleTierLabels-CustomizeTimescaleTierLabels.cs" >}}
## **Setting Timescale Count for Project**
The [TimeScaleTier](https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/timescaletier) class makes it possible to set the TimeScale count information for a project. The below example shows how to achieve this objective using the Aspose.Tasks for .NET API

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-SetTimeScaleCount-SetTimeScaleCount.cs" >}}
## **Support for Text Styling**
Text styling can be applied to a Gantt Chart View using TableTextStyle as shown in the following code sample.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-SupportForTextStyle-SupportForTextStyle.cs" >}}
## **Saving MPP with Default GanttChartView**
The following code example demonstrates the ability to save the MPP by setting the default view as a Gantt Chart.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithProjectViews-SaveWithDefaultGanttChartView-SaveWithDefaultGanttChartView.cs" >}}
