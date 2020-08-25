---
title: Saving Project Data to Excel Format
type: docs
weight: 10
url: /java/saving-project-data-to-excel-format/
---

{{% alert color="primary" %}} 

This articles shows how to save project data to XLSX format using Aspose.Tasks.

{{% /alert %}} 
## **Saving Project Data to Excel Format**
The [Project](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Project) class exposes the save method which is used to save a project in various formats. The save method allows you to save project tasks, resources and assignments to separate worksheets to XLSX format using the SaveFileFormat enumeration type.

To save a project to XLSX:

1. Load a Microsoft Project file.
1. Save the project to XLSX using SaveFileFormat.XLSX.
### **Saving a Project as XLSX**
The following lines of code shows how to achieve this using Java



{{< gist "aspose-tasks" "378a8af8eeb0c3aa8f0e0095b3bd1d94" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveDataToExcel-saving-project-to-xlsx.java" >}}
### **Save Project Data to Spreadsheet2003 XML**
There are two ways to save data to Spreadsheet2003 XML format: default, or using [save options](/tasks/java/saving-project-data-to-excel-format/). Using the SaveFileFormat instance, the default view data is saved.

{{< gist "aspose-tasks" "378a8af8eeb0c3aa8f0e0095b3bd1d94" "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveDataToExcel-saving-project-to-spreadsheet2003.java" >}}
