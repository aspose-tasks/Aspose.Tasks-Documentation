---
title: Convert Project Pages to Separate Image Files
description: "Learn how to convert Microsoft Project (MPP/XML) files to several JPEG files using Aspose.Tasks for C++."
keywords: "Convert Microsoft Project (MPP/XML) to JPEG, Convert MPP to JPEG, Export MPP Project to JPEG, save project data to several JPEG, Save MPP as JPEG, Aspose.Tasks for C++"
type: docs
weight: 80
url: /cpp/convert-project-pages-to-separate-image-files/
---

{{% alert color="primary" %}} 

To print a Project's pages to separate output files, use the ImageSaveOptions.SaveToSeparateFiles property. It specifies whether to save pages to separate files or not. Also, the API provides the ImageSaveOptions.Pages property that contains a list of page numbers to save when saving project layouts to separate files. All pages are saved if this list is empty and ImageSaveOptions.SaveToSeparateFiles is set to true.

{{% /alert %}}

## **Printing Project Pages to Separate Files**
The following code example demonstrates how to print individual pages in a project to separate files.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-PrintProjectPagesToSeparateFiles-PrintProjectPagesToSeparateFiles.cpp" >}}
