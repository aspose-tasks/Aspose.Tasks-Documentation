---
title: Managing Currency Codes
description: "Learn how to manage currency codes in Microsoft Project (MPP/XML) files using Aspose.Tasks for Java."
type: docs
weight: 10
url: /java/managing-currency-codes/
---

## **Managing Currency Codes**
The CurrencyCode property exposed by the [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/project)
class is used to set or get the three-letter currency code for a project. This property supports the string data type.

To see a project's currency code in Microsoft Project:

1. On the **Tools** menu, select **Options**.
2. Select the **View** tab

**Currency codes in Microsoft Project**

![show currency codes in Microsoft Project](managing-currency-codes_1.png)

### **Setting Currency using Aspose.Tasks**
The following example shows how to set these properties.

{{< highlight java >}}
Project prj = new Project();
prj.set(Prj.CURRENCY_CODE, "USD");
{{< /highlight >}}

### **Getting Currency Code using Aspose.Tasks**
These properties can be accessed using the project's CurrencyCode property.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Currencies-CurrencyCodes-getting-currency-codes.java" >}}
