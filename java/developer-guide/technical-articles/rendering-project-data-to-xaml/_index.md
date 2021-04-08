---
title: Rendering Project Data to XAML
description: "Learn how to render a project as XAML using Aspose.Tasks for Java."
type: docs
weight: 30
url: /java/rendering-project-data-to-xaml/
---

Aspose.Tasks for Java lets you render project data to an XAML file. The easiest way to accomplish this task is to use the SaveFileFormat.XAML option with the Project.Save function. SaveOptions can be used to set the options like FitContent, LegendOnEachPage, TimeScale and View. GanttChartView and GanttChartColumn can be used to select the columns for display.

## **Rendering to XAML**

The following code sample demonstrates how this feature can be used using Aspose.Tasks for Java:

**Java**

{{< highlight java >}}
Project project = new Project("RenderMe.mpp");
project.save("NewProductDev.xaml", SaveFileFormat.XAML);
{{< /highlight >}}

### **Render XAML with Options**

**Java**

{{< highlight java >}}
Project project = new Project("NewProductDev.mpp");
SaveOptions options = new XamlOptions();
options.setFitContent(true);
options.setLegendOnEachPage(false);
options.setTimescale(Timescale.ThirdsOfMonths);
project.save("NewProductDev.xaml", options);
{{< /highlight >}}

### **Render to XAML using Different Presentation Formats**
Different presentation formats can be used to render the project to XAML: PresentationFormat.GanttChart, PresentationFormat.TaskUsage, PresentationFormat.ResourceUsage and PresentationFormat.ResourceSheet.

**Java**

{{< highlight java >}}
Project project = new Project("NewProductDev.mpp");
SaveOptions options = new XamlOptions();
options.setPresentationFormat(PresentationFormat.GanttChart);
project.save("NewProductDev GanttChart.xaml", options);
{{< /highlight >}}
