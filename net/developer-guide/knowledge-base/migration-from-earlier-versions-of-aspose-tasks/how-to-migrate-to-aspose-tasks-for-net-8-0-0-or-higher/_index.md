---
title: How to Migrate to Aspose.Tasks for .NET 8.0.0 or higher
description: "Learn how to migrate from earlier versions of Aspose.Tasks for .NET 8.0.0 to the latest versions."
type: docs
weight: 90
url: /net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/
---

{{% alert color="primary" %}} 

Aspose.Tasks for .NET 8.0.0 is a revamped version of the API that includes considerable changes from usage perspective. Key differences of both the implementations include:

- Legacy API allowed to set public fields of various project data classes such as Project, Tasks, Resource, etc. while the new implementation introduces Set and Get methods to achieve the same
- Recalculate methods required to be called manually by user in the legacy API after certain operations such as Resource Assignments. The new Aspose.Tasks for .NET API performs most of such calculations automatically without user intervention required.
- The new API provides manual as well as automatic recalculation modes similar to Microsoft Project (MSP). Manual mode calculates only the necessary fields whereas automatic mode recalculates everything.  This eliminates the need of calling recalculating methods manually and improves overall API usage.

This new API is incompatible with the Legacy API and the objective of this article is to help you migrate your code to the new API.  The article shows comparative code samples of the Legacy and the new API implementation, and includes:

- [Setting Default Project Properties](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)
- [Creating Calendar and Adding to Project](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)
- [Make Standard Calendar](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)
- [Adding Task to Project](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)
- [Adding a Resource to Project](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)
- [Create Resource Assignment](/tasks/net/how-to-migrate-to-aspose-tasks-for-net-8-0-0-or-higher/)

{{% /alert %}} 

### **Setting Default Project Properties**
Aspose.Tasks' legacy API allowed setting default properties of a project by directly setting the public attributes of the Project class. In the new API implementation, however, it exposes Set and Get methods to achieve the same.

###### **Legacy API Code Sample**

{{< highlight csharp >}}
Project prj = new Project();
prj.IsScheduleFromStart = true;
prj.StartDate = DateTime.Now;
prj.DefaultStartTime = prj.StartDate;
prj.DefaultTaskType = TaskType.FixedDuration;
prj.DefaultStandardRate=15;
prj.DefaultOvertimeRate=12;
prj.DefaultTaskEVMethod = EarnedValueMethodType.PercentComplete;
prj.DefaultFixedCostAccrual = CostAccrualType.Prorated;
prj.Save( "Project4.xml" , Aspose.Tasks.Saving.SaveFileFormat.XML);
{{< /highlight >}}

{{< highlight csharp >}}
'Create a project instance
Dim prj As New Project()
prj.IsScheduleFromStart = True
prj.StartDate = DateTime.Now
prj.DefaultStartTime = prj.StartDate
prj.DefaultTaskType = TaskType.FixedDuration
prj.DefaultStandardRate = 15
prj.DefaultOvertimeRate = 12
prj.DefaultTaskEVMethod = EarnedValueMethodType.PercentComplete
prj.DefaultFixedCostAccrual = CostAccrualType.Prorated
prj.Save("Project4.xml", Aspose.Tasks.Saving.SaveFileFormat.XML)
{{< /highlight >}}

###### **New Aspose.Tasks for .NET 8.x Approach**
{{< highlight csharp >}}
Project project = new Project();
project.Set(Prj.ScheduleFromStart,true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime,project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);
project.Save("ProjectDefaultProps.xml", SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
Dim project As New Project()
project.[Set](Prj.ScheduleFromStart, True)
project.[Set](Prj.StartDate, DateTime.Now)
project.[Set](Prj.DefaultStartTime, project.[Get](Prj.StartDate))
project.[Set](Prj.DefaultTaskType, TaskType.FixedDuration)
project.[Set](Prj.DefaultStandardRate, 15)
project.[Set](Prj.DefaultOvertimeRate, 12)
project.[Set](Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete)
project.[Set](Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated)
project.Save("ProjectDefaultProps.xml", SaveFileFormat.XML)
{{< /highlight >}}

### **Creating and Adding Calendar to a Project**
In order for proper functionality of Calendar items added to the Project, the legacy API required to recalculate Calendar UIDs. In the new API, however, UIDs recalculation are automatically dealt and there is no need to call the calculations manually.

###### **Legacy API Code Sample**

{{< highlight csharp >}}
Project prj =  new Project();
Aspose.Tasks.Calendar cal1 = new  Aspose.Tasks.Calendar();
cal1.Name ="no info";
Aspose.Tasks.Calendar cal2 = new  Aspose.Tasks.Calendar(1);
cal2.Name = "no name";
Aspose.Tasks.Calendar cal3 = new  Aspose.Tasks.Calendar( "cal3" );
prj.Calendars.Add(cal1);
prj.Calendars.Add(cal2);
prj.Calendars.Add(cal3);
prj.CalcCalendarUids();
prj.Save( "Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
'Create a project instance
Dim prj As New Project()
'Define Calendar
Dim cal1 As New Aspose.Tasks.Calendar()
cal1.Name = "no info"
Dim cal2 As New Aspose.Tasks.Calendar(1)
cal2.Name = "no name"
Dim cal3 As New Aspose.Tasks.Calendar("cal3")
prj.Calendars.Add(cal1)
prj.Calendars.Add(cal2)
prj.Calendars.Add(cal3)
prj.CalcCalendarUids()
'Save the Project
prj.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML)
{{< /highlight >}}

###### **New Aspose.Tasks for .NET 8.x Approach**
**C#**

{{< highlight csharp >}}
//Create a project instance
Project prj = new Project();
Aspose.Tasks.Calendar cal1 = prj.Calendars.Add("no info");
Aspose.Tasks.Calendar cal2 = prj.Calendars.Add("no name");
Aspose.Tasks.Calendar cal3 = prj.Calendars.Add("cal3");
prj.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
'Create a project instance
Dim prj As New Project()
Dim cal1 As Aspose.Tasks.Calendar = prj.Calendars.Add("no info")
Dim cal2 As Aspose.Tasks.Calendar = prj.Calendars.Add("no name")
Dim cal3 As Aspose.Tasks.Calendar = prj.Calendars.Add("cal3")
prj.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML)
{{< /highlight >}}

### **Making A Standard Calendar**
Recalculating Calendar UIDs are no more required in the new ASpose.Tasks' API as compared to the legacy API.

###### **Legacy API Code Sample**
**C#**

{{< highlight csharp >}}
//Create a project instance
Project prj = new  Project();
//Define Calendar and make it standard
Aspose.Tasks.Calendar cal1 = new  Aspose.Tasks.Calendar("My Cal");
Aspose.Tasks.Calendar.MakeStandardCalendar(cal1);
prj.Calendars.Add(cal1);
prj.CalcCalendarUids();
prj.Save( "Project.Xml" , Aspose.Tasks.Saving.SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
'Create a project instance
Dim prj As New Project()
'Define Calendar and make it standard
Dim cal1 As New Aspose.Tasks.Calendar("My Cal")
Aspose.Tasks.Calendar.MakeStandardCalendar(cal1)
prj.Calendars.Add(cal1)
prj.CalcCalendarUids()
'Save the Project
prj.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML)
{{< /highlight >}}

###### **New Aspose.Tasks for .NET 8.x Approach**
**C#**

{{< highlight csharp >}}

 //Create a project instance

Project project = new Project();

//Define Calendar and make it standard

Aspose.Tasks.Calendar cal1 = project.Calendars.Add("My Cal");

Aspose.Tasks.Calendar.MakeStandardCalendar(cal1);

//Save the Project

project.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML);

{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}

 'Create a project instance

Dim project As New Project()

'Define Calendar and make it standard

Dim cal1 As Aspose.Tasks.Calendar = project.Calendars.Add("My Cal")

Aspose.Tasks.Calendar.MakeStandardCalendar(cal1)

'Save the Project

project.Save("Project.Xml", Aspose.Tasks.Saving.SaveFileFormat.XML)

{{< /highlight >}}
### **Create and Add Task to Project**
Creating a new task in the legacy API, it required to define a root task, add it to the project as its root task, and then add a new task to this root task as a child. The new API, however, doesn't need you to define the root task and takes care of it automatically while adding the first task to the project.
###### **Legacy API Code Sample**
**C#**

{{< highlight csharp >}}

 Project project = new Project();

Task rootTask = new Task();

Task tskGen = new Task("Task1");

tskGen.Id = 1;

tskGen.Uid = 1;

tskGen.Start = DateTime.Parse("17-Aug-2009 8:00 AM" );

tskGen.Finish = DateTime.Parse( "17-Aug-2009 5:00 PM" );

project.RootTask = rootTask;

project.RootTask.Children.Add(tskGen);

project.Save("Project.xml", SaveFileFormat.XML);

{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}

 Dim project As New Project()

Dim tskGen As New Task("Task1")

tskGen.Id = 1

tskGen.Uid = 1

tskGen.Start = DateTime.Parse("17-Aug-2009 8:00 AM")

tskGen.Finish = DateTime.Parse("17-Aug-2009 5:00 PM")

project.RootTask = rootTask

project.RootTask.Children.Add(tskGen)

project.Save("Project.xml", SaveFileFormat.XML)

{{< /highlight >}}
###### **New Aspose.Tasks for .NET 8.x Approach**
**C#**

{{< highlight csharp >}}

 Project project = new Project();

Task task = project.RootTask.Children.Add("Task 1");

task.Set(Tsk.Start, project.RootTask.Get(Tsk.Start).AddDays(1));

//set task start day

project.Save("CreateTasks.xml", SaveFileFormat.XML);

{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}

 Dim project As New Project()

Dim task As Task = project.RootTask.Children.Add("Task 1")

task.[Set](Tsk.Start, project.RootTask.[Get](Tsk.Start).AddDays(1))

'set task start day

project.Save("CreateTasks.xml", SaveFileFormat.XML)

{{< /highlight >}}

### **Create and Add Resource to Project**
Set and Get methods have been added to the Resource class of the API for manipulating attributes related to a project's Resource.
###### **Legacy API Code Sample**
**C#**

{{< highlight csharp >}}

 Project project = new Project();

Resource res =   Resource(new "Res1");

res.Id = 1;

res.Uid = 1;

res.Start = DateTime.Parse("19-Aug-2009 8:00 AM");

res.Finish = DateTime.Parse("19-Aug-2009 5:00 PM");

project.Resources.Add(res);

project.Save("Project.xml", SaveFileFormat.XML);

{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}

 Dim project As New Project()

Dim res As New Resource("Res1")

res.Id = 1

res.Uid = 1

res.Start = DateTime.Parse("19-Aug-2009 8:00 AM")

res.Finish = DateTime.Parse("19-Aug-2009 5:00 PM")

project.Resources.Add(res)

project.Save("Project.xml", SaveFileFormat.XML)

{{< /highlight >}}

###### **New Aspose.Tasks for .NET 8.x Approach**
**C#**

{{< highlight csharp >}}
Project project = new Project();
Resource rsc = project.Resources.Add("R1");
rsc.Set(Rsc.Start, DateTime.Parse("31-Aug-2014 8:00 AM"));
rsc.Set(Rsc.Finish, DateTime.Parse("31-Aug-2014 5:00 PM"));
project.Save("CreateResource.xml", SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
Dim project As New Project()
Dim rsc As Resource = project.Resources.Add("R1")
rsc.[Set](Rsc.Start, DateTime.Parse("31-Aug-2014 8:00 AM"))
rsc.[Set](Rsc.Finish, DateTime.Parse("31-Aug-2014 5:00 PM"))
project.Save("CreateResource.xml", SaveFileFormat.XML)
{{< /highlight >}}

### **Create and Add Resource Assignment to Project**
The ResourceAssignment class also introduces the Set and Get methods similar to other data collections of the API such as Tasks, Resources and Tasks Links.
###### **Legacy API Code Sample**
**C#**

{{< highlight csharp >}}
Project project = new Project();
Task tskRoot =  new Task();
Task task = new Task("Task");
Resource rsc = new Resource();
rsc.StandardRate=10;
rsc.OvertimeRate=15;
ResourceAssignment assignment = new ResourceAssignment(task, rsc);
assignment.Uid = 1;
assignment.Start = DateTime.Parse("18-Aug-2009 8:00 AM" );
assignment.Finish = DateTime.Parse("18-Aug-2009 5:00 PM" );
project.RootTask = tskRoot;
project.RootTask.Children.Add(task);
project.Resources.Add(res);
project.ResourceAssignments.Add(assignment);
project.Save("project.xml", SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
Dim project As New Project()
Dim tskRoot As New Task()
Dim task As New Task("Task")
Dim rsc As New Resource()
rsc.StandardRate = 10
rsc.OvertimeRate = 15
Dim assignment As New ResourceAssignment(task, rsc)
assignment.Start = DateTime.Parse("18-Aug-2009 8:00 AM" )
assignment.Finish = DateTime.Parse("18-Aug-2009 5:00 PM" )
assignment.Uid = 1
project.RootTask = tskRoot
project.RootTask.Children.Add(task)
project.Resources.Add(res)
project.ResourceAssignments.Add(assignment)
project.Save("project.xml", SaveFileFormat.XML)
{{< /highlight >}}

###### **New Aspose.Tasks for .NET 8.x Approach**
**C#**

{{< highlight csharp >}}
Project project = new Project();
Task task = project.RootTask.Children.Add("Task");
Resource rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);
ResourceAssignment assignment = project.ResourceAssignments.Add(task, rsc);
assignment.Set(Assn.Start,DateTime.Parse("18-Aug-2009 8:00 AM" );
assignment.Set(Assn.Finish, DateTime.Parse("18-Aug-2009 5:00 PM" );
project.Save("ResourceAssignments.xml", SaveFileFormat.XML);
{{< /highlight >}}

**VB.NET**

{{< highlight csharp >}}
Dim project As New Project()
Dim task As Task = project.RootTask.Children.Add("Task")
Dim rsc As Resource = project.Resources.Add("Rsc")
rsc.[Set](Rsc.StandardRate, 10)
rsc.[Set](Rsc.OvertimeRate, 15)
Dim assignment As ResourceAssignment = project.ResourceAssignments.Add(task, rsc)
assignment.Set(Assn.Start,DateTime.Parse("18-Aug-2009 8:00 AM" )
assignment.Set(Assn.Finish, DateTime.Parse("18-Aug-2009 5:00 PM" ) project.Save("ResourceAssignments.xml", SaveFileFormat.XML)
{{< /highlight >}}
