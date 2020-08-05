---
title: Printing Project Pages to Separate Image Files
type: docs
weight: 50
url: /java/printing-project-pages-to-separate-image-files/
---

## **Saving Project Pages to Separate Files**
To print the pages in a Project to separate output files, use the ImageSaveOptions.SaveToSeparateFiles property. This specifies whether to save project pages to separate files or not. Also, the API provides the ImageSaveOptions.Pages property which contains a list of page numbers to save when saving project layout to separate files. All pages are saved if this list is empty and ImageSaveOptions.SaveToSeparateFiles is set to true.

The code sample below shows how to print pages to separate files.



{{< gist "aspose-tasks" "378a8af8eeb0c3aa8f0e0095b3bd1d94" "Examples-src-main-java-com-aspose-tasks-examples-Projects-PrintPagesToSeparateImage-saving-project-pages-to-seperate-images.java" >}}
