---
title: Task Views
type: docs
weight: 220
url: /cpp/task-views/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ API supports rendering project tasks to a variety of formats, such as PDF. Task usage can be rendered using Aspose.Tasks' PresentationFormat with different timescale settings like Days, ThirdOfMonths and Months.

{{% /alert %}} 
## **Rendering Task Usage View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the Project class.
2. Read the source MPP file.
3. Initiate the SaveOptions object with required timescale settings.
4. Set the presentation format to TaskUsage.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-RenderTaskUsageView-RenderTaskUsageView.cpp" >}}
## **Rendering Details Column to Output in Task Usage View**
Details column included in the MPP file can be rendered to the output using the View's DisplayDetailsHeaderColumn property. This includes the list of following supported fields:

- Work
- Actual Work
- Actual Overwork time
- Baseline Work
- Baseline 1-10 Work

The following code example illustrates the usage of this property.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-RenderTaskUsageViewWithDetails-RenderTaskUsageViewWithDetails.cpp" >}}
## **Rendering Task Sheet View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the Project class.
2. Read the source MPP file.
3. Initiate the SaveOptions object with required timescale settings.
4. Set the presentation format to TaskSheet.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-RenderTaskSheetView-RenderTaskSheetView.cpp" >}}
