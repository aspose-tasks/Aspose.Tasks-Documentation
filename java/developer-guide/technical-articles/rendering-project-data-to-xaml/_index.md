---
title: Rendering Project Data to XAML
type: docs
weight: 30
url: /java/rendering-project-data-to-xaml/
---

{{% alert color="primary" %}} 

Aspose.Tasks lets you render project data to an XAML file. The easiest way to accomplish this task is to use the SaveFileFormat.XAML option with the Project.Save function. SaveOptions can be used to set the options like FitContent, LegendOnEachPage, TimeScale and View. GanttChartView and GanttChartColumn can be used to select the columns for display.

{{% /alert %}} 
## **Rendering to XAML**
The following code sample demonstrates how this feature can be used using Aspose.Tasks for Java:



**Java**

{{< highlight java >}}

 //Load project

Project project = new Project("RenderMe.mpp");

String resFile = "NewProductDev.xaml";

project.save(resFile, SaveFileFormat.XAML);

{{< /highlight >}}
### **Render XAML with Options**
**Java**

{{< highlight java >}}

 //Load project

Project project = new Project("NewProductDev.mpp");

String resFile = "NewProductDev.xaml";

SaveOptions options = new XamlOptions();

options.setFitContent(true);

options.setLegendOnEachPage(false);

options.setTimescale(Timescale.ThirdsOfMonths);

project.save(resFile, options);

{{< /highlight >}}
### **Render to XAML using Different Presentation Formats**
Different presentation formats can be used to render the project to XAML: PresentationFormat.GanttChart, PresentationFormat.TaskUsage, PresentationFormat.ResourceUsage and PresentationFormat.ResourceSheet.

**Java**

{{< highlight java >}}

 //Load project

Project project = new Project("NewProductDev.mpp");

//PresentationFormat presentationFormat = PresentationFormat.GanttChart;

String resFile = "NewProductDev GanttChart" + ".xaml";

SaveOptions options = new XamlOptions();

options.setPresentationFormat(PresentationFormat.GanttChart);

project.save(resFile, options);

{{< /highlight >}}






