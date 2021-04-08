---
title: Currency Properties
description: "Learn how to manage Microsoft Project (MPP/XML) currency properties using Aspose.Tasks for C++."
type: docs
weight: 50
url: /cpp/currency-properties/
---

## **Overview**
Microsoft Project lets users set which currency costs are shown in, in a project. They can define set the currency code, numbers after the decimal point and currency symbol so that costs show in an easy to read and intuitive way. Aspose.Tasks for C++ supports these features and provides a series of properties that help developers set and control currency properties. This topic explains how to read currency properties, and how to set them.

Aspose.Tasks provides properties exposed by the [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) class, for managing currency properties:

- [CurrencyCode](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#acc9204a460e7507e5b366d965252fae5): the three-letter currency code, for example, USD, GBP or AUD, passed as a string.
- [CurrencyDigits](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a0a9077f31756b5261a8386138902989d): the number of numbers after the decimal point, for example, 2 (100.00) or 3 (100.000), passed as an integer.
- [CurrencySymbol](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#ab979d548829ea8f9ed20b98214c69304): the currency symbol, for example, $ or £, passed as a string.
- [CurrencySymbolPosition](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a25a9b67902c0655d1b16b00ac9ef59d5): the position of the currency symbol, for example before ($100) or after (100$). CurrencySymbolPosition takes a value from the [CurrencySymbolPositionType](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.prj#a25a9b67902c0655d1b16b00ac9ef59d5) enumeration.

### **Reading Currency Properties**
The code example given below demonstrates how to read a project's currency properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-ReadCurrencyProperties-ReadCurrencyProperties.cpp" >}}

### **Writing Currency Properties**
To see the currency properties in Microsoft Project:

1. Open the project file.
2. On the **Tools** menu, select **Options**.
3. Click the **View** tab and for Project 2016 **Display**. It will look like the one shown below.

![edit currency properties in Microsoft Project 2016](currency-properties_1.png)

The code example given below demonstrates how to write currency properties to the project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-WriteCurrencyProperties-WriteCurrencyProperties.cpp" >}}
