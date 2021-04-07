---
title: Create Resources and Link in VSTO and Aspose.Tasks
type: docs
weight: 40
url: /net/create-resources-and-link-in-vsto-and-aspose-tasks/
---

## **Code Examples**
### **VSTO**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the COM components tab.
3. Select Microsoft Project 12.0 Object Library and click OK. This imports the Microsoft.Office.Interop.MSProject namespace at the start of the code.Use the code from the following example to read tasks and resources.

{{< highlight csharp >}}
//Create an Application object
Microsoft.Office.Interop.MSProject.Application projectApplication = new MSProject.Application();
object missingValue = System.Reflection.Missing.Value;
//Open an MPP file
projectApplication.FileOpenEx("Project1.mpp",
	missingValue, missingValue, missingValue, missingValue,
	missingValue, missingValue, missingValue, missingValue,
	missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,
	missingValue, missingValue, missingValue, missingValue,
	missingValue);
Microsoft.Office.Interop.MSProject.Project project = projectApplication.ActiveProject;
int iResourceId = 1;
foreach (Task tsk in project.Tasks)
{
	string developer = "Developer0" + iResourceId;
	project.Resources.Add(developer, iResourceId);
	tsk.Assignments.Add(tsk.ID, iResourceId, missingValue);
	iResourceId++;
}
projectApplication.FileCloseAll(Microsoft.Office.Interop.MSProject.PjSaveType.pjSave);
{{< /highlight >}}

### **Aspose.Tasks**
The following steps are required to accomplish this task:

1. Create a new project in Visual Studio.
2. In the Solution Explorer, right-click and select Add Reference, then select the .NET tab.
3. Select Aspose.Tasks and then click OK. This imports the Aspose.Tasks namespace at the start of the code.Use the code from the following example to create resources and link them to tasks. 

{{< highlight csharp >}}
Project prj = new Project("Project.mpp");
// Declare ChildTasksCollector class object
ChildTasksCollector collector = new ChildTasksCollector();
// Use TaskUtils to get all children tasks in RootTask
TaskUtils.Apply(prj.RootTask, collector, 0);
// Define Resources
ArrayList resources = new ArrayList();
for (int i = 1; i <= 5; i++)
{
	string developer = "Developer0" + i;
	// Create resource
	Resource rec = new Resource(developer);
	rec.Type = ResourceType.Work;
	// Add resource to project
	prj.Resources.Add(rec);
	// define assignment
	ResourceAssignment assignment = new ResourceAssignment((Aspose.Tasks.Task)collector.Tasks[i], rec);
	prj.ResourceAssignments.Add(assignment);
}
prj.CalcResourceUids();
prj.CalcResourceIds();
prj.CalcResourceFields();
prj.CalcResourceAssignmentUids();
prj.CalcResourceAssignmentIds();
prj.Save("Project1_CSharp_Aspose.mpp", Aspose.Tasks.Saving.SaveFileFormat.MPP);
{{< /highlight >}}

## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/download/AsposeTaskNETVsVSTOProjectv1.1/Create.Resources.and.Link.Aspose.Tasks.zip)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-vsto/downloads/Create%20Resources%20and%20Link%20(Aspose.Tasks).zip)
