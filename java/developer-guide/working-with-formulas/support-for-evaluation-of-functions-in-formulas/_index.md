---
title: Support for Evaluation of Functions in Formulas
type: docs
weight: 40
url: /java/support-for-evaluation-of-functions-in-formulas/
---

{{% alert color="primary" %}} 

Aspose.Tasks API supports evaluating functions defined as formula expression in Extended Attribute. These include calculation of Math, General, Text, and DateTime functions.

{{% /alert %}} 
## **Calculation of Math Expressions**
1. Abs( number )
1. Atn( number )
1. Cos( number )
1. Exp( number )
1. Fix( number )
1. Int( number )
1. Log( number )
1. Rnd( number )
1. Sgn( number )
1. Sin( number )
1. Sqr( number )
1. Tan( number )

**C#**

{{< highlight csharp >}}

 public void TestSine()

{

Project project = CreateTestProjectWithCustomField(); 

// Sin(pi/2) 

project.setFormula("Sin(3.1415926/2)"); 

Task task = project.getRootTask().getChildren().getById(1); 

System.out.println(task.getExtendedAttributes().get(0).get.Value()); 

}

Project CreateTestProjectWithCustomField()

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
## **Calculation of General Functions**
The following General functions can be calculated by the API.

1. Choose( index, choice-1, choice-2, ... , choice-n|, choice-n)
1. IIf( expr, truepart, falsepart )
1. IsNumeric( expression)
1. IsNull( expression )
1. Switch( expr-1, value-1\, expr-2, value-2, ... , expr-n,value-n|, expr-n,value-n )

**C#**

{{< highlight csharp >}}

 public void TestChoose()

{

    Project project = CreateTestProjectWithCustomField();

    project.getExtendedAttributes().get(0).setFormula("Choose(3, \"This is a\", \"right\", \"choice\")");

    Task task = project.getRootTask().getChildren().getById(1);

}

public void TestIsNumeric(Values("IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))") string isNumFormula)

{

    Project project = CreateTestProjectWithCustomField();

    project.getExtendedAttributes().get(0).setFormula(isNumFormula);

}

public void TestSwitch()

{

    Project project = CreateTestProjectWithCustomField();

    project.getExtendedAttributes().get(0).setFormula("Switch(False, \"False predicate\", true, \"True predicate\")");

}

{{< /highlight >}}
## **Calculation of Text Functions**
1. Asc( string )
1. Chr( charcode )
1. Format( expression, format, firstdayofweek, firstweekofyear)
1. Instr( start,string1, string2, compare )
1. LCase( string )
1. Left( string, length )
1. Len( string )
1. LTrim( string )
1. Mid( string, start, length )
1. Right( string, length )
1. RTrim( string )
1. Space( number )
1. StrComp( string1, string2, compare )
1. StrConv( string, conversion, LCID )
1. String( number, character )
1. Trim( string )
1. UCase( string )

**Java**

{{< highlight csharp >}}

 public void TestStrConv()

{

Project project = CreateTestProjectWithCustomField();

Task task = project.getRootTask().getChildren().getById(1);

project.getExtendedAttributes().get(0).setFormula("StrConv(\"sTring and sTRINg\",3)");

project.getExtendedAttributes().get(0).setFormula("StrConv(\"sTring and sTRINg\",1)");

project.getExtendedAttributes().get(0).setFormula("StrConv(\"sTring and sTRINg\",2)");

}

public void TestStringFunction()

{

Project project = CreateTestProjectWithCustomField();

Task task = project.getRootTask().getChildren().getById(1);

project.getExtendedAttributes().get(0).setFormula("String(5 ,40)");

project.getExtendedAttributes().get(0).setFormula("String(5 ,\"Astr\")");

project.getExtendedAttributes().get(0).setFormula("String(-5 ,\"Astr\")");

}

{{< /highlight >}}
## **Calculation of Date/Time Functions**
1. CDate( expression )
1. Date ()
1. DateAdd( interval, number, date )
1. DateDiff( interval, date1, date2\, firstdayofweek, firstweekofyear )
1. DatePart( interval, date\, firstdayofweek, firstweekofyear)
1. DateSerial( year, month, day )
1. DateValue( date)
1. Day( date)
1. Hour( time )
1. IsDate( expression )
1. Minute( time)
1. Month( date)
1. Now ()
1. ProjDateAdd( date, duration, calendar )
1. ProjDateConv( expression, dateformat )
1. ProjDateDiff( date1, date2, calendar )
1. ProjDateSub( date, duration, calendar )
1. ProjDateValue( expression )
1. ProjDurConv( expression, durationunits )
1. ProjDurValue( duration )
1. Second( time )
1. Time ()
1. Timer ()
1. TimeSerial( hour, minute, second)
1. TimeValue( time)
1. Weekday( date, firstdayofweek )
1. Year( date)

**C#**

{{< highlight csharp >}}

 Project project = CreateTestProjectWithCustomField();

Task task = project.getRootTask().getChildren().getById(1);

//ProjDateDiff

project.getExtendedAttributes().get(0).setFormula("ProjDateDiff(\"03/23/2015\",\"03/18/2015\")");

project.getExtendedAttributes().get(0).setFormula("ProjDateDiff(\"03/23/2015\",\"03/25/2015\")");

//ProjDateSub

project.getExtendedAttributes().get(0).setFormula("ProjDateSub(\"3/19/2015\", \"1d\")");

//ProjDurConv

project.getExtendedAttributes().get(0).setFormula("ProjDurConv([Duration], pjHours)");

project.getExtendedAttributes().get(0).setFormula("ProjDurConv([Duration], pjWeeks)");

//Second

project.getExtendedAttributes().get(0).setFormula("Second(\"4/21/2015 2:53:41 AM\")");

//Weekday

project.getExtendedAttributes().get(0).setFormula("Weekday(\"24/3/2015\", 1)");

project.getExtendedAttributes().get(0).setFormula("Weekday(\"24/3/2015\", 2)");

project.getExtendedAttributes().get(0).setFormula("Weekday(\"24/3/2015\", 3)");

{{< /highlight >}}
