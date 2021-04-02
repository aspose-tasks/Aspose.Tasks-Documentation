---
title: Support for Evaluation of Functions in Formulas
type: docs
weight: 40
url: /java/support-for-evaluation-of-functions-in-formulas/
---

{{% alert color="primary" %}} 

Aspose.Tasks for Java API supports evaluating functions defined as formula expression in Extended Attribute. These include the calculation of Math, General, Text, and DateTime functions.

{{% /alert %}} 
## **Calculation of Math Expressions**
1. Abs( number )
2. Atn( number )
3. Cos( number )
4. Exp( number )
5. Fix( number )
6. Int( number )
7. Log( number )
8. Rnd( number )
9. Sgn( number )
10. Sin( number )
11. Sqr( number )
12. Tan( number )

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Formulae-SupportEvaluationFunctions-CalculationOfMathExpressions.java" >}}

## **Calculation of General Functions**
The following General functions can be calculated by the API.

1. Choose( index, choice-1, choice-2, ... , choice-n|, choice-n)
2. IIf( expr, truepart, falsepart )
3. IsNumeric( expression)
4. IsNull( expression )
5. Switch( expr-1, value-1\, expr-2, value-2, ... , expr-n,value-n|, expr-n,value-n )

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Formulae-SupportEvaluationFunctions-CalculationOfGeneralFunctions.java" >}}


## **Calculation of Text Functions**
1. Asc( string )
2. Chr( charcode )
3. Format( expression, format, firstdayofweek, firstweekofyear)
4. Instr( start,string1, string2, compare )
5. LCase( string )
6. Left( string, length )
7. Len( string )
8. LTrim( string )
9. Mid( string, start, length )
10. Right( string, length )
11. RTrim( string )
12. Space( number )
13. StrComp( string1, string2, compare )
14. StrConv( string, conversion, LCID )
15. String( number, character )
16. Trim( string )
17. UCase( string )

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Formulae-SupportEvaluationFunctions-CalculationOfTextFunctions.java" >}}

## **Calculation of Date/Time Functions**
1. CDate( expression )
2. Date ()
3. DateAdd( interval, number, date )
4. DateDiff( interval, date1, date2\, firstdayofweek, firstweekofyear )
5. DatePart( interval, date\, firstdayofweek, firstweekofyear)
6. DateSerial( year, month, day )
7. DateValue( date)
8. Day( date)
9. Hour( time )
10. IsDate( expression )
11. Minute( time)
12. Month( date)
13. Now ()
14. ProjDateAdd( date, duration, calendar )
15. ProjDateConv( expression, dateformat )
16. ProjDateDiff( date1, date2, calendar )
17. ProjDateSub( date, duration, calendar )
18. ProjDateValue( expression )
19. ProjDurConv( expression, durationunits )
20. ProjDurValue( duration )
21. Second( time )
22. Time ()
23. Timer ()
24. TimeSerial( hour, minute, second)
25. TimeValue( time)
26. Weekday( date, firstdayofweek )
27. Year( date)

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Formulae-SupportEvaluationFunctions-CalculationOfDateTimeFunctions.java" >}}