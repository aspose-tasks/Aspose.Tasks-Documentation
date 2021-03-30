---
title: Display Multiple Columns in Rendered Gantt Chart Image
type: docs
weight: 10
url: /net/display-multiple-columns-in-rendered-gantt-chart-image/
---

## **Overview**
{{% alert color="primary" %}} 

In Microsoft Project, project data is not only available in the textual form, but can also be displayed graphically as a chart known as a Gantt chart. Aspose.Tasks for .NET provides API classes under the Aspose.Tasks namespace to work with project elements like tasks, resources, assignments, calendars, calendar exceptions and so on.

In recent releases, Aspose.Tasks for .NET has introduced the Aspose.Tasks.Visualization namespace that provides classes for rendering project data.

This article describes how to select project columns to include in a Gantt chart and how to render the chart to an image.

{{% /alert %}} 
## **Gantt Chart**
A Gantt chart is a graphical representation of project tasks broken down by days, weeks or months. A project is composed of tasks assigned to different resources. An individual task may be divided into sub-tasks as part of tasks management. Every task has a start date and end date that determines its duration. A Gantt chart in Microsoft Project gives a quick view of such project data. This screenshot shows a typical Gantt chart in Microsoft Project: 

![todo:image_alt_text](display-multiple-columns-in-rendered-gantt-chart-image_1.png)
## **Gantt Chart Image in Aspose.Tasks for .NET**
In Aspose.Tasks for .NET, the Project class is the main class for handling project files. The Project class exposes the Export overload method for exporting project data to different file formats. The users can configure this method to export project data to any supported format by passing parameters:

- The first parameter defines the rendering format, one of the members of the RenderFormat enumeration.
- The second parameter defines the presentation format of the rendered object and is one of the PresentationFormat enumeration members.
- The third parameter is the destination file name.
- The fourth, and most important, parameter is IRenderParam which defines the rendering dimensions.

IRenderParam is basically the base interface for rendering parameters. In order to define the rendering parameters for the image, we have to use the BaseImageRenderParam type that implements the IRenderParam interface.
### **BaseImageRenderParam Type**
Before actually using the Export method (exposed by the Project class) to render the project data to an image, define image rendering parameters using the BaseImageRenderParam type which exposes a number of constructor overloads. This type can be configured to define the image size, location, zoom factor, page number and to display a legend on each page.

The number of pages in the rendered image depends on the task's net duration. The possible number of pages in the rendered image is equal to the number of months of the tasks net duration. If the task's net duration is one month or less than a month, there will only be one page.

You pass the number of pages to be rendered in the image. For example, this code example defines an image that is 800x600, with no zoom factor and only one page of the project data:

{{< highlight java >}}

 BaseImageRenderParam imageRenderingParameters=new BaseImageRenderParam(null, Point.Empty, new Size(800, 600),100, 0, true);

{{< /highlight >}}

{{< highlight java >}}

 Dim imageRenderingParameters As New BaseImageRenderParam(Nothing, Point.Empty, New Size(800, 600),100, 0, True)

{{< /highlight >}}
### **ProjectView Type**
The ProjectView class can be used to display specific columns in the output image. A constructor of this class takes an array list of the GanttChartColumn class as its argument. The example code shows how it works:

{{< highlight java >}}

 //Create the view columns

ArrayList columns = new ArrayList();

columns.Add(new GanttChartColumn("Name", 100, new TaskToColumnTextConverter(TaskName)));

columns.Add(new GanttChartColumn("Notes", 100, new TaskToColumnTextConverter(TaskNotes)));

columns.Add(new GanttChartColumn("Resources", 200, new TaskToColumnTextConverter(TaskResources)));

//Create the view

ProjectView view = new ProjectView(columns);

{{< /highlight >}}


The constructor of the GanttChartColumn class takes three arguments - the column name, width and a delegate TaskToColumnTextConverter - to convert task data to column text.

In the above code example, TaskToColumnTextConverter delegate calls three target methods, TaskName, TaskNotes and TaskResources, to convert the data in these columns to text. The three methods are implemented in the following code example.

{{< highlight java >}}

 /// <summary>

/// Converts a task's name data to column text.

/// </summary>

/// <param name="task">Current task.</param>

/// <returns>Column's text.</returns>

private string TaskName(Task task)

{

    StringBuilder res = new StringBuilder();

    for (int i = 1; i < task.OutlineLevel; i++)

        res.Append("  ");

    res.AppendFormat("{0}. {1}", task.Id, task.Name);

    return res.ToString();

}


/// <summary>

/// Converts a task's name data to column text.

/// </summary>

/// <param name="task">Current task.</param>

/// <returns>Column's text.</returns>

private string TaskNameHtml(Task task)

{

    StringBuilder res = new StringBuilder();

    for (int i = 1; i < task.OutlineLevel; i++)

        res.Append("&nbsp;&nbsp;");

    res.AppendFormat("{0}. {1}", task.Id, task.Name);

    return res.ToString();

}


/// <summary>

/// Converts a task's notes data to column text.

/// </summary>

/// <param name="task">Current task.</param>

/// <returns>Column's text.</returns>

private string TaskNotes(Task task)

{

    if (task.NotesText != null)

        return task.NotesText;

    else

        return string.Empty;

}


/// <summary>

/// Converts a task's resources data to column text.

/// </summary>

/// <param name="task">Current task.</param>

/// <returns>Column's text.</returns>

private string TaskResources(Task task)

{

    StringBuilder res = new StringBuilder();

    Project project = task.ParentProject;

    bool bFirst = true;


    foreach (ResourceAssignment assignment in project.GetResourceAssignmentsByTask(task))

        if (assignment.Resource != null)

        {

            if (!bFirst)

                res.Append(", ");

            res.Append(assignment.Resource.Name);

            bFirst = false;

        }

    return res.ToString();

}

{{< /highlight >}}
### **Using Export Method Exposed by Project Class**
After defining the image rendering parameters and project view, use the Export method of the Project class to render the project data to a Gantt chart image as shown in the code below:

{{< highlight java >}}

 project.Export(RenderFormat.Image, PresentationFormat.GanttChart, "project.html", new BaseImageRenderParam(null, new Point(), new Size(1200, 800), 100, 0, false), true, null, view);

{{< /highlight >}}
### **Complete Code Listing**
The complete source code listing in the form of a Console Application is as under:

{{< highlight java >}}

 using System;

using System.Collections.Generic;

using System.Linq;

using System.Text;

using Aspose.Tasks;

using Aspose.Tasks.Visualization;

using System.Collections;

using System.Drawing;


namespace RenderProject

{

    class Program

    {

        static void Main(string[] args)

        {

            Program prg = new Program();

            ProjectReader reader = new ProjectReader();

            Project project = reader.Read("Project1.mpp");

            //Create the view columns

            ArrayList columns = new ArrayList();

            columns.Add(new GanttChartColumn("Name", 100, new TaskToColumnTextConverter(prg.TaskName)));

            columns.Add(new GanttChartColumn("Notes", 100, new TaskToColumnTextConverter(prg.TaskNotes)));

            columns.Add(new GanttChartColumn("Resources", 200, new TaskToColumnTextConverter(prg.TaskResources)));

            //Create the view

            ProjectView view = new ProjectView(columns);

            //Render to image

            IRenderResult res = project.Export(RenderFormat.Image, PresentationFormat.GanttChart, "project.tiff", new BaseImageRenderParam(null,

                new Point(), new Size(1200, 800), 100, 0, true), true, null, view);

            //Create a new view

            ArrayList columns2 = new ArrayList();

            columns2.Add(new GanttChartColumn("Name", 100, new TaskToColumnTextConverter(prg.TaskNameHtml)));

            columns2.Add(new GanttChartColumn("Notes", 100, new TaskToColumnTextConverter(prg.TaskNotes)));

            columns2.Add(new GanttChartColumn("Resources", 200, new TaskToColumnTextConverter(prg.TaskResources)));

            //Create the view

            ProjectView view2 = new ProjectView(columns2);

            //Render to html

            project.Export(RenderFormat.Html, PresentationFormat.GanttChart, "project.html", new BaseImageRenderParam(null, new Point(), new Size(1200, 800), 100, 0, false), true, null, view2);

        }


        /// <summary>

        /// Forms task's name column.

        /// </summary>

        /// <param name="task">Current task.</param>

        /// <returns>Column's text.</returns>

        private string TaskName(Task task)

        {

            StringBuilder res = new StringBuilder();

            for (int i = 1; i < task.OutlineLevel; i++)

                res.Append("  ");

            res.AppendFormat("{0}. {1}", task.Id, task.Name);

            return res.ToString();

        }


        /// <summary>

        /// Forms task's name column.

        /// </summary>

        /// <param name="task">Current task.</param>

        /// <returns>Column's text.</returns>

        private string TaskNameHtml(Task task)

        {

            StringBuilder res = new StringBuilder();

            for (int i = 1; i < task.OutlineLevel; i++)

                res.Append("&nbsp;&nbsp;");

            res.AppendFormat("{0}. {1}", task.Id, task.Name);

            return res.ToString();

        }


        /// <summary>

        /// Forms task's notes column.

        /// </summary>

        /// <param name="task">Current task.</param>

        /// <returns>Column's text.</returns>

        private string TaskNotes(Task task)

        {

            if (task.NotesText != null)

                return task.NotesText;

            else

                return string.Empty;

        }


        /// <summary>

        /// Forms task's resources column.

        /// </summary>

        /// <param name="task">Current task.</param>

        /// <returns>Column's text.</returns>

        private string TaskResources(Task task)

        {

            StringBuilder res = new StringBuilder();

            Project project = task.ParentProject;

            bool bFirst = true;


            foreach (ResourceAssignment assignment in project.GetResourceAssignmentsByTask(task))

                if (assignment.Resource != null)

                {

                    if (!bFirst)

                        res.Append(", ");

                    res.Append(assignment.Resource.Name);

                    bFirst = false;

                }

            return res.ToString();

        }

    }

}

{{< /highlight >}}


The following is the image and HTML image produced with the example code: 

![todo:image_alt_text](display-multiple-columns-in-rendered-gantt-chart-image_2.png)




![todo:image_alt_text](display-multiple-columns-in-rendered-gantt-chart-image_3.png)
## **Conclusion**
Define image rendering parameters using one of the BaseImageRenderParam constructor overloads and project view to display selected columns in the output image and render a project file to a Gantt chart image using the Export method exposed by the Project class.

The rendered image may be customized to show the number of pages within the available range.
