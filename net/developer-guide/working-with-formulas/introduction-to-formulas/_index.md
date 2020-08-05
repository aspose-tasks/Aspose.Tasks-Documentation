---
title: Introduction to Formulas
type: docs
weight: 10
url: /net/introduction-to-formulas/
---

{{% alert color="primary" %}} 

Aspose.Tasks API supports reading/writing formulas to MPP project files. The Formula property of the ExtendedAttributeDefinition provides the interface for reading the formula value. This section describes methods to read/write and use formulas in Aspose.Tasks.

{{% /alert %}} 

When assigning an invalid formula string to the instance of ExtendedAttributeDefinition class,FormatException is thrown
## **Formula Grammar**
Microsoft Project uses the following grammar for formula.

**Formula Grammar (Simplified)**

{{< highlight java >}}

 Formula -> Formula Binary_Op Primary | Primary

Primary -> (Formula) | Unary_Op Primary | Function | [ValidFieldName] | ValidDoubleValue | "StringLiteral"

Function -> ValidFunctionName(Args)

Args -> Args Delimiter Formula | Formula | |

Delimiter -> , | ;   Note that Delimiter is culture-specific in xml format ( , or ; ) and persistent in mpp ( , )

Binary_Op -> + | - | * | / | & | MOD | ^ | = | <> | < | >| AND | OR

Unary_Op -> NOT | + | -

{{< /highlight >}}
