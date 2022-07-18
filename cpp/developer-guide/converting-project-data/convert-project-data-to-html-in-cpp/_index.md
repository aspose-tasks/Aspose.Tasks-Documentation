---
title: Convert Project Data to HTML in C++
description: "Learn how to convert Microsoft Project (MPP/XML) projects to HTML using Aspose.Tasks for C++."
type: docs
weight: 20
url: /cpp/convert-project-data-to-html-in-cpp/
---

{{% alert color="primary" %}}

Microsoft Project (MSP) allows developers to save project data (MPP/XML) to HTML. Aspose.Tasks for C++ API also allows you to save project data to the same formats similar to MSP. This is achieved using the standard Save method exposed by the [Project](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.project) class.

{{% /alert %}}

## **Saving Project Data as HTML**
Aspose.Tasks for C++ can export project data to HTML format. It allows to save all the data to HTML or export only required pages to HTML by using the SaveOptions as shown in the following code samples.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectDataAsHTML-SaveProjectDataAsHTML.cpp" >}}

### **Controlling Document Header Name during Export to HTML**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-ControlHeaderNameDuringHTMLExport-ControlHeaderNameDuringHTMLExport.cpp" >}}

### **Saving Fonts, Images and CSS Styles Separately**
Aspose.Tasks for C++ API gives you enough power to save fonts, images, and CSS styles information separately to files while saving Project Data to HTML. This is achieved using the HtmlSaveOptions class by providing information about CSS, Font and Image destinations.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-ResourcePrefixForNestedResources-ResourcePrefixForNestedResources.cpp" >}}

### **Adding Page Prefix in CSS Classes While Exporting to HTML**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-AddingCssStylePrefix-AddingCssStylePrefix.cpp" >}}
