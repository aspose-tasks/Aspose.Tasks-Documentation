---
title: Managing Currency Codes
type: docs
weight: 10
url: /java/managing-currency-codes/
---

## **Managing Currency Codes**
The CurrencyCode property exposed by the [Project](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Project)
class is used to set or get the three letter currency code for a project. This property supports the string data type.

To see a project's currency code in Microsoft Project:

1. On the **Tools** menu, select **Options**.
1. Select the **View** tab

**Currency codes in Microsoft Project** 

![todo:image_alt_text](managing-currency-codes_1.png)
### **Setting Currency using Aspose.Tasks**
The following example shows how to set these properties.

**Java**

{{< highlight java >}}

 Project prj = new Project();

prj.set(Prj.CURRENCY_CODE, "USD");

{{< /highlight >}}
### **Getting Currency Code using Aspose.Tasks**
These properties can be accessed using the project's CurrencyCode property.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Currencies-CurrencyCodes-getting-currency-codes.java" >}}
