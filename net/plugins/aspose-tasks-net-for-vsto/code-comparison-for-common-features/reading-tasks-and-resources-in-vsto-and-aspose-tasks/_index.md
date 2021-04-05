---
title: Reading Tasks and Resources in VSTO and Aspose.Tasks
type: docs
weight: 60
url: /net/reading-tasks-and-resources-in-vsto-and-aspose-tasks/
---

## **Code Examples**
### **VSTO**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the COM components tab.
3. Select Microsoft Project 12.0 Object Library and click OK.
4. This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.Use the code from the following example to read tasks and resources.

{{< highlight csharp >}}

 //Create Application object

Application projectApplication = new MSProject.Application();

object missingValue = System.Reflection.Missing.Value;

//Open an MPP file

projectApplication.FileOpenEx("Project1.mpp",

	missingValue, missingValue, missingValue, missingValue,

	missingValue, missingValue, missingValue, missingValue,

	missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

	missingValue, missingValue, missingValue, missingValue,

	missingValue);

//Create a Project object by assigning active project

Project project = projectApplication.ActiveProject;

//Loop through each task and read information related to tasks

foreach (Task task in project.Tasks)

{

	Console.WriteLine("Reading Task " + task.Name);

	Console.WriteLine("\nID: " + task.ID);

	Console.WriteLine("Start: " + task.Start);

	Console.WriteLine("Finish: " + task.Finish);

	Console.WriteLine("\n===========================\n");

	//Read any other information you need

}

//Loop through each resource and read information related to resources

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

	//Read any other information you need

}

Console.ReadLine();

{{< /highlight >}}
### **Aspose.Tasks**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the .NET tab.
3. Select Aspose.Tasks and then click OK.
4. This imports the Aspose.Tasks namespace at the start of the code.Use the code from the following example to read tasks and resources.

{{< highlight csharp >}}

 using Aspose.tasks;

//Load MPP file using project reader

ProjectReader reader = new ProjectReader();

Project project = reader.Read("Project.mpp");

//Load all tasks

ArrayList allTasks =new ArrayList(project.RootTask.Children);


//Loop through each task and read information related to tasks

foreach (Aspose.Tasks.Task task in allTasks)

{

	Console.WriteLine("Reading Task " + task.Name);

	Console.WriteLine("\nID: " + task.Id);

	Console.WriteLine("Start: " + task.Start);

	Console.WriteLine("Finish: " + task.Finish);

	Console.WriteLine("\n===========================\n");

	//Read any other information you need

}

//Loop through each resource and read information related to resources

foreach (Resource resource in project.Resources)

{

	string resourceType = null;

	switch (resource.Type)

	{

		case ResourceType.Material:

			resourceType = "Material";

			break;

		case ResourceType.Work:

			resourceType = "Work";

			break;

		default:

			resourceType = "Cost";

			break;

	}

	Console.WriteLine("Reading Resource " + resource.Name);

	Console.WriteLine("\nID: " + resource.Id);

	Console.WriteLine("Type: " + resourceType);

	Console.WriteLine("\n===========================\n");

	//Read any other information you need

}

Console.ReadLine();

{{< /highlight >}}
## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/download/AsposeTaskNETVsVSTOProjectv1.1/Reading.Tasks.and.Resources.Aspose.Tasks.zip)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-vsto/downloads/Reading%20Tasks%20and%20Resources%20(Aspose.Tasks).zip)
