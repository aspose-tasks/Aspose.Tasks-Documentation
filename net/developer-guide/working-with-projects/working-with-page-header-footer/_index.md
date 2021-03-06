---
title: Working with Page Header Footer
description: "Learn how to read header and footer information from Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET."
type: docs
weight: 90
url: /net/working-with-page-header-footer/
---

## **Reading Header and Footer Information from MPP file**
Aspose.Tasks for .NET API provides the capability to read the Header and Footer information from MPP file. The API has classes mapped to each tab of Microsoft Project Page Setup dialog as detailed in the section below.

- Microsoft Project Page Setup dialog box has 6 tabs. These tabs are mapped to new classes:
  - Page tab -> Aspose.Tasks.Visualization.PageSettings class
  - Margins tab -> Aspose.Tasks.Visualization.PageMargins class
  - Header, footer tabs -> Aspose.Tasks.Visualization.HeaderFooterInfo class
  - Legend tab -> Aspose.Tasks.Visualization.PageLegend class
  - View tab -> Aspose.Tasks.Visualization.PageViewSettings class

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ReadHeaderFooterInfo.cs" >}}

## **Adding Image to Page Header/Footer**
Aspose.Tasks for .NET API provides the capability to manipulate the document's page header and footer information. The example below shows how to add image to page's header.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-AddImageToPageHeaderFooter.cs" >}}
