---
title: Rendering Task Usage View
description: "Learn how to render Microsoft Project (MPP/XML) task usage views using Aspose.Tasks for .NET."
type: docs
weight: 250
url: /net/rendering-task-usage-view/
---

Aspose.Tasks for .NET supports rendering project tasks to a variety of formats, such as PDF. Task usage can be rendered using [PresentationFormat](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat) of Aspose.Tasks with different timescale settings like Days, ThirdOfMonths and Months.

## **Rendering Task Usage View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the [Project](https://reference.aspose.com/tasks/net/aspose.tasks/project) class.
2. Read the source MPP file.
3. Initiate the [SaveOptions](https://reference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions) object with required timescale settings.
4. Set the presentation format to TaskUsage.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-RenderTaskUsageView.cs" >}}

## **Rendering Details Column to Output in Task Usage View**
Details column included in the MPP file can be rendered to the output using the View's DisplayDetailsHeaderColumn property. This includes the list of following supported fields:

- Work
- Actual Work
- Actual Overwork time
- Baseline Work
- Baseline 1-10 Work

The following code sample illustrates the usage of this property.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-RenderTaskUsageViewWithDetails.cs" >}}
