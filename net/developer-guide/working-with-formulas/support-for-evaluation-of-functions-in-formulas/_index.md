---
title: Support for Evaluation of Functions in Formulas
type: docs
weight: 40
url: /net/support-for-evaluation-of-functions-in-formulas/
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

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithFormulas-CalculateMathExpressions-CalculateMathExpressions.cs" >}}
## **Calculation of General Functions**
The following General functions can be calculated by the API.

1. Choose( index, choice-1, choice-2, ... , choice-n|, choice-n)
1. IIf( expr, truepart, falsepart )
1. IsNumeric( expression)
1. IsNull( expression )
1. Switch( expr-1, value-1\, expr-2, value-2, ... , expr-n,value-n|, expr-n,value-n )

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithFormulas-CalculateGeneralFunctions-CalculateGeneralFunctions.cs" >}}
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

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithFormulas-CalculateTextFunctions-CalculateTextFunctions.cs" >}}
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

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithFormulas-CalculateDateTimeFunctions-CalculateDateTimeFunctions.cs" >}}
