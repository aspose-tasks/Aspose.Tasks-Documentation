---
title: Reading the Critical Path in VSTO and Aspose.Tasks
type: docs
weight: 70
url: /net/reading-the-critical-path-in-vsto-and-aspose-tasks/
---

## **Code Examples**
### **VSTO**
Following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the COM components tab.
3. Select the Microsoft Project 12.0 Object Library and then click OK.
4. This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.Use the code from the following example to read critical tasks. 

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

// Enumerate the tasks

foreach (Task task in project.Tasks)

{

	//Get critical tasks

	if (task != null)

		if ((bool)task.Critical)

		{

			Console.WriteLine(task.ID + "  " + task.Name);

			Console.WriteLine(task.Start);

			Console.WriteLine(task.Finish + "\n");

		}

}

// Make sure to clean up and close the file

projectApplication.FileCloseAll(PjSaveType.pjDoNotSave);

{{< /highlight >}}
### **Aspose.Tasks**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the .NET tab.
3. Select Aspose.Tasks and click OK.
4. This imports the Aspose.Tasks namespace at the start of the code.
5. Use the code from the following example to read tasks and resources. 

{{< highlight csharp >}}

 using Aspose.tasks

//Open project file

string fileName = "Project.mpp";

ProjectReader reader = new ProjectReader();

Project project = reader.Read(fileName);

// Get the critical path

ArrayList criticalPath = new ArrayList(project.GetCriticalPath());

// Enumerate the tasks in the critical path

foreach (Aspose.Tasks.Task task in criticalPath)

{

	Console.WriteLine(task.Id + "  " + task.Name);

	Console.WriteLine(task.Start);

	Console.WriteLine(task.Finish + "\n");

}

{{< /highlight >}}
## **Download Sample Code**
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/download/AsposeTaskNETVsVSTOProjectv1.1/Reading.the.Critical.Path.Aspose.Tasks.zip)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-vsto/downloads/Reading%20the%20Critical%20Path%20\(Aspose.Tasks\).zip)
