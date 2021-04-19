---
title: Licensing
description: "Aspose.Tasks for C++ provides different plans for purchase or offers a Free Trial and a 30-day Temporary License for evaluation using Licensing policies."
type: docs
weight: 40
url: /cpp/licensing/
---

## **Evaluate Aspose.Tasks**
A free evaluation version of Aspose.Tasks for C++ can be downloaded from the downloads section of Aspose [website](https://downloads.aspose.com/tasks/cpp).

{{% alert color="primary" %}}

If you want to test Aspose.Tasks without evaluation version limitations, you can also request a 30 Day Temporary License. Please refer to [How to get a Temporary License](https://purchase.aspose.com/temporary-license)?

{{% /alert %}}

### **PDF Creator Information**
- Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Tasks for C++ x.x.x will be displayed against these fields.

### **Evaluation Limitations**
The evaluation version provides all the features except the following:

#### **DateTime Limitation**
The date year will be converted to 2000 in the projects that will be written through Aspose.Tasks for C++ as explained in the following code example. This example tries to create a project with two tasks through Aspose.Tasks for C++ without using a license file.

The project file created from the code looks like the one below in Microsoft Project. Note that the Start and Finish dates for Task1 have been converted from 06-Apr-2010 to 06-Apr-2000. Similarly, the Start and Finish dates for Task2 have been converted from 10-Apr-2010 to 10-Apr-2000. These dates are written with the same original year if the project is created using a licensed version of Aspose.Tasks for C++.

|**Date changes in the evaluation version of Aspose.Tasks**|
| :- |
|![reset task dates on evaluation version of Aspose.Tasks for C++](licensing_1.png)|

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Licensing-EvaluationDateTimeLimitations-DateTimeLimitations.cpp" >}}

#### **MPP Write Support**
Aspose.Tasks for C++ supports reading MPP files, updating the project summary information and then writing updated project files in original MPP format. That is if original MPP format belongs to Microsoft Project 2003 version, the MPP file updated through Aspose.Tasks for C++ API will also be in Microsoft Project 2003 MPP format. The same is valid for Microsoft Project 2007, 2010 and 2013 MPP formats. However, this support is only available in licensed versions of Aspose.Tasks for C++.

## **Applying the License**
Once you are happy with your evaluation of Aspose.Tasks for C++, buy a license at the Aspose [website](https://purchase.aspose.com/buy). Make yourself familiar with the different [licenses](https://purchase.aspose.com/policies/license-types/) offered. If you have any questions, [contact the Aspose sales team](https://about.aspose.com/contact) and they'll be happy to help you.

Every Aspose license carries a one-year [subscription](https://purchase.aspose.com/policies/subscriptions) for free upgrades to any new versions or fixes that come out during this time. Technical support is free and unlimited and provided both to licensed and evaluation users.

The license is a plain-text XML file that contains details such as the product name, number of licensed developers, subscription expiry date and so on. The file is digitally signed, so do not modify the file: even adding an extra line break to the file invalidates it.

### **When to Apply a License**
Follow these simple rules:

- The license only needs to be set once per application domain.
- You need to set the license before using any other Aspose.Tasks for C++ classes.
- Calling SetLicense multiple times is not harmful but wastes processor time.
- If you are developing a Windows Forms or console application, call SetLicense in your startup code, before using Aspose.Tasks for C++ classes.
- Do not call SetLicense from within the Page_Load methods since it means the license will be loaded every time a web page is loaded.
- If you are developing a class library, call SetLicense from a static constructor of your class that uses Aspose.Tasks. The static constructor executes before an instance of your class is created making sure that the Aspose.Tasks for C++ license is properly set.

### **Applying a License**
Use the **License.SetLicense** method to licensing the component. The easiest way to set a license is to put the license file in the same folder as the Aspose.Tasks.dll and specify the file name, without a path, as shown below.

#### **Applying a License Using File or Stream**
This code snippet initializes a license stored in a file or in an embedded resource.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Licensing-ApplyLicenseUsingFile-ApplyLicenseUsingFile.cpp" >}}

This code snippet initializes a license from a stream.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Licensing-ApplyLicenseUsingStream-ApplyLicenseUsingStream.cpp" >}}

#### **Applying Licensing Using an Embedded Resource**
Another neat way of packaging the license with your application and making sure it will not be lost, is to include it as an embedded resource into one of the assemblies that call the component's DLL (included in Aspose.Email). To include the license file as an embedded resource, perform the following steps:

1. In Visual Studio .NET, including the license (.lic) file into the project using the **Add Existing Item** on the **File** menu.
2. Select the file in the Solution Explorer.
3. Set **Build Action** to **Embedded Resource** in the Properties window.

To access the license embedded in the assembly (as an embedded resource), you don't have to call the Microsoft .NET Framework's System.Reflection.Assembly class' GetExecutingAssembly and GetManifestResourceStream methods. Instead, just add the license file as an embedded resource to your project and pass the name of the license file to the License class' SetLicense method. The License class will automatically find the license file in the embedded resources.
