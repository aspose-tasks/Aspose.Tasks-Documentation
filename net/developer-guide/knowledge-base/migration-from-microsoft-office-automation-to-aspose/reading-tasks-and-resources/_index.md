---
title: Reading Tasks and Resources
description: "Learn how to read tasks and resources from the Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET. in comparison with Microsoft Office Automation Tools."
type: docs
weight: 10
url: /net/reading-tasks-and-resources/
---

{{% alert color="primary" %}} 

While working with MPP files, you might need to read tasks and resources from your project. This article gives a small idea about how to load MPP files in your .NET applications and read tasks or resources from your projects using [VSTO](/tasks/net/reading-tasks-and-resources/) and [Aspose.Tasks for .NET](/tasks/net/reading-tasks-and-resources/).

{{% /alert %}} 
## **Read Tasks and Resources Using VSTO**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **COM components** tab.
3. Select Microsoft Project 12.0 Object Library and click **OK**.
   This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.
4. Use the code from the following example to read tasks and resources.
### **Code Examples - VSTO**


{{< highlight csharp >}}
// Create Application object
Application projectApplication = new ApplicationClass();
object missingValue = System.Reflection.Missing.Value;
// Open an MPP file
projectApplication.FileOpenEx(@"C:\Project1.mpp",

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

    missingValue, missingValue, missingValue, missingValue,

    missingValue);

// Create a Project object by assigning active project

Project project = projectApplication.ActiveProject;

// Loop through each task and read information related to tasks

foreach (Task task in project.Tasks)

{

    Console.WriteLine("Reading Task " + task.Name);

    Console.WriteLine("\nID: " + task.ID);

    Console.WriteLine("Start: " + task.Start);

    Console.WriteLine("Finish: " + task.Finish);

    Console.WriteLine("\n===========================\n");

}

// Loop through each resource and read information related to resources

foreach (Resource resource in project.Resources)

{

    string resourceType = null;

    switch (resource.Type)

    {

        case PjResourceTypes.pjResourceTypeCost: 

            resourceType = "Cost";

            break;

        case PjResourceTypes.pjResourceTypeMaterial: 

            resourceType = "Material";

            break;

        case PjResourceTypes.pjResourceTypeWork: 

            resourceType = "Work";

            break;

    }

    Console.WriteLine("Reading Resource " + resource.Name);

    Console.WriteLine("\nID: " + resource.ID);

    Console.WriteLine("Type: " + resourceType);

    Console.WriteLine("\n===========================\n");

}

Console.ReadLine();

{{< /highlight >}}
## **Read Tasks and Resources Using Aspose.Tasks for .NET**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select **Add Reference**, then select the **.NET** tab.
3. Select **Aspose.Tasks** and then click **OK**.
   This imports the Aspose.Tasks namespace at the start of the code.
4. Use the code from the following example to read tasks and resources.
### **Code Examples - Aspose.Tasks**


{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-KnowledgeBase-ReadTaskAndResources-ReadTaskAndResources.cs" >}}
