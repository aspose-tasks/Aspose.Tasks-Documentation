---
title: Rendering Task Usage View
type: docs
weight: 250
url: /java/rendering-task-usage-view/
---

{{% alert color="primary" %}} 

Aspose.Tasks supports rendering project tasks to a variety of formats, such as PDF. Task usage can be rendered using Aspose.Tasks' PresentationFormat with different timescale settings like Days, ThirdofMonths and Months.

{{% /alert %}} 
## **Rendering Task Usage View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the Project Reader.
1. Read the source MPP file.
1. Initiate the SaveOptions object with required timescale settings.
1. Set the presentation format to TaskUsage.
1. Render the project to PDF output.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-RenderTaskUsage-render-task-usage.java" >}}
### **Rendering Details Column to Output in Task Usage Veiw**
Details column included in the MPP file can be rendered to the output using the View's DisplayDetailsHeaderColumn property. The following code sample illustrates the usage of this property.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-RenderDetailColumnsTaskUsage-render-detail-column-task-usage.java" >}}
