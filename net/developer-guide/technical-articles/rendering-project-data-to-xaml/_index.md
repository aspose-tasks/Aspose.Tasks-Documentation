---
title: Rendering Project Data to XAML
description: "Learn how to render a project as XAML using Aspose.Tasks for .NET."
type: docs
weight: 60
url: /net/rendering-project-data-to-xaml/
---

Aspose.Tasks lets you render project data to an XAML file. The easiest way to accomplish this task is to use the SaveFileFormat.XAML option with the Project.Save function. SaveOptions can be used to set the options like FitContent, LegendOnEachPage, TimeScale and View}}. GanttChartView and GanttChartColumn can be used to select the columns for display.

## **Rendering to XAML with Options**
The following code sample demonstrates how this feature can be used in C#.NET and VB.NET:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-Articles-RenderToXAML-RenderToXAML.cs" >}}

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-Articles-RenderXAMLWithOptions-RenderXAMLWithOptions.cs" >}}

Different presentation formats can be used to render the project to XAML: 
- PresentationFormat.GanttChart;
- PresentationFormat.TaskUsage;
- PresentationFormat.ResourceUsage; 
- PresentationFormat.ResourceSheet.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-Articles-RenderDifferentPresentationFormatsToXAML-RenderDifferentPresentationFormatsToXAML.cs" >}}
