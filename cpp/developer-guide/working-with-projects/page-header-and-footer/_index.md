---
title: Working with Page Header Footer
description: "Learn how to read header and footer information from Microsoft Project (MPP/XML) files using Aspose.Tasks for C++."
type: docs
weight: 60
url: /cpp/page-header-and-footer/
---

## **Reading Header and Footer Information from MPP file**
Aspose.Tasks for C++ API provides the capability to read the Header and Footer information from MPP file. The API has classes mapped to each tab of Microsoft Project Page Setup dialog as detailed in the section below.

- Microsoft Project Page Setup dialog box has 6 tabs (see screenshot). These tabs are mapped to new classes:
  - Page tab ->[Aspose.Tasks.Visualization](https://reference.aspose.com/tasks/cpp/namespace/aspose.tasks.visualization)[.PageSettings](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.visualization.page_settings) class
  - Margins tab -> [Aspose.Tasks.Visualization.PageMargins](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.visualization.page_margins) class
  - Header, footer tabs -> [Aspose.Tasks.Visualization.HeaderFooterInfo](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.visualization.header_footer_info) class
  - Legend tab -> [Aspose.Tasks.Visualization.PageLegend](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.visualization.page_legend) class
  - View tab -> [Aspose.Tasks.Visualization.PageViewSettings](https://reference.aspose.com/tasks/cpp/class/aspose.tasks.visualization.page_view_settings) class

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ReadHeaderFooterInfo-ReadHeaderFooterInfo.cpp" >}}

## **Adding Image to Page Header/Footer**
Aspose.Tasks for C++ API provides the capability to manipulate the document's page header and footer information. The code example given below demonstrates how to add image to page's header.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-AddImageToPageHeaderFooter-AddImageToPageHeaderFooter.cpp" >}}
