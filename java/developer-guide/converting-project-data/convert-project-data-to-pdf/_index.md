---
title: Convert Project Data to PDF
type: docs
weight: 60
url: /java/convert-project-data-to-pdf/
---

{{% alert color="primary" %}} 

This article shows how to render project data to PDF using Aspose.Tasks for Java. The API provides the following capabilities while rendering project data to various output formats including PDF.

{{% /alert %}} 
## **PDF Creator Information**
- Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Tasks for Java x.x.x will be displayed against these fields.
## **Saving a Project as a PDF**
The [Project](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Project) class exposes the Save method which is used to save a project in various formats. The Save method allows you to render project data to PDF using the SaveFileFormat enumeration type.

To save a project to PDF:

1. Load a Microsoft Project file.
1. Save the project to PDF using SaveFileFormat.PDF.

The following lines of code show how to achieve this.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveAsPdf-saving-as-pdf.java" >}}


### **Supported Graphical Column Indicators**
Aspose.Tasks draw graphical column indicators while rendering project data to PDF. Following are the graphical indicators supported by Aspose.Tasks.

|**Indicator Type**|**Graphical Representators**|
| :- | :- |
|Task Indicators|![todo:image_alt_text](convert-project-data-to-pdf_1.png)|
|Resource Indicators|![todo:image_alt_text](convert-project-data-to-pdf_2.png)|
|Assignment Indicators|![todo:image_alt_text](convert-project-data-to-pdf_3.png)|

### **Saving to Multiple PDF Files**
In order to save the project data to multiple PDF files, set the SaveToSeparateFiles flag to true.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveAsPdf-save-to-multiple-pdf-pages.java" >}}


### **Customising TextStyle for Project Data**
Aspose.Tasks allows you to customise the text style for overallocated resources. By default, the style for overallocated resources is similar to Microsoft Project (MSP), that is, it is red and bold. TextItemType.OverallocatedResources enables you to customise the colour and style for overallocated resources. The example below shows how.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveAsPdf-customizing-text-style-for-project-data.java" >}}


### **Customising Date Format**
Aspose.Tasks give developers control over date formatting when rendering project data to output. The following example shows how to use the DateFormat enumerator to specify the date format.

**Java**

{{< highlight java >}}

 Project project = new Project();

Date dt = new Date();

project.setStartDate(dt);

// By default project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14)

// customize DateFormat (September 22, 2014)

project.setDateFormat(DateFormat.Date_mmmm_dd_yyyy);

project.save("saved.pdf", SaveFileFormat.PDF);

//Export to date format 19/07/2016

project.setDateFomrat(DateFormat.DateDdMmYyyy);

project.save("p2.pdf", SaveFileFormat.PDF);

{{< /highlight >}}
