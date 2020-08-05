---
title: Working with Page Header Footer
type: docs
weight: 90
url: /net/working-with-page-header-footer/
---

## **Reading Header and Footer Information from MPP file**
Aspose.Tasks API provides the capability to read the Header and Footer information from MPP file. The API has classes mapped to each tab of MS Project Page Setup dialog as detailed in the section below.

- MS Project Page Setup dialog box has 6 tabs (see screenshot). These tabs are mapped to new classes:
  - Page tab -> Aspose.Tasks.Visualization.PageSettings class
  - Margins tab -> Aspose.Tasks.Visualization.PageMargins class
  - Header, footer tabs -> Aspose.Tasks.Visualization.HeaderFooterInfo class
  - Legend tab -> Aspose.Tasks.Visualization.PageLegend class
  - View tab -> Aspose.Tasks.Visualization.PageViewSettings class

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ReadHeaderFooterInfo-ReadHeaderFooterInfo.cs" >}}
## **Adding Image to Page Header/Footer**
Aspose.Tasks API provides the capability to manipulate the document's page header and footer information. The example below shows how to add image to page's header.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-AddImageToPageHeaderFooter-AddImageToPageHeaderFooter.cs" >}}
