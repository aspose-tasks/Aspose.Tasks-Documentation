---
title: Migrate to the latest Aspose.Tasks for Java
description: "Learn how to migrate from Aspose.Tasks for Java 8.1.0 to the latest ones."
type: docs
weight: 100
url: /java/how-to-migrate-to-aspose-tasks-for-java-8-1-0-or-higher/
---

{{% alert color="primary" %}}

Aspose.Tasks for Java 8.1.0 is a revamped version of the API that includes considerable changes from usage perspective. Key differences of both the implementations include:

- Legacy API allowed to set public fields of various project data classes such as Project, Tasks, Resource, etc. while the new implementation introduces Set and Get methods to achieve the same
- Recalculate methods required to be called manually by user in the legacy API after certain operations such as Resource Assignments. The new Aspose.Tasks for Java API performs most of such calculations automatically without user intervention required.
- The new API provides manual as well as automatic recalculation modes similar to Microsoft Project (MSP). Manual mode calculates only the necessary fields whereas automatic mode recalculates everything.  This eliminates the need of calling recalculating methods manually and improves overall API usage.

This new API is incompatible with the Legacy API and the objective of this article is to help you migrate your code to the new API.  The article shows comparative code samples of the Legacy and the new API implementation, and includes:

{{% /alert %}}

## **Setting Default Project Properties**
Aspose.Tasks' legacy API allowed setting default properties of a project by directly setting the public attributes of the Project class. In the new API implementation, however, it exposes Set and Get methods to achieve the same.

### **Legacy API Code Sample**

{{< highlight java >}}
// Create a project instance
Project prj = new Project();
// Set properties default
prj.setScheduleFromStart(true);
prj.setStartDate(prj.getStartDate());
prj.setDefaultStartTime(prj.getStartDate());
prj.setDefaultTaskType(TaskType.FixedDuration);
prj.setDefaultStandardRate(15);
prj.setDefaultOvertimeRate(12);
prj.setDefaultTaskEVMethod(EarnedValueMethodType.PercentComplete);
prj.setDefaultFixedCostAccrual(CostAccrualType.Prorated);
// Save the project to XML format
prj.save( "Project4.xml" , SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**

{{< highlight java >}}
Project project = new Project();
// Set default properties
project.set(Prj.SCHEDULE_FROM_START,new NullableBool(true));
project.set(Prj.DEFAULT_START_TIME,project.get(Prj.START_DATE));
project.set(Prj.DEFAULT_TASK_TYPE, TaskType.FixedDuration);
project.set(Prj.DEFAULT_STANDARD_RATE, 15d);
project.set(Prj.DEFAULT_OVERTIME_RATE, 12d);
project.set(Prj.DEFAULT_TASK_EV_METHOD, EarnedValueMethodType.PercentComplete);
project.set(Prj.DEFAULT_FIXED_COST_ACCRUAL, CostAccrualType.Prorated);
project.save("ProjectDefaultProps.xml", SaveFileFormat.XML);
{{< /highlight >}}

## **Creating and Adding Calendar to Project**
In order for proper functionality of Calendar items added to the Project, the legacy API required to recalculate Calendar UIDs. In the new API, however, UIDs recalculation are automatically dealt and there is no need to call the calculations manually.

### **Legacy API Code Sample**
{{< highlight java >}}
// Create a project instance
Project prj =  new Project();
// Define Calendar
Calendar cal1 = new  Calendar();
cal1.setName("no info");
Calendar cal2 = new  Calendar(1);
cal2.setName("no name");
Calendar cal3 = new Calendar( "cal3" );
prj.getCalendars().add(cal1);
prj.getCalendars().add(cal2);
prj.getCalendars().add(cal3);
prj.calcCalendarUids();
prj.save( "Project.Xml", SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**
{{< highlight java >}}
Project prj = new Project();
Calendar cal1 = prj.getCalendars().add("no info");
Calendar cal2 = prj.getCalendars().add("no name");
Calendar cal3 = prj.getCalendars().add("cal3");
prj.save("Project.Xml", SaveFileFormat.XML);
{{< /highlight >}}

## **Making a Standard Calendar**
Recalculating Calendar UIDs are no more required in the new Aspose.Tasks' API as compared to the legacy API.

### **Legacy API Code Sample**
{{< highlight java >}}
Project prj = new  Project();
//Define Calendar and make it standard
Calendar cal1 = new Calendar("My Cal");
Calendar.makeStandardCalendar(cal1);
prj.getCalendars().add(cal1);
prj.calcCalendarUids();
prj.save( "Project.Xml" , SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**
{{< highlight java >}}
//Create a project instance
Project project = new Project();
//Define Calendar and make it standard
Calendar cal1 = project.getCalendars().add("My Cal");
Calendar.makeStandardCalendar(cal1);
project.save("Project.Xml", SaveFileFormat.XML);
{{< /highlight >}}

## **Create and Adding Task to Project**
Creating a new task in the legacy API, it required to define a root task, add it to the project as its root task, and then add a new task to this root task as a child. The new API, however, doesn't need you to define the root task and takes care of it automatically while adding the first task to the project.

### **Legacy API Code Sample**
{{< highlight java >}}
Project project = new Project();
Task rootTask = new Task();
Task tskGen = new Task("Task1");
tskGen.setId(1);
tskGen.setUid (1);
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2014, 04, 23, 0, 0, 0);
tskGen.setStart(cal.getTime());
cal.set(2014, 04, 25, 0, 0, 0);
tskGen.setFinish(cal.getTime());
project.setRootTask (rootTask);
project.getRootTask().getChildren().add(tskGen);
project.save("Project.xml", SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**
{{< highlight java >}}
Project project = new Project();
Task task = project.getRootTask().getChildren().add("Task 1");
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2014,3,4,0,0,0);
task.set(Tsk.START, cal.getTime());
//set task start day
project.save("CreateTasks.xml", SaveFileFormat.XML);
{{< /highlight >}}

## **Create and Add Resource to Project**
The *set* and *get* methods have been added to the Resource class of the API for manipulating attributes related to a project's Resource.

### **Legacy API Code Sample**
{{< highlight java >}}
Project project = new Project();
Resource res =   new Resource("Res1");
res.setId (1);
res.setUid(1);
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2014, 04, 23, 0, 0, 0);
res.setStart(cal.getTime());
cal.set(2014, 04, 25, 0, 0, 0);
res.setFinish(cal.getTime());
project.getResources().add(res);
project.save("Project.xml", SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**
{{< highlight java >}}
Project project = new Project();
Resource rsc = project.getResources().add("R1");
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2014,3,4,0,0,0);
rsc.set(Rsc.START, cal.getTime());
cal.set(2014,3,10,0,0,0);
rsc.set(Rsc.FINISH, cal.getTime());
project.save("CreateResource.xml", SaveFileFormat.XML);
{{< /highlight >}}

## **Create and Add Resource Assignment to Project**
The *ResourceAssignment* class also introduces the *set* and *get* methods similar to other data collections of the API such as Tasks, Resources and Tasks Links.

### **Legacy API Code Sample**
{{< highlight java >}}
Project project = new Project();
Task tskRoot =  new Task();
Task task = new Task("Task");
Resource rsc = new Resource();
rsc.setStandardRate(BigDecimal.valueOf(10));
rsc.setOvertimeRate(BigDecimal.valueOf(15));
ResourceAssignment assignment = new ResourceAssignment(task, rsc);
assignment.setUid(1);
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2009, 8, 18, 0, 0, 0);
assignment.setStart(cal.getTime());
cal.set(2009,8,20,0,0,0);
assignment.setFinish(cal.getTime() );
project.setRootTask(tskRoot);
project.getRootTask().getChildren().add(task);
project.getResources().add(rsc);
project.getResourceAssignments().add(assignment);
project.save("project.xml", SaveFileFormat.XML);
{{< /highlight >}}

### **New Aspose.Tasks for Java 8.x Approach**
{{< highlight java >}}
Project project = new Project();
Task task = project.getRootTask().getChildren().add("Task");
Resource rsc = project.getResources().add("Rsc");
rsc.set(Rsc.STANDARD_RATE, BigDecimal.valueOf(10));
rsc.set(Rsc.OVERTIME_RATE, BigDecimal.valueOf(15));
ResourceAssignment assignment = project.getResourceAssignments().add(task, rsc);
java.util.Calendar cal = java.util.Calendar.getInstance();
cal.set(2014,3,4,0,0,0);
assignment.set(Asn.START,cal.getTime());
cal.set(2014,3,4,0,0,0);
assignment.set(Asn.FINISH, cal.getTime());
project.save("ResourceAssignments.xml", SaveFileFormat.XML);
{{< /highlight >}}
