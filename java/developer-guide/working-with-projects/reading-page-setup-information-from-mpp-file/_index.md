---
title: Reading Page Setup Information from MPP File
description: "Learn how to read Microsoft Project (MPP/XML) page setup information using Aspose.Tasks for Java."
type: docs
weight: 50
url: /java/reading-page-setup-information-from-mpp-file/
---

Aspose.Tasks for Java API provides the capability to read the Header and Footer information from MPP file. The API has classes mapped to each tab of Microsoft Project Page Setup dialog as detailed in the section below.

## **Reading Page Setup Information from MPP File**
Microsoft Project Page Setup dialog box has 6 tabs (see screenshot). These tabs are mapped to new classes:
- Page tab -> Aspose.Tasks.Visualization.PageSettings class
- Margins tab -> Aspose.Tasks.Visualization.PageMargins class
- Header, footer tabs -> Aspose.Tasks.Visualization.HeaderFooterInfo class
- Legend tab -> Aspose.Tasks.Visualization.PageLegend class
- View tab -> Aspose.Tasks.Visualization.PageViewSettings class

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ReadPageSetupInformation-reading-a-page-setup.java" >}}
