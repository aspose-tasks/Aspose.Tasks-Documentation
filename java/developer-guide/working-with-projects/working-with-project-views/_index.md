---
title: Working with Project Views
description: "Learn how to work with Gantt chart project representation from Microsoft Project MPP files using Aspose.Tasks for .NET."
type: docs
weight: 70
url: /java/working-with-project-views/
---

## **Reading Specific Gantt Chart View Data**
Gantt charts provide a graphical representation of project plans. Sometimes it is necessary to read particular data associated with a Gantt chart view such as the bar-style information, gridline properties, progress lines properties and time scale information. Aspose.Tasks for Java API provides the capability to access all the properties individually using the [GanttChartView](https://apireference.aspose.com/tasks/java/com.aspose.tasks/GanttChartView) class that inherits from View. This feature is supported for Microsoft Project 2003, 2007, 2010, 2013, 2016 and 2019 MPP file formats.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ReadSpecificGanttChartData-reading-speficific-gant-chart-data.java" >}}
## **Configure Gantt Chart View by Showing Selected Custom Fields**
Extended attributes added to a project may be assigned to a task and it is often desirable to add custom fields to the default view of an MPP file, or you might want selected custom fields to be shown automatically rather than selected manually. This article describes how to achieve this by customizing a Project's table.

The code below shows how to configure a Gantt chart view with custom fields.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ConfigureGanttChartView-ConfigureGantChart.java" >}}
## **Customize Timescale Tier Labels according to Local Culture**
Aspose.Tasks for Java API can be used to customer timescale tier labels according to local culture information.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-CustomizeTimeScaleTierLabels-customize-time-scale-tier-labels.java" >}}
## **Setting TimeScale Count for Project**
The TimeScaleTier class makes it possible to set the time scale count information for a Project. This topic shows how to achieve this objective using Aspose.Tasks for Java API.

The code below shows how to set the time scale count.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SetTimeScaleCount-set-time-scale-count.java" >}}
