---
title: Working with Task, Resource and Project Fields Calculation in Expressions
type: docs
weight: 30
url: /java/working-with-task-resource-and-project-fields-calculation-in-expressions/
---

{{% alert color="primary" %}} 

Aspose.Tasks API can use Task, Resource and Project fields as formula in expressions. Fields such as Work, Cost, Number fields, Date Time, Boolean and Project Fields such as task count and resource count can be used in formula expressions in extended attribute.

{{% /alert %}} 
## **Using Tasks and Resource Fields in Formula Calculations**
**Java**

{{< highlight csharp >}}

 private static void TaskFieldsFormula()

{

	// see this helper method below

	Project project = CreateTestProjectWithCustomField();

	ExtendedAttributeDefinition attr = project.getExtendedAttributes().get(0);

	attr.setAlias("Days from finish to deadline");

	attr.setFormula("[Deadline] - [Finish]");

	Task task = project.getRootTask().getChildren().getById(1);

	java.util.Calendar cal = java.util.Calendar.getInstance();

	cal.set(2015, 26, 3, 8,0,0);

	task.set(Tsk.DEADLINE, cal.getTime());

	project.save("SaveFile.mpp", SaveFileFormat.MPP);

}

public static Project CreateTestProjectWithCustomField()

{

	Project project = new Project();

	java.util.Calendar cal = java.util.Calendar.getInstance();

	cal.set(2015, 26, 3, 8,0,0);

	project.set(Prj.START_DATE, cal.getTime());

	ExtendedAttributeDefinition attr = new ExtendedAttributeDefinition();

	project.getExtendedAttributes().add(attr);

	attr.setFieldId(Integer.toString(ExtendedAttributeTask.Text1));

	Task task = project.getRootTask().getChildren().add("Task");

	ExtendedAttribute a = attr.createExtendedAttribute();

	task.getExtendedAttributes().add(a);

	Resource rsc = project.getResources().add("Rsc");

	ResourceAssignment assn = project.getResourceAssignments().add(task, rsc);

	return project;

}

{{< /highlight >}}


## **Using Arithmetic Expression ((1+3*(2+ -5)+8/2)^3)**
**Java**

{{< highlight csharp >}}

 Project project = CreateTestProjectWithCustomField();

ExtendedAttributeDefinition attr = project.getExtendedAttributes().get(0);

attr.setAlias("Arithmetic Expression");

attr.setFormula("(1+3*(2+ -5)+8/2)^3");

Task task = project.getRootTask().getChildren().getById(1);

System.out.println(task.getExtendedAttributes().get(0).getValue());

{{< /highlight >}}


## **Using Task Number Fields : (Outline Level + Priority + % Complete|% Complete)/2**
**Java**

{{< highlight csharp >}}

 Project project = CreateTestProjectWithCustomField();

ExtendedAttributeDefinition attr = project.getExtendedAttributes().get(0);

attr.setAlias("Task number fields");

attr.setFormula("(([Outline Level] + [Priority] + [% Complete])/2");

Task task = project.getRootTask().getChildren().getById(1);

System.out.println(task.getExtendedAttributes().get(0).getValue());

task.set(Tsk.PERCENT_COMPLETE, 50);

System.out.println(task.getExtendedAttributes().get(0).getValue());

{{< /highlight >}}
## **Formula With Boolean Values**
{{< highlight csharp >}}

 Project project = CreateTestProjectWithCustomField();

ExtendedAttributeDefinition attr = project.getExtendedAttributes().get(0);

attr.setAlias("Task number fields");

attr.setFormula("[Critical]-[Marked]+4+[Active]-Not [Active]");

Task task = project.getRootTask().getChildren().getById(1);

System.out.println("Formula with boolean values" + task.getExtendedAttributes().get(0).getValue());

{{< /highlight >}}
## **Formula With Project Fields**
**Java**

{{< highlight csharp >}}

 Project project = CreateTestProjectWithCustomField();

ExtendedAttributeDefinition attr = project.getExtendedAttributes().get(0);

attr.setAlias("Task number fields");

attr.setFormula("\"Total tasks: \" & [Task Count] & \" Total resources: \" & [Resource Count]");

Task task = project.getRootTask().getChildren().getById(1);

System.out.println("Total tasks: 1 Total resources: 0" + task.getExtendedAttributes().get(0).getValue());

{{< /highlight >}}
